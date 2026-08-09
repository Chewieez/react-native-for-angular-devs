# Learning Record 0001: React Context vs. Angular Services

## Date: 2026-08-09

## Key Insight
React Context (`createContext` + `<Provider>` + `useContext`) is the direct functional equivalent of Angular root `@Injectable()` services. Instead of RxJS subscriptions or Signals, React triggers component re-renders when the state setter (`setUser`) updates the Provider value.

## Application to Codebase
- State provider components (`AuthProvider`) wrap root layouts (`_layout.tsx`).
- Route guarding is managed declaratively via `useEffect` watching context state (e.g. `user`) and calling Expo Router's `router.replace()`.
- Debugging state flow is straightforward using Metro console logs inside `useEffect` state observers.
