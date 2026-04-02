# BPSA - Beyond Python SmolAgents

![How to Install BPSA](https://github.com/joaopauloschuler/beyond-python-smolagents/blob/master/docs/img/BPSA-HowToInstall.gif?raw=true)

**BPSA - Beyond Python SmolAgents** is a fork of the original [smolagents](https://github.com/huggingface/smolagents) that extends its original abilities:
* 💻 **Interactive CLI ([`bpsa`](https://github.com/joaopauloschuler/beyond-python-smolagents/blob/master/README.md#cli-bpsa)):** Multi-turn REPL with slash commands, command history, tab completion, session stats, and auto-approve mode.
* 🔄 **Infinite runtime CLI ([`ad-infinitum`](https://github.com/joaopauloschuler/beyond-python-smolagents/blob/master/README.md#cli-ad-infinitum)):** Allows agents to **run ad infinitum** via autonomous looping.
* 🗜️ **Context compression**: Biologically inspired [automatic LLM-based summarization](https://github.com/joaopauloschuler/beyond-python-smolagents/blob/master/docs/compression.md) of older memory steps to manage context window size during long-running tasks.
* 🌐 **Browser integration:** Control a headed Chromium browser from agent code blocks via Playwright (`--browser` flag).
* 🖥️ **GUI interaction:** Launch, screenshot, click, type, and send keys to native GUI applications on X11 via xdotool/ImageMagick (`--gui-x11` flag).
* 🔌 **MCP server integration:** Connect any [Model Context Protocol](https://modelcontextprotocol.io) server as a tool source via the `--mcp` CLI flag. Supports both HTTP (Streamable HTTP) and stdio-based servers.
* 👁️ **Image loading:** Agents can load and visually inspect image files (plots, screenshots, diagrams) via the built-in `load_image` tool — always available, no flags needed.
* 🎨 **Image tools:** Visual image diffing (`diff_images`), OCR text extraction from images (`screen_ocr`), and a canvas for drawing shapes, text, and annotations (`canvas_create`, `canvas_draw`) — always available.
* 🎤 **Dictation input:** Dictate prompts via microphone using Whisper or ElevenLabs transcription (`/dictation` command, requires `BPSA_DICTATION_TRANSCRIBER` env var).
* ⚡ **Native Python execution:** Execute Python code natively via `exec` for unrestricted processing.
* 🌍 **Multi-language support:** Code in multiple languages beyond Python (Pascal, PHP, C++, Java and more).
* 🛠️ **Developer tools:** Lots of new tools that help agents to compile, test, and debug source code in various computing languages.
* 👥 **Multi-agent collaboration:** Collaborate across multiple agents to solve complex problems.
* 🔍 **Research tools:** Tools that help agents to research and write technical documentation.
* 📚 **Documentation generation:** Generate and update documentation including READMEs for existing codebases.


## Installation
Install the project, including the dictation support, CLIs, OpenAI protocol and LiteLLM dependencies.

```bash
$ pip install bpsa[dictation,browser,openai,litellm]
```

Find out more at [BPSA](https://github.com/joaopauloschuler/beyond-python-smolagents/) repository.

This will set up the necessary libraries and the Beyond Python Smolagents framework in your environment.
