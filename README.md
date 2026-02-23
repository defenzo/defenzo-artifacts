<div align="center">
  <img src="logo.png" alt="Defenzo Logo" width="120" />
  <h1>Defenzo Artifacts</h1>
  <p>Official Distribution Channel for the Defenzo Security Brain</p>
  <br />
</div>

---

### Overview
This repository serves as the public infrastructure for Defenzo binary distribution. It hosts compiled assets for the Defenzo CLI engine, enabling zero-initiative onboarding for the VS Code extension and MCP ecosystem.

### Distribution Matrix

| Platform | Architecture | Format | Stability |
| :--- | :--- | :--- | :--- |
| **macOS** | Apple Silicon (arm64) | `.tar.gz` | Stable / Beta |
| **macOS** | Intel (amd64) | `.tar.gz` | Stable / Beta |
| **Linux** | x86_64 (amd64) | `.tar.gz` | Stable / Beta |
| **Linux** | ARM64 | `.tar.gz` | Stable / Beta |
| **Windows**| x64 | `.zip` | Stable / Beta |

---

### Release Channels

#### 1. Stable (Standard)
The default channel for production environments. These binaries have passed full regression testing and security audits. 
*   **Source**: [Stable Releases](https://github.com/defenzo/defenzo-artifacts/releases)
*   **VS Code**: Default behavior

#### 2. Beta (Edge)
Experimental builds generated automatically from the [main](cci:1://file:///Users/admin/Projects/defenzo/backend/cmd/api/main.go:22:0-96:1) branch. These contain the latest security heuristics and LLM triage optimizations.
*   **Source**: [latest-beta](https://github.com/defenzo/defenzo-artifacts/releases/tag/latest-beta)
*   **Activation**: Set `"defenzo.betaChannel": true` in VS Code settings.

---

### Integrity Verification
To ensure the authenticity of the downloaded binaries, a `checksums.txt` file (SHA-256) is provided with every release. 

```bash
# Verify integrity on Linux/macOS
sha256sum --check checksums.txt
