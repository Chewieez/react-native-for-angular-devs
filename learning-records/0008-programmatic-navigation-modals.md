# Learning Record 0008: Programmatic Navigation & Modals

## Date: 2026-08-12

## Key Insight
1. **Programmatic Navigation**: Use `router.push()`, `router.replace()`, and `router.back()` from `useRouter()` (equivalent to Angular `Router.navigate()`).
2. **Route Parameters**: Read dynamic params and search params with `useLocalSearchParams<Type>()`.
3. **Native Modal Presentation**: Expo Router supports native presentation styles (`presentation: 'modal'`, `'formSheet'`) via stack layout options.

## Application to Codebase
- Trigger transitions and sheet modals via `router.push('/modal')`.
- Read item details with `useLocalSearchParams<{ id: string }>()`.
