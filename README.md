# React + TypeScript + Vite + Tailwind

This template provides a minimal setup to get Electron and React working in Vite with HMR and some ESLint rules with Tailwind styling.

### `Failed to connect to the bus` Error fix

1️⃣ Start DBus Manually (For WSL or Headless Linux)
Run this command before launching Electron:

```bash
export $(dbus-launch)
```

Then try running your app again:

```bash
yarn dev
```

If this works, add it to your shell profile (~/.bashrc or ~/.zshrc):

```bash
echo 'export $(dbus-launch)' >> ~/.bashrc
source ~/.bashrc
```
