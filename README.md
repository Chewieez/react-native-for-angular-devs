# React Native for Angular Devs: Fast-Track Course

A tailored, high-density learning track designed specifically for **Angular engineers and leads** transitioning into **React Native & Expo** mobile development.

Rather than starting from zero with basic programming concepts, this course translates the architectural patterns you already master in Angular (Services, Components, RxJS, Dependency Injection, Route Guards, Flexbox) into React Native equivalents.

---

## 📚 Course Curriculum & Lessons

| Lesson # | Module Title | Core Topics | Status |
| :--- | :--- | :--- | :--- |
| **0001** | [**Angular Lead to React Native Mental Model**](./lessons/0001-angular-to-react-native-mental-model.html) | Concept translation matrix, `View`/`Text`/`Image` primitives, Expo Dev Menu (`Cmd+D`), Metro shortcuts, Chrome DevTools. | ✅ Complete |
| **0002** | [**React Context vs. Angular Services**](./lessons/0002-react-context-vs-angular-services.html) | `createContext`, `<Provider>`, `useContext`, state re-rendering mechanics vs Zone.js/Signals, Expo Router route guarding. | ✅ Complete |
| **0003** | [**What is a React Hook?**](./lessons/0003-what-is-a-hook.html) | Why hooks exist, `useState`, `useEffect`, `useContext`, `useRef`, custom hooks (`useAuth`), Golden Rules of Hooks. | ✅ Complete |
| **0004** | [**Forms & Controlled Inputs**](./lessons/0004-forms-and-inputs.html) | Controlled components vs. `[(ngModel)]`, `TextInput` props (`onChangeText`, `value`), keyboard handling. | ✅ Complete |
| **0005** | [**Native Flexbox & Layout Masterclass**](./lessons/0005-flexbox-native-layout.html) | `flexDirection: 'column'` default, unitless dp dimensions, `flex: 1` vs web CSS, `SafeAreaView`. | ✅ Complete |
| **0006** | [**FlatList vs. ScrollView & Virtualization**](./lessons/0006-flatlist-vs-scrollview.html) | Memory management on mobile, list virtualization, `FlatList` vs `ScrollView`, key extractors. | ✅ Complete |

---

## 🎯 Course Blueprint & Structure

```text
react-native-for-angular-devs/
├── README.md                 # Course homepage and lesson index
├── MISSION.md                # Overall mission & learning goals
├── RESOURCES.md              # Official docs, debugging guides, community links
├── NOTES.md                  # Angular-to-React concept translation cheat sheet
├── assets/
│   └── style.css             # Clean Tufte-inspired responsive HTML typography
├── learning-records/         # Architectural decision records & key takeaways
│   └── 0001-context-vs-services.md
└── lessons/                  # Interactive, self-contained HTML lessons
    ├── 0001-angular-to-react-native-mental-model.html
    ├── 0002-react-context-vs-angular-services.html
    ├── 0003-what-is-a-hook.html
    ├── 0004-forms-and-inputs.html
    ├── 0005-flexbox-native-layout.html
    └── 0006-flatlist-vs-scrollview.html
```

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
