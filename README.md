# Gemini CLI - sidx1fork

[![Gemini CLI CI](https://github.com/sidx1-scratch/gemini-cli-sidx1fork/actions/workflows/ci.yml/badge.svg)](https://github.com/sidx1-scratch/gemini-cli-sidx1fork/actions/workflows/ci.yml)

![Gemini CLI Screenshot](./docs/assets/gemini-screenshot.png)

This is my fork of the Gemini CLI. It's a command-line AI that hooks into your tools, understands your code, and (hopefully) makes your life easier.

It lets you:
- Work with codebases bigger than Gemini's 1M token context window.
- Build apps from PDFs or sketches.
- Automate boring stuff like pull requests.
- Connect to MCP servers for more tools.
- Use Google Search to ground your queries so it doesn't just make stuff up.

---

## Installation

### The Right Way (npm)

If you just want to use the tool, this is all you need. Don't overcomplicate it.

```bash
npm install -g gemini-cli-sidx1fork
```

Now run it:

```bash
sidx1chat
```

Sign in with your Google account when it asks. Done.

### For Developers (Manual Build)

Only do this if you plan on messing with the code.

1.  **Clone the repo:**
    ```bash
    git clone https://github.com/sidx1-scratch/gemini-cli-sidx1fork.git
    cd gemini-cli-sidx1fork
    ```
2.  **Install dependencies and build:**
    ```bash
    npm install
    npm run build
    ```
3.  **Link the CLI to your system:**
    ```bash
    npm link
    ```
4.  **Run it:**
    ```bash
    sidx1chat
    ```

---

## Using Your Own API Key

If you have your own Gemini API key from Google AI Studio, you can use it. This gives you more control and higher rate limits.

**On Linux/macOS:**
```bash
export GEMINI_API_KEY="YOUR_API_KEY"
```

**On Windows (PowerShell):**
```powershell
$env:GEMINI_API_KEY="YOUR_API_KEY"
```

---

## What You Can Do

**Start a new project:**
```bash
mkdir my-new-app
cd my-new-app
gemini
> Write me a Discord bot in Python that answers questions from a FAQ.md file.
```

**Work on an existing repo:**
```bash
git clone some-repo
cd some-repo
gemini
> Summarize all the changes made yesterday.
> Draft a fix for GitHub issue #123.
> Convert all JPG images in this directory to PNG.
```

---

## Troubleshooting & Uninstall

- **Problems?** Check the [Troubleshooting Guide](./docs/troubleshooting.md).
- **Want to remove it?** See the [Uninstall Instructions](./docs/uninstall.md).
