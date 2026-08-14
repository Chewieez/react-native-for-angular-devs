# Learning Record 0003: Backend Integration & Persistent Storage

## Date: 2026-08-14

## Key Insight
In Angular web applications, auth tokens are stored in synchronous `localStorage` and attached via `HttpInterceptor`. In React Native:
1. **Async Storage Persistence**: `@react-native-async-storage/async-storage` runs asynchronously to avoid blocking the UI thread.
2. **Supabase Storage Adapter**: By providing `AsyncStorage` to `createClient()`, the Supabase client handles token hydration, token rotation, and header attachment automatically.
3. **Session Hydration**: App boot requires an explicit `isLoading` state in `AuthContext` while `supabase.auth.getSession()` resolves from native storage, preventing false unauthenticated redirects.

## Application to Codebase
- Initialize `supabase` client with `auth.storage = AsyncStorage` in `src/lib/supabase/client.ts`.
- Guard Expo Router navigation in `src/app/_layout.tsx` by verifying `isLoading === false` before redirecting.
