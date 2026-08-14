# Learning Record 0011: Offline-First Architecture & Optimistic UI

## Date: 2026-08-14

## Key Insight
1. **Angular PWA vs. Native Mobile**:
   - **App Shell**: PWAs rely on Service Worker caching of HTML/JS; Native compiles JS bundles directly into the binary (`.ipa`/`.aab`) with zero cold-boot network overhead.
   - **Storage Engine**: PWA `IndexedDB` is susceptible to 7-day Safari cache eviction; native `MMKV` is permanent, non-evictable, and ~30x faster via C++ memory-mapped buffers.
   - **Background Sync**: Native `NetInfo` + background queues work reliably across iOS and Android without browser sandbox limits.
2. **Zero-Latency Mobile UI**: Optimistic mutations in TanStack Query update the client cache instantly (0ms) and perform rollback upon network failure.
3. **Persistent Query Cache**: TanStack React Query + `MMKV` allows instant cold-start screen rendering from disk cache before network revalidation.

## Application to Codebase
- Use optimistic mutations in TanStack Query for likes, RealMoji reactions, and comments.
- Persist feed queries in `MMKV` for instant app launch.
