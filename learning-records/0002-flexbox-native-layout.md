# Learning Record 0002: Native Flexbox & Layout Masterclass

## Date: 2026-08-09

## Key Insight
1. **Column Direction Default**: In React Native Yoga engine, every `View` defaults to `flexDirection: 'column'` (vertical stacking) instead of web's `row`.
2. **Unitless DP Dimensions**: Dimensions are unitless density-independent pixels (`width: 100`, not `100px` or `100rem`).
3. **Screen Insets & Notches**: Web `env(safe-area-inset-*)` translates directly to `SafeAreaView` / `useSafeAreaInsets()` from `react-native-safe-area-context`.

## Application to Codebase
- Build responsive mobile screens using `flex: 1` container hierarchies.
- Wrap root layouts in `SafeAreaProvider` and header/footer bars in `SafeAreaView`.
