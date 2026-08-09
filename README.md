# Angular to React Native & Expo: Fast-Track Course for Senior Front-End Developers

A tailored, high-density learning track designed specifically for **Angular engineers and leads** transitioning into **React Native & Expo** mobile development.

Rather than starting from zero with basic programming concepts, this course translates the architectural patterns you already master in Angular (Services, Components, RxJS, Dependency Injection, Route Guards, Flexbox) into React Native equivalents.

---

## 📚 Course Curriculum & Lessons

| Lesson # | Module Title | Core Topics |
| :--- | :--- | :--- |
| **0001** | [**Angular Lead to React Native Mental Model**](./lessons/0001-angular-to-react-native-mental-model.html) | Concept translation matrix, `View`/`Text`/`Image` primitives, Expo Dev Menu (`Cmd+D`), Metro terminal shortcuts, and Chrome DevTools debugging. |
| **0002** | [**React Context vs. Angular Services**](./lessons/0002-react-context-vs-angular-services.html) | `createContext`, `<Provider>`, `useContext`, state re-rendering mechanics vs Zone.js/Signals, and Expo Router declarative route guarding. |
| **0003** | [**What is a React Hook?**](./lessons/0003-what-is-a-hook.html) | Why hooks exist for functional components, `useState`, `useEffect`, `useContext`, `useRef`, custom hooks (`useAuth`), and the Golden Rules of Hooks. |

---

## 🎯 Course Blueprint & Structure

```text
react-native-learning/
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
    └── 0003-what-is-a-hook.html
```

---

## 🚀 How Teammates Can Use This Course

1. **Clone or Share Folder**: Share the `react-native-learning` directory or host it as a Git repository.
2. **Open Lessons in Any Browser**: Double-click any `.html` file inside `lessons/` to view styled, responsive lessons with code comparisons, diagrams, and self-checks.
3. **Follow Alongside a Practice App**: Build along with any Expo project (like an Expo Router tutorial or starter app).

---

## 💡 Quick Concept Translation Summary

| Angular Concept | React Native / Expo Equivalent |
| :--- | :--- |
| **HTML Template (`div`, `span`)** | **JSX (`<View>`, `<Text>`)** |
| **`@Input()`** | **`props`** |
| **`@Output() EventEmitter`** | **Callback Props (`onPress={handlePress}`)** |
| **`@Injectable()` Service** | **React Context (`createContext`) + Custom Hook** |
| **`BehaviorSubject` / Signals** | **`useState()` Hook** |
| **`ngOnInit` / `ngOnDestroy`** | **`useEffect()` Hook** |
| **`CanActivate` Guard** | **`useEffect` + `router.replace()` in Expo Router** |
| **`HttpClient` / RxJS** | **`fetch` / `async-await` / Supabase JS Client** |
