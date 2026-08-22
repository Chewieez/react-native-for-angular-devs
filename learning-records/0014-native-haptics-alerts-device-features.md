# Learning Record 0014: Native Haptics, Alerts & Device Features

## Date: 2026-08-14

## Key Insight
1. **Native Dialogs**: `Alert.alert()` uses asynchronous native OS dialogs (UIAlertController / AlertDialog) that do not block the JS thread like web `window.alert()`.
2. **Tactile Feedback**: `expo-haptics` brings physical feedback to buttons, toggles, success/error notifications, and drag gestures.
3. **Platform Branching**: Use `Platform.select()` for OS-specific style rules (e.g. iOS shadows vs. Android elevation) and platform file extensions (`.ios.tsx` / `.android.tsx`).

## Application to Codebase
- Use `Haptics.impactAsync(ImpactFeedbackStyle.Medium)` on primary button actions and photo snaps.
- Use `Alert.alert()` with `style: 'destructive'` for deletion confirmation flows.
