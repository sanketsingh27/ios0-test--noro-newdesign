# Blank Native iOS App

This folder contains a minimal SwiftUI-based iOS app scaffold:

- `Sources/App.swift` – app entrypoint
- `Sources/ContentView.swift` – starter empty screen
- `Info.plist` – app metadata
- `Assets.xcassets/` – app icon and accent color asset folders

To run:

1. Open Xcode and create a new iOS app target.
2. Replace the generated `App` source files with these files or copy this folder into a new project.
3. Build and run on an iOS simulator.

## MobAI + Builder one-shot path

From your local machine (with Xcode + GitHub access):

1. Install builder:

```bash
curl -sSL https://raw.githubusercontent.com/MobAI-App/ios-builder/main/install.sh | bash
```

2. Ensure your repo has a GitHub `origin` remote and push this project.
3. Run in this repo:

```bash
PATH=$HOME/.local/bin:$PATH
builder init
builder ios build --unsigned
```

4. In MobAI, open API server at `http://localhost:8686`, install the IPA from `dist/`, then launch it on your device/simulator.
