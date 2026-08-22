# Learning Record 0015: Hardware Biometrics & Encrypted Storage

## Date: 2026-08-14

## Key Insight
1. **Hardware Enclaves**: Sensitive session tokens and cryptographic secrets must be stored in iOS Keychain and Android KeyStore via `expo-secure-store`.
2. **Biometric Verification**: `expo-local-authentication` provides FaceID/TouchID/Fingerprint authentication prompts with device passcode fallback.
3. **Storage Tiering**: Use `expo-secure-store` for secrets/tokens (2KB limit) and SQLite / `MMKV` for high-volume general data.

## Application to Codebase
- Securely store Supabase session refresh tokens in `SecureStore`.
- Protect account settings and profile deletion with `LocalAuthentication.authenticateAsync()`.
