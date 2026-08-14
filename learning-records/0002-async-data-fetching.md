# Learning Record 0002: Async Data Fetching & Loading States

## Date: 2026-08-14

## Key Insight
In Angular, asynchronous data pipelines are managed via RxJS Observables, `HttpClient`, and template unwrapping via `| async`. In React Native:
1. **Asynchronous Fetching**: Encapsulated into Custom Hooks (e.g. `useFeedData()`) using standard `async/await` and local state flags (`data`, `loading`, `error`).
2. **Native Spinners**: Use `<ActivityIndicator size="large" color="#007AFF" />` rather than CSS spinners for smooth platform-native loading animations.
3. **Pull-to-Refresh**: Directly bind `RefreshControl` into `FlatList` with `refreshing={loading}` and `onRefresh={refetch}`.

## Application to Codebase
- Encapsulate data fetching into custom hooks in `src/hooks/`.
- Render `<ActivityIndicator>` conditionally in screen views when initial datasets load.
- Wire `RefreshControl` into feed and list views for smooth pull-down revalidation.
