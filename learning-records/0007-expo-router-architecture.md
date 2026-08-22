# Learning Record 0007: Expo Router Architecture & File-Based Navigation

## Date: 2026-08-12

## Key Insight
1. **File-Based Routing**: Expo Router maps files in `app/` directory directly to navigation routes (matching Next.js App Router and replacing Angular `RouterModule`).
2. **Layout Hierarchies**: `_layout.tsx` defines nested stacks, tab bars (`<Tabs>`), and modal containers (`<Stack>`) — acting as `<router-outlet>`.
3. **Route Groups**: Parentheses folders `(tabs)` and `(auth)` group routes logically without affecting URL path structure.

## Application to Codebase
- Structure screens under `app/(auth)/` and `app/(tabs)/`.
- Use `app/_layout.tsx` for global providers, safe areas, and root routing guards.
