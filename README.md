# 📋 Task Management - To-Do List App

A modern, animated, and scalable mobile app built with **React Native**, **Expo**, **TypeScript**, and **NativeWind**. This app helps users manage tasks within projects, track time estimates, and stay productive with a clean UI and smooth animations.

---

## 🚀 Features

- ✅ Task management with status: `Todo`, `InProgress`, `Pending`, `Done`, `Cancel`
- 🧠 Tasks require estimate before starting, and actual time before marking done
- ⏱ Time estimate warnings when 80% used
- 📊 Visual overview of project progress
- 🧩 Organized and maintainable folder structure
- 💨 Smooth UI with **Reanimated** and **NativeWind**
- 🎨 Tailwind-style utility-first styling with **NativeWind v4**

---

## 🧱 Tech Stack

| Tech                     | Description                            |
|--------------------------|----------------------------------------|
| [Expo SDK 50+]           | React Native runtime & tooling         |
| [React Native]           | Cross-platform mobile development      |
| [TypeScript]             | Static typing                          |
| [NativeWind v4]          | Tailwind CSS in React Native           |
| [TailwindCSS v3.4.17]    | Utility-first CSS framework            |
| [React Native Reanimated]| Declarative animations                 |
| [React Navigation]       | Navigation between screens             |
| [AsyncStorage]           | Local data storage                     |

---

## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/task-management-app.git
cd task-management-app
```

### 2. Install dependencies

```bash
yarn install
```

### 3. Install native dependencies

```bash
yarn expo install nativewind react-native-reanimated@~3.17.4 react-native-safe-area-context@5.4.0
```

### 4. Install Tailwind & Prettier plugins

```bash
yarn add -D tailwindcss@^3.4.17 prettier-plugin-tailwindcss
```

### 5. Initialize Tailwind (if not already)

```bash
npx tailwindcss init
```

Ensure `tailwind.config.js` includes:

```js
module.exports = {
  content: [
    "./app/**/*.{js,ts,jsx,tsx}",
    "./components/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

---

## ▶️ Running the App

```bash
yarn start
# or
npx expo start
```

---

## 📁 Folder Structure

```
.
├── app/                # Screens (Expo Router)
├── components/         # Shared UI components
├── hooks/              # Custom React hooks
├── constants/          # Theme, icons, etc.
├── assets/             # Fonts, images, svgs
├── global.css          # TailwindCSS base
├── tailwind.config.js  # TailwindCSS configuration
├── metro.config.js     # Expo + NativeWind config
└── .gitignore          # Git exclusions
```

---

## 🧩 NativeWind Notes

- ✅ Uses **NativeWind v4** (no Babel plugin required)
- ✅ Compatible only with **TailwindCSS v3** — do NOT use v4+
- ✅ Tailwind styles work on core components (`View`, `Text`, `ScrollView`, etc.)
- ❗ Custom components must be wrapped with `styled()` if using Tailwind classes
- 🗂️ `.tailwind/` cache folder is ignored via `.gitignore`

---

## 💅 Prettier Tailwind Plugin (Optional)

Ensure your `.prettierrc` or VSCode uses:

```json
{
  "plugins": ["prettier-plugin-tailwindcss"]
}
```

To auto-sort classnames.

---

## 🧪 Testing (optional)

Coming soon.

---

## 📦 Build for Production

```bash
eas build --platform android
# or
eas build --platform ios
```

---

## 🤝 Contributing

Pull requests and feature ideas are welcome. Please open an issue or discussion first to propose changes.

---

## 📄 License

MIT © 2025 [Your Name]
