# Learning Record 0010: Async Data Fetching & Loading States

## Date: 2026-08-13

## Key Insight
1. **HttpClient & RxJS vs TanStack Query**: Translating Angular `HttpClient` + `switchMap` + `| async` pipe to TanStack React Query (`useQuery`, `useMutation`).
2. **Native Loading Indicators**: Mobile replaces web spinner CSS with native `<ActivityIndicator size="large" color="#..." />`.
3. **Error Boundaries**: Catch render errors declaratively with React Error Boundaries matching Angular Global ErrorHandlers.

## Application to Codebase
- Wrap data-fetching components with TanStack Query hooks.
- Render `<ActivityIndicator>` during initial fetch and skeleton loaders for feeds.
