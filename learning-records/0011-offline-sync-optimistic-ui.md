# Learning Record 0011: Offline-First Architecture & Optimistic UI

## Date: 2026-08-14

## Key Insight
1. **Zero-Latency Mobile UI**: Optimistic mutations update the client cache instantly (0ms) and perform rollback upon network failure, creating a snappy native feel.
2. **Persistent Query Cache**: TanStack React Query + `MMKV` allows instant cold-start screen rendering from disk cache before network revalidation.
3. **Network Resilience**: Seamless automatic retry queues using `@react-native-community/netinfo`.

## Application to Codebase
- Use optimistic mutations in TanStack Query for likes, RealMoji reactions, and comments.
- Persist feed queries in `MMKV` for instant app launch.
