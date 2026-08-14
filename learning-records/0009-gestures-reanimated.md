# Learning Record 0009: Fluid Gestures & UI-Thread Animations

## Date: 2026-08-14

## Key Insight
1. **Worklets & UI Thread**: `react-native-reanimated` compiles animation functions to execute on the native UI thread, guaranteeing 60/120 FPS animations independent of JS event loop pressure.
2. **Shared Values**: Use `useSharedValue` and `useAnimatedStyle` instead of React `useState` to drive fluid animations without triggering component re-renders.
3. **Declarative Gestures**: `react-native-gesture-handler` (`Gesture.Pinch()`, `Gesture.Pan()`) integrates seamlessly with `useAnimatedStyle` for interactive photo manipulations.

## Application to Codebase
- Implement pinch-to-zoom on BeReal camera viewfinder and photo feed items.
- Use `withSpring()` for tactile reaction buttons (RealMojis).
