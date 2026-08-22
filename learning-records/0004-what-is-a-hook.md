# Learning Record 0004: What is a React Hook?

## Date: 2026-08-10

## Key Insight
1. **Hooks vs Class Properties**: React function components use hooks (`useState`, `useEffect`, `useRef`, `useContext`) to tap into React runtime capabilities without classes.
2. **Golden Rules of Hooks**: Only call hooks at top level; never inside loops, conditions, or nested functions.
3. **Custom Hooks**: Extract stateful logic into reusable functions (e.g. `useAuth()`, `useDebounce()`) — direct equivalent to Angular injectable helper services.

## Application to Codebase
- Encapsulate reusable domain logic in custom hooks under `src/hooks/`.
- Replace Angular component lifecycle methods with `useEffect` dependency array patterns.
