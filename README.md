# React Native for Angular Devs: Fast-Track Course

🌐 **Live Course Website**: [https://chewieez.github.io/react-native-for-angular-devs/](https://chewieez.github.io/react-native-for-angular-devs/)

A tailored, high-density learning track designed specifically for **Angular engineers and leads** transitioning into **React Native & Expo** mobile development.

Rather than starting from zero with basic programming concepts, this course translates the architectural patterns you already master in Angular (Services, Components, RxJS, Dependency Injection, Route Guards, Flexbox) into React Native equivalents.

---

## 📚 Course Curriculum & Enterprise Pillars

### 🏛️ Pillar 1: Core Paradigms, Native UI & Layout (Foundations)
| Lesson # | Module Title | Core Topics | Status |
| :--- | :--- | :--- | :--- |
| **0001** | [**Angular Lead to React Native & Expo Mental Model**](./lessons/0001-angular-to-react-native-mental-model.html) | Concept translation matrix, `View`/`Text`/`Image` primitives, Expo Dev Menu (`Cmd+D`), Metro shortcuts, Chrome DevTools. | ✅ Active |
| **0002** | [**Native Flexbox & Layout Masterclass**](./lessons/0002-flexbox-native-layout.html) | `flexDirection: 'column'` default, unitless dp dimensions, `flex: 1` vs web CSS, `SafeAreaView`. | ✅ Active |
| **0003** | [**FlatList vs. ScrollView & Virtualization**](./lessons/0003-flatlist-vs-scrollview.html) | Memory management on mobile, list virtualization, `FlatList` vs `ScrollView`, key extractors, cell recycling. | ✅ Active |

### ⚡ Pillar 2: Reactivity, Hooks, Forms & Context
| Lesson # | Module Title | Core Topics | Status |
| :--- | :--- | :--- | :--- |
| **0004** | [**What is a React Hook?**](./lessons/0004-what-is-a-hook.html) | Why hooks exist, `useState`, `useEffect`, `useContext`, `useRef`, custom hooks (`useAuth`), Golden Rules of Hooks. | ✅ Active |
| **0005** | [**Forms & Controlled Inputs**](./lessons/0005-forms-and-inputs.html) | Controlled components vs. `[(ngModel)]`, `TextInput` props (`onChangeText`, `value`), keyboard handling. | ✅ Active |
| **0006** | [**React Context vs. Angular Services**](./lessons/0006-react-context-vs-angular-services.html) | `createContext`, `<Provider>`, `useContext`, state re-rendering mechanics vs Zone.js/Signals, Expo Router route guarding. | ✅ Active |

### 🧭 Pillar 3: Navigation, Modals & Deep Linking
| Lesson # | Module Title | Core Topics | Status |
| :--- | :--- | :--- | :--- |
| **0007** | [**Expo Router Architecture & File-Based Routing**](./lessons/0007-expo-router-architecture.html) | File-based routing, `(tabs)`, `(auth)`, `Stack`, `Slot`, & `_layout.tsx` vs Angular `RouterModule`. | ✅ Active |
| **0008** | [**Programmatic Navigation & Modals**](./lessons/0008-programmatic-navigation-modals.html) | `router.push`, `router.replace`, `router.back`, modal presentation, route parameters (`useLocalSearchParams`). | ✅ Active |
| **0009** | [**Push Notifications & Deep Linking Architecture**](./lessons/0009-push-notifications-deep-linking.html) | APNs/FCM push tokens (`expo-notifications`), notification handling, auto-routing via Expo Router deep links. | ✅ Active |

### 🌐 Pillar 4: Data Pipelines, Storage & Offline Architecture
| Lesson # | Module Title | Core Topics | Status |
| :--- | :--- | :--- | :--- |
| **0010** | [**Async Data Fetching & Loading States**](./lessons/0010-async-data-fetching.html) | `async/await`, `ActivityIndicator`, Error Boundaries vs Angular `HttpClient`/RxJS. | ✅ Active |
| **0011** | [**Backend Integration & Persistent Storage**](./lessons/0011-backend-integration-persistent-storage.html) | Supabase/Firebase integration, local storage with `AsyncStorage` / `MMKV` key-value persistence. | ✅ Active |
| **0012** | [**Offline-First Architecture & Optimistic UI**](./lessons/0012-offline-sync-optimistic-ui.html) | TanStack Query caching, fast disk persistence (`MMKV`), instant 0ms optimistic mutations. | ✅ Active |

### 🛡️ Pillar 5: Device Hardware, Animations & Production
| Lesson # | Module Title | Core Topics | Status |
| :--- | :--- | :--- | :--- |
| **0013** | [**Native Camera & Image Picker**](./lessons/0013-native-camera-image-picker.html) | Camera access (`expo-camera`), photo library picker (`expo-image-picker`), device permissions. | ✅ Active |
| **0014** | [**Native Haptics, Alerts & Device Features**](./lessons/0014-native-haptics-alerts-device-features.html) | `expo-haptics` feedback, `Alert.alert` dialogs, toast notifications, platform-specific code (`Platform.OS`). | ✅ Active |
| **0015** | [**Hardware Biometrics & Encrypted Storage**](./lessons/0015-hardware-biometrics-secure-storage.html) | iOS Keychain & Android KeyStore (`expo-secure-store`), FaceID / TouchID (`expo-local-authentication`). | ✅ Active |
| **0016** | [**60/120 FPS Native Gestures & Animations**](./lessons/0016-fluid-gestures-reanimated.html) | UI-thread Worklets (`react-native-reanimated`), pinch/pan gestures (`react-native-gesture-handler`), spring physics. | ✅ Active |
| **0017** | [**Advanced Debugging & Performance Profiling**](./lessons/0017-advanced-debugging-performance-profiling.html) | React DevTools, Flipper, network tab profiling, memory leak detection, JS thread performance. | ✅ Active |
| **0018** | [**Production Builds & EAS Pipeline**](./lessons/0018-production-builds-eas-pipeline.html) | Expo Managed vs Prebuild, `eas build`, App Store / TestFlight readiness, release channels. | ✅ Active |

---

## 💡 Quick Concept Translation Summary

| Concept | Angular (Web) | React Native (Mobile) |
| :--- | :--- | :--- |
| **UI & Component Primitives** | HTML Template (`<div>`, `<span>`, `<p>`, `<img>`) | Functional JSX (`<View>`, `<Text>`, `<Image>` / `expo-image`) |
| **Component Inputs** | `@Input() name: string` / `input()` signal | Component Props: `props.name` / `{ name }: Props` |
| **Event Emission** | `@Output() changed = new EventEmitter()` | Callback Props (`onPress={handlePress}`, `onChanged(val)`) |
| **Conditionals** | `*ngIf="condition"` / `@if (condition)` | `{condition && <Component />}` / Ternary (`condition ? <A /> : <B />`) |
| **Loops & Lists** | `*ngFor="let item of items; trackBy: id"` / `@for` | `<FlatList data={items} keyExtractor={item => item.id} />` |
| **Content Projection / Slots** | `<ng-content>` / `<ng-content select="...">` | `props.children` / Named JSX slot props (`header={...}`) |
| **Local & Shared State** | Angular Signals (`signal()`) / `BehaviorSubject` | `useState()` Hook / React Context / Zustand |
| **Computed / Derived State** | `computed(() => ...)` | `useMemo(() => ..., [deps])` |
| **Lifecycle & Cleanup** | `ngOnInit`, `ngOnDestroy` / `takeUntilDestroyed()` | `useEffect(() => { return () => cleanup(); }, [deps])` |
| **Root Services & DI** | `@Injectable({ providedIn: 'root' })` | React Context (`createContext`) + Custom Hook (`useAuth()`) |
| **Native Layout Engine** | Web CSS Box Model (SCSS, `px`, `rem`, `flex-direction: row`) | Yoga Flexbox Engine (Unitless dp, `flex-direction: column` default) |
| **Screen Insets & Notches** | Viewport Units (`100dvh`) / Safe Area CSS env() | `SafeAreaView` (`react-native-safe-area-context`) |
| **Forms & Inputs** | `ReactiveFormsModule` (`FormGroup`, `FormControl`) | Controlled Inputs (`value` + `onChangeText`) / `react-hook-form` + `zod` |
| **List Virtualization** | `*cdkVirtualFor` (Angular CDK) | `<FlatList>` / `@shopify/flash-list` (Recycled Native Cells) |
| **Routing Architecture** | `RouterModule` + `<router-outlet>` | `Expo Router` (File-based routes in `app/` + `_layout.tsx`) |
| **Route Guards & Redirects** | `CanActivateFn` / `CanDeactivateFn` | Root Layout `useEffect()` + `router.replace()` redirect logic |
| **HTTP & Server State** | `HttpClient` + RxJS Observables | `fetch()` / Axios + `@tanstack/react-query` (`useQuery`, `useMutation`) |
| **Persistent Storage** | `localStorage` / `IndexedDB` | `react-native-mmkv` (JSI sync disk storage) / SQLite |
| **Secure Hardware Secrets** | HTTP-Only Secure Cookies / Web Crypto | `expo-secure-store` (iOS Keychain & Android KeyStore Enclave) |
| **Biometric Authentication** | WebAuthn API | `expo-local-authentication` (FaceID, TouchID, Fingerprint) |
| **Device Hardware & Media** | HTML5 `<input type="file">` / MediaDevices | `expo-camera` (`CameraView`) + `expo-image-picker` |
| **Haptics & Alerts** | `window.alert()` (Blocking) / Web Vibration API | `Alert.alert()` (Native OS Dialog) + `expo-haptics` (Taptic Engine) |
| **Gestures & Animations** | `@angular/animations` / CSS transitions | `Reanimated 3` (UI Worklets) + `react-native-gesture-handler` (`GestureDetector`) |
| **Push & Deep Linking** | Web Push API / Service Workers | `expo-notifications` (APNs / FCM) + Expo Router Universal Links |
| **Offline-First & Sync** | `@angular/pwa` Service Worker caching | TanStack Query Sync Persister + NetInfo + Optimistic Rollbacks |
| **Compilation & Builds** | `ng build` &rarr; Static Web Assets (`dist/`) | `EAS Build` &rarr; Native Signed Binaries (`.ipa` / `.aab`) |
| **Performance Tuning** | `ChangeDetectionStrategy.OnPush` / Zone.js | `React.memo()` / `useCallback` / Hermes JS + TurboModules |
