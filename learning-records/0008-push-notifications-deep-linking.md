# Learning Record 0008: Push Notifications & Deep Linking Architecture

## Date: 2026-08-14

## Key Insight
1. **APNs & FCM Pipeline**: Native push notifications flow through Apple and Google push services via `expo-notifications`, requiring device token registration with `getExpoPushTokenAsync()`.
2. **Foreground vs. Background**: Foreground alerts are controlled via `setNotificationHandler()`; tap interactions are captured by `addNotificationResponseReceivedListener()`.
3. **Expo Router Auto-Routing**: Deep links from notification payloads map automatically to file-based routes (e.g. `/post/[id]`) without custom URL router parsing.

## Application to Codebase
- Request push permissions on physical devices during onboarding.
- Handle notification tap events to route directly to newly created BeReal posts.
