# Learning Record 0001: Angular Lead to React Native Mental Model

## Date: 2026-08-09

## Key Insight
1. **Framework vs. Library**: Angular is an opinionated framework; React Native is a declarative UI library with native bridge/JSI bindings.
2. **Native Primitives**: No HTML DOM (`div`, `span`, `p`, `img`). Instead, use native primitives (`View`, `Text`, `Image` / `expo-image`).
3. **Uni-Directional Data Flow**: Props pass data down; callbacks pass events up (`onPress={handlePress}`).

## Application to Codebase
- Use `<View>` and `<Text>` for layout and copy.
- Leverage Expo Dev Menu (Cmd+D / Cmd+M) and Chrome DevTools for high-efficiency debugging.
