# Learning Record 0005: Forms & Controlled Inputs

## Date: 2026-08-11

## Key Insight
1. **Controlled Components**: `TextInput` binds `value` and `onChangeText` directly to React state (equivalent to `[(ngModel)]` / Reactive Forms).
2. **Mobile Keyboard Ergonomics**: On mobile, the software keyboard overlays UI. Handle with `KeyboardAvoidingView` and `TouchableWithoutFeedback` + `Keyboard.dismiss()`.
3. **Validation Architecture**: Combine `react-hook-form` with `zod` for declarative schema validation matching Angular `FormGroup` with strong TypeScript type inference.

## Application to Codebase
- Wrap form screens in `KeyboardAvoidingView` with platform-specific behavior (`behavior={Platform.OS === 'ios' ? 'padding' : undefined}`).
- Use `react-hook-form` + `zod` for auth and profile editing forms.
