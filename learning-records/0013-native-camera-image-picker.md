# Learning Record 0013: Native Camera & Image Picker

## Date: 2026-08-14

## Key Insight
1. **Permissions First**: Native devices strictly require runtime OS permission prompts via `useCameraPermissions()` or `ImagePicker.requestMediaLibraryPermissionsAsync()` before hardware access.
2. **Local File URIs**: Mobile file pickers produce local disk paths (`file:///var/mobile/.../temp.jpg`) rather than in-memory browser File objects.
3. **Binary Storage Uploads**: Uploading to cloud object storage (Supabase / S3) requires reading local URIs as base64 or binary buffers using `expo-file-system`.

## Application to Codebase
- Encapsulate photo picking in `src/utils/imagePicker.ts`.
- Build camera screen with `expo-camera` (`CameraView`) for BeReal dual-photo captures.
