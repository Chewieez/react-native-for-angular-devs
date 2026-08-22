# Learning Record 0003: FlatList vs. ScrollView & High-Performance Virtualization

## Date: 2026-08-10

## Key Insight
1. **ScrollView vs FlatList**: `ScrollView` renders all child components at once into memory; `FlatList` virtualizes and recycles cells, only rendering items currently in or near viewport.
2. **cdkVirtualFor Equivalent**: `FlatList` is the direct native equivalent to Angular CDK Virtual Scroll (`*cdkVirtualFor`).
3. **Key Extraction**: Always provide `keyExtractor={(item) => item.id}` (equivalent to Angular `trackBy: item.id`) to avoid unnecessary cell re-renders.

## Application to Codebase
- Use `FlatList` for feeds, comments, and long lists.
- Optimize with `windowSize`, `initialNumToRender`, and `removeClippedSubviews`.
