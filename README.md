# React Native for Angular Devs: Fast-Track Course

🌐 **Live Course Website**: [https://chewieez.github.io/react-native-for-angular-devs/](https://chewieez.github.io/react-native-for-angular-devs/)

A tailored, high-density learning track designed specifically for **Angular engineers and leads** transitioning into **React Native & Expo** mobile development.

Rather than starting from zero with basic programming concepts, this course translates the architectural patterns you already master in Angular (Services, Components, RxJS, Dependency Injection, Route Guards, Flexbox) into React Native equivalents.

---

## 📚 Course Curriculum & Lessons

| Lesson # | Module Title | Core Topics | Status |
| :--- | :--- | :--- | :--- |
| **0001** | [**Angular Lead to React Native Mental Model**](./lessons/0001-angular-to-react-native-mental-model.html) | Concept translation matrix, `View`/`Text`/`Image` primitives, Expo Dev Menu (`Cmd+D`), Metro shortcuts, Chrome DevTools. | ✅ Active |
| **0002** | [**React Context vs. Angular Services**](./lessons/0002-react-context-vs-angular-services.html) | `createContext`, `<Provider>`, `useContext`, state re-rendering mechanics vs Zone.js/Signals, Expo Router route guarding. | ✅ Active |
| **0003** | [**What is a React Hook?**](./lessons/0003-what-is-a-hook.html) | Why hooks exist, `useState`, `useEffect`, `useContext`, `useRef`, custom hooks (`useAuth`), Golden Rules of Hooks. | ✅ Active |
| **0004** | [**Forms & Controlled Inputs**](./lessons/0004-forms-and-inputs.html) | Controlled components vs. `[(ngModel)]`, `TextInput` props (`onChangeText`, `value`), keyboard handling. | ✅ Active |
| **0005** | [**Native Flexbox & Layout Masterclass**](./lessons/0005-flexbox-native-layout.html) | `flexDirection: 'column'` default, unitless dp dimensions, `flex: 1` vs web CSS, `SafeAreaView`. | ✅ Active |
| **0006** | [**FlatList vs. ScrollView & Virtualization**](./lessons/0006-flatlist-vs-scrollview.html) | Memory management on mobile, list virtualization, `FlatList` vs `ScrollView`, key extractors. | ✅ Active |
| **0007** | [**Expo Router Architecture & File-Based Routing**](./lessons/0007-expo-router-architecture.html) | File-based routing, `(tabs)`, `(auth)`, `Stack`, `Slot`, & `_layout.tsx` vs Angular `RouterModule`. | ✅ Active |
| **0008** | [**Programmatic Navigation & Modals**](./lessons/0008-programmatic-navigation-modals.html) | `router.push`, `router.replace`, `router.back`, modal presentation, route parameters. | ✅ Active |
| **0009** | **Async Data Fetching & Loading States** | `async/await`, `ActivityIndicator`, Error Boundaries vs Angular `HttpClient`/RxJS. | ⏳ Pending |
| **0010** | **Backend Integration & Persistent Storage** | Supabase/Firebase integration, local storage with `AsyncStorage` / `MMKV` key-value persistence. | ⏳ Pending |
| **0011** | **Native Camera & Image Picker** | Camera access (`expo-camera`), photo library picker (`expo-image-picker`), device permissions. | ⏳ Pending |
| **0012** | **Native Haptics, Alerts & Device Features** | `expo-haptics` feedback, `Alert.alert` dialogs, toast notifications, platform-specific code (`Platform.OS`). | ⏳ Pending |
| **0013** | **Advanced Debugging & Performance Profiling** | React DevTools, Flipper, network tab profiling, memory leak detection, JS thread performance. | ⏳ Pending |
| **0014** | **Production Builds & EAS Pipeline** | Expo Managed vs Prebuild, `eas build`, App Store / TestFlight readiness, release channels. | ⏳ Pending |

---

## 💡 Quick Concept Translation Summary

| Angular Concept | React Native / Expo Equivalent |
| :--- | :--- |
| **HTML Template (`div`, `span`)** | **JSX (`<View>`, `<Text>`)** |
| **`@Input()`** | **`props`** |
| **`@Output() EventEmitter`** | **Callback Props (`onPress={handlePress}`)** |
| **`@Injectable()` Service** | **React Context (`createContext`) + Custom Hook** |
| **`BehaviorSubject` / Signals** | **`useState()` Hook** |
| **`[(ngModel)]` / Reactive Forms** | **Controlled Components (`value` + `onChangeText`)** |
| **`CanActivate` Guard** | **`useEffect` + `router.replace()` in Expo Router** |
| **`HttpClient` / RxJS** | **`fetch` / `async-await` / Supabase JS Client** |
