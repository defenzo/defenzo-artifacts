# 🧠 Defenzo Security Brain: Artifacts

This repository is the official distribution channel for **Defenzo CLI** binaries and release assets. 

> **Note**: This is a distribution-only repository. The core engine source code remains private and secure within the primary Defenzo organization.

## 🚀 Installation

### 1. VS Code Extension (Recommended)
The easiest way to install and manage Defenzo is via the [Official VS Code Extension](https://marketplace.visualstudio.com/items?itemName=defenzo.defenzo). It handles automatic updates, binary verification, and MCP integration for Claude Desktop.

### 2. Direct Download
You can download the latest binaries directly from the [Releases](https://github.com/defenzo/defenzo-artifacts/releases) page for your specific platform:

*   **macOS**: `darwin-amd64` (Intel) or `darwin-arm64` (Apple Silicon)
*   **Linux**: `linux-amd64` or `linux-arm64`
*   **Windows**: `windows-amd64.zip`

## 🧪 Release Channels

### 🟢 Stable Channel
Official production-ready releases. These have undergone full security validation and are recommended for most users.

### 🟡 Beta Channel
Experimental builds from the [main](cci:1://file:///Users/admin/Projects/defenzo/backend/cmd/api/main.go:22:0-96:1) branch. These include the newest security patterns and experimental AI triage features. Enable this in the VS Code settings via `defenzo.betaChannel`.

## 🛡️ Security & Verification
All artifacts are packaged with a `checksums.txt` file. To verify the integrity of your download:

```bash
sha256sum --check checksums.txt
