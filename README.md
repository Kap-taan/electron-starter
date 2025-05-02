---

# 🚀 Electron App Starter with React, Node, and TypeScript

A modern starter template for building desktop apps using **Electron**, **React 19**, **TypeScript**, and **Vite**. It supports fast development with HMR for React and production-ready builds across **macOS**, **Windows**, and **Linux**.

---

## 📦 Project Setup

Clone the repository and install dependencies:

```bash
git clone <repository_url>
cd <project_directory>
npm install
```

---

## 🗂️ Project Structure

* `src/`: Source code for the React frontend and Electron main process.
* `tsconfig.app.json`: TypeScript config for the React app.
* `src/electron/tsconfig.json`: TypeScript config for the Electron process.
* `tsconfig.node.json`: TypeScript config for Vite/Electron configs.

---

## 🔧 Scripts

### 🧪 Development

#### `dev:react`

```bash
npm run dev:react
```

Starts the Vite development server with Hot Module Replacement (HMR) for React.

#### `dev:electron`

```bash
npm run dev:electron
```

Launches the Electron app (should be run after starting `dev:react`).

---

### 🏗️ Build

#### `build`

```bash
npm run build
```

Builds the production React app using Vite and cleans up TypeScript build info.

#### `transpile:electron`

```bash
npm run transpile:electron
```

Transpiles Electron's TypeScript code using `src/electron/tsconfig.json`.

---

### 📦 Distribute

#### `dist:mac`

```bash
npm run dist:mac
```

Builds and packages the app for **macOS (ARM64)**.

#### `dist:win`

```bash
npm run dist:win
```

Builds and packages the app for **Windows (x64)**.

#### `dist:linux`

```bash
npm run dist:linux
```

Builds and packages the app for **Linux (x64)**.

---

### 🔍 Preview

```bash
npm run preview
```

Previews the production build of the React app in the browser (useful for frontend testing).

---

### 🧹 Lint

```bash
npm run lint
```

Runs ESLint to check for code issues and enforce style.

---

## ⚙️ Customize for Your Project

* **Install Libraries**: Add routing, state management, or UI libraries as needed.

  ```bash
  npm install react-router-dom
  ```

* **Electron Configuration**: Modify `src/electron/main.ts` for window settings, menus, etc.

* **TypeScript Settings**: Adjust `tsconfig.app.json` or `src/electron/tsconfig.json` for your needs.

---

## 📝 Final Notes

This starter provides a clean and flexible foundation to build modern cross-platform desktop apps. With a streamlined workflow, you can rapidly prototype, develop, and package your app for multiple OS targets.

---