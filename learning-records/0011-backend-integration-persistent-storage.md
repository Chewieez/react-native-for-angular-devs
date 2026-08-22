# Learning Record 0011: Backend Integration & Persistent Storage

## Date: 2026-08-13

## Key Insight
1. **Async Storage Persistence**: `@react-native-async-storage/async-storage` runs asynchronously to avoid blocking the UI thread.
2. **Supabase Storage Adapter**: Providing `AsyncStorage` / `MMKV` to `createClient()` enables automatic token hydration, session rotation, and header attachment.
3. **Session Hydration**: App boot requires an explicit `isLoading` state in `AuthContext` while `supabase.auth.getSession()` resolves from native storage.

## Application to Codebase
- Initialize `supabase` client with `auth.storage = AsyncStorage` in `src/lib/supabase/client.ts`.
- Guard Expo Router navigation in `src/app/_layout.tsx` by verifying `isLoading === false` before redirecting.
