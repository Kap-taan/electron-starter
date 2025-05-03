---
# 🚀 Electron App Starter with React, Node, and TypeScript

A modern starter template for building cross-platform desktop apps using **Electron**, **React 19**, **TypeScript**, and **Vite**. It supports fast development with HMR and production-ready builds for **macOS**, **Windows**, and **Linux**.
---

## 📦 Project Setup

Clone the repository and install dependencies:

```bash
git clone https://github.com/Kap-taan/electron-starter.git <CUSTOM_NAME>
cd <CUSTOM_NAME>
npm install
```

---

## 🗂️ Project Structure

- `src/`: Source code for the React frontend and Electron main process.
- `tsconfig.app.json`: TypeScript config for the React app.
- `src/electron/tsconfig.json`: TypeScript config for the Electron main process.
- `tsconfig.node.json`: TypeScript config used by tooling like Vite and Electron.

---

## 🔧 Scripts

### 🧪 Development

#### `dev`

```bash
npm run dev
```

Runs both the React and Electron development servers in parallel using `npm-run-all`.

#### `dev:react`

```bash
npm run dev:react
```

Starts the Vite development server with Hot Module Replacement (HMR) for React.

#### `dev:electron`

```bash
npm run dev:electron
```

Transpiles the Electron code and launches the Electron app in development mode.

---

### 🏗️ Build

#### `build`

```bash
npm run build
```

Cleans TypeScript build info and builds the React app using Vite.

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

> These use [`electron-builder`](https://www.electron.build/) for bundling and packaging.

## 📚 Technologies Used

- **React 19**
- **Electron 36**
- **TypeScript**
- **Vite 6**
- **ESLint**
- **electron-builder**
- **npm-run-all**
- **cross-env**

---

## 📝 Final Notes

This starter template helps you kickstart modern desktop app development using a clean, modular structure. It supports fast iteration in development and simple packaging for distribution across all major platforms.

---
