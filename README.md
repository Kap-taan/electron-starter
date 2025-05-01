# Electron App Starter with React, Node, and TypeScript

This is a starter template to quickly set up an Electron app with React, Node, and TypeScript. The project uses Vite for bundling the React app and Electron for building the desktop application. It includes essential development scripts for building, running, and linting the project.

## Project Setup

To get started, clone the repository and install the dependencies:

```bash
git clone <repository_url>
cd <project_directory>
npm install
```

## Project Structure

The project is organized as follows:
- **src**: Contains the source code for the React application and Electron main process.
- **tsconfig.app.json**: TypeScript configuration for the app.
- **tsconfig.node.json**: TypeScript configuration for the Node and Electron process.

## Scripts

The project includes the following scripts to facilitate development:

### `dev:react`

```bash
"dev:react": "vite"
```
This command runs Vite's development server, which serves the React application in development mode with Hot Module Replacement (HMR). You can access the React app in your browser while Electron handles the desktop window.

To run this, simply use:
```bash
npm run dev:react
```

### `dev:electron`

```bash
"dev:electron": "electron ."
```
This command starts the Electron application in development mode, opening the app in a desktop window. It runs after the React app has been started using `dev:react`.

To run Electron with the React app, use:
```bash
npm run dev:react   # Start React development server
npm run dev:electron   # Launch the Electron app
```

### `build`

```bash
"build": "tsc -b --clean && vite build"
```
This command does the following:
1. `tsc -b --clean`: Compiles TypeScript files for both the app and Electron process.
2. `vite build`: Builds the React application for production using Vite.

To build the app for production, run:
```bash
npm run build
```

### `lint`

```bash
"lint": "eslint ."
```
This command runs ESLint to check your code for any issues and enforce coding standards. It helps keep your code clean and error-free.

To lint the project, run:
```bash
npm run lint
```

### `preview`

```bash
"preview": "vite preview"
```
This command previews the production build of the React app, simulating how the app will behave in production. It is useful to test the final output before packaging the app.

To preview the production build, run:
```bash
npm run preview
```

## Configuring for Your Own Project

You can customize the setup to suit your project's needs by following these steps:

1. **Install additional dependencies**: You can add libraries, such as `react-router` for routing or `redux` for state management, by running:
   ```bash
   npm install <library_name>
   ```

2. **Configure Electron**: Modify the `main.js` file in the Electron directory to adjust how your Electron app behaves. This can include settings for the Electron window, app lifecycle, etc.

3. **Update TypeScript Configurations**: If you need to update TypeScript settings, modify `tsconfig.app.json` and `tsconfig.node.json` as needed.

## Final Notes

This project provides a minimal yet flexible starting point for building an Electron app with React, Node, and TypeScript. The development workflow allows for fast iteration with HMR in React and seamless integration with Electron for building desktop applications.

---