# Learning Record 0017: Advanced Debugging & Performance Profiling

## Date: 2026-08-14

## Key Insight
1. **Thread Separation vs. Single Browser Thread**: Angular runs on the single browser main thread. React Native separates the **JavaScript Thread** (logic, state updates, React reconciliation) from the **UI Native Thread** (layout, pixels, 60/120 FPS gesture interactions).
2. **OnPush & trackBy Equivalents**: 
   - `ChangeDetectionStrategy.OnPush` -> `React.memo(Component)`
   - `trackBy: item.id` -> `keyExtractor={(item) => item.id}`
   - `ngZone.runOutsideAngular()` -> UI-Thread Reanimated Worklets
3. **FlatList Virtualization**: Direct equivalent to Angular CDK `cdk-virtual-scroll-viewport`. Tuned with `windowSize`, `removeClippedSubviews`, and `maxToRenderPerBatch` for memory-safe photo feeds.

## Application to Codebase
- Memoize list items (e.g. `PostCard`) with `React.memo` and wrap handler callbacks in `useCallback`.
- Inspect UI/JS FPS with Expo Dev Menu (Cmd+D / Cmd+M) Performance Monitor.
