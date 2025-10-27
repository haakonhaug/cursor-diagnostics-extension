# Cursor Diagnostics Bridge - VS Code Extension

A VSCode-Compatible extension that exposes real-time IDE diagnostics (errors, warnings, and info) to Claude Code via Unix socket/named pipe.

## 📦 Installation

Download the latest `.vsix` file from this repository and install it using one of these methods:

### Method 1: Command Line

```bash
# For VS Code
code --install-extension cursor-diagnostics-bridge-x.x.x.vsix

# For Cursor
cursor --install-extension cursor-diagnostics-bridge-x.x.x.vsix

# For other IDEs (Codium, VSCodium, etc.)
<your-ide> --install-extension cursor-diagnostics-bridge-x.x.x.vsix
```

### Method 2: Drag and Drop

Simply drag the `.vsix` file and drop it into the Extensions panel in your IDE.

### Method 3: Command Palette

1. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
2. Type **"Extensions: Install from VSIX..."**
3. Select the `cursor-diagnostics-bridge-x.x.x.vsix` file
4. Reload when prompted

## 🚀 Usage

Once installed, the extension automatically starts a WebSocket server via Unix socket (macOS/Linux) or named pipe (Windows) and exposes diagnostics to MCP servers.

Look for `$(pulse) Diagnostics Bridge` in your status bar to confirm it's running.

## 🤝 Works With

Pairs with **[cursor-diagnostics-mcp](https://www.npmjs.com/package/cursor-diagnostics-mcp)** for Claude Code integration.

## 📄 License

MIT
