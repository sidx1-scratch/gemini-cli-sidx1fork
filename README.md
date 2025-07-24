# Gemini CLI

[![Gemini CLI CI](https://github.com/sidx1-scratch/gemini-cli-sidx1fork/actions/workflows/ci.yml/badge.svg)](https://github.com/sidx1-scratch/gemini-cli-sidx1fork/actions/workflows/ci.yml)

![Gemini CLI Screenshot](./docs/assets/gemini-screenshot.png)

This repo is for the sidx1chat CLI — a command-line AI tool that hooks into your tools, understands your code, and speeds up your workflow.

With the sidx1chat CLI, you can:

- Query and edit huge codebases beyond Gemini’s 1M token context window.
- Generate new apps from PDFs or sketches using Gemini's multimodal power.
- Automate boring stuff like pull requests or tricky rebases.
- Hook up to MCP servers and tools for extra power, like [media generation with Imagen, Veo, or Lyria](https://github.com/GoogleCloudPlatform/vertex-ai-creative-studio/tree/main/experiments/mcp-genmedia)
- Ground your queries with built-in [Google Search](https://ai.google.dev/gemini-api/docs/grounding).

## Quickstart

### Old way (legacy install)

1. Clone the repo:
   ```bash
   git clone https://github.com/sidx1-scratch/gemini-cli-sidx1fork.git
   cd gemini-cli-sidx1fork
Install dependencies and build:

bash
Copy
Edit
npm install
npm run build
Link the CLI globally:

bash
Copy
Edit
npm link
Run it:

bash
Copy
Edit
gemini
Login with your Google account when prompted.

New way (just install the package)
bash
Copy
Edit
npm install -g gemini-cli-sidx1fork
Then just run:

bash
Copy
Edit
gemini
Sign in when asked. Done. No hassle.

Using a Gemini API Key
Want more control or higher rate limits? Get a key from Google AI Studio and set it:

bash
Copy
Edit
export GEMINI_API_KEY="YOUR_API_KEY"
(Windows PowerShell: $env:GEMINI_API_KEY="YOUR_API_KEY")

Examples
Start fresh:

bash
Copy
Edit
mkdir new-project
cd new-project
gemini
> Write me a Gemini Discord bot that answers questions using a FAQ.md file I will provide
Or use it on an existing repo:

bash
Copy
Edit
git clone https://github.com/sidx1-scratch/gemini-cli-sidx1fork.git
cd gemini-cli-sidx1fork
gemini
> Summarize all the changes made yesterday
Troubleshooting
If you hit problems, check Troubleshooting Guide.

Popular tasks
Explore a codebase:

kotlin
Copy
Edit
> Describe the main parts of this system’s architecture.
Work on code:

less
Copy
Edit
> Draft a fix for GitHub issue #123.
Automate stuff:

shell
Copy
Edit
> Generate a slide deck of last week’s git history by feature and member.
Manage files:

pgsql
Copy
Edit
> Convert all images here to PNG and rename them using EXIF dates.
Uninstall
See Uninstall Instructions.
