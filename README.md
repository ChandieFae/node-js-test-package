# 🧪 @chandiefae/test-cli

This is a test Node.js package designed to demonstrate:

- GitHub Packages publishing
- A simple CLI interface using Node.js
- GitHub Actions automation

---

## 📦 Usage

### 📥 Install (after publishing)

```bash
npm install -g @chandiefae/test-cli
💻 Run the CLI
bash
Copy
Edit
test-cli
You should see:

bash
Copy
Edit
🧶 Welcome to the test CLI from @chandiefae/test-cli!
🛠 CLI Script
This package exposes a CLI command via the bin field in package.json:

📁 cli.js
js
Copy
Edit
#!/usr/bin/env node

console.log("🧶 Welcome to the test CLI from @chandiefae/test-cli!");
Make sure it's executable:

bash
Copy
Edit
chmod +x cli.js
📄 package.json Highlights
json
Copy
Edit
{
  "name": "@chandiefae/test-cli",
  "version": "1.0.0",
  "bin": {
    "test-cli": "./cli.js"
  },
  "scripts": {
    "test": "echo '✅ CLI test passed!'"
  },
  "publishConfig": {
    "registry": "https://npm.pkg.github.com/"
  }
}
