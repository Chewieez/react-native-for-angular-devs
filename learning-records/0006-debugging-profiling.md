# Learning Record 0006: Advanced Debugging & Performance Profiling

## Date: 2026-08-14

## Key Insight
1. **Thread Separation**: The JavaScript thread handles logic and React reconciliation; the UI (native) thread handles rendering and gesture frames.
2. **Memoization Equivalent to Angular OnPush**: `React.memo(Component)` combined with `useCallback` for event handlers prevents unnecessary re-rendering across component subtrees.
3. **FlatList Virtualization Tuning**: In large image feeds, use `initialNumToRender`, `maxToRenderPerBatch`, `windowSize`, and `removeClippedSubviews` to prevent memory blowouts.

## Application to Codebase
- Memoize feed item cards in feed lists with `React.memo`.
- Maintain stable event callback references with `useCallback`.
