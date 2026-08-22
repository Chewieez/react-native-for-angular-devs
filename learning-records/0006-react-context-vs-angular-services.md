# Learning Record 0006: React Context vs. Angular Services

## Date: 2026-08-11

## Key Insight
1. **Root Services & DI**: React Context (`createContext` + `<Provider>` + `useContext`) is the direct functional equivalent of Angular root `@Injectable()` services.
2. **Re-rendering Mechanics**: When context state updates via its setter, all consumer components re-render unless memoized.
3. **Layout Tree Providers**: Context Providers wrap root layouts (`_layout.tsx`) to supply auth, theme, and user session down the entire component tree.

## Application to Codebase
- State provider components (`AuthProvider`) wrap root layouts (`src/app/_layout.tsx`).
- Route guarding is managed declaratively via `useEffect` watching context state (`user`) and calling `router.replace()`.
