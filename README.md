# Jarvis OS

Available on PyPI: [https://pypi.org/project/jarvis-os/](https://pypi.org/project/jarvis-os/)

Jarvis OS is a voice assistant designed to streamline and automate anything from daily tasks to advanced development workflows. It integrates offline speech recognition, AI-powered natural language responses, and system-level command execution. It can also function as a voice-powered command-line interface, capable of organizing, accessing, and manipulating files, as well as executing bash commands. Jarvis supports optional local customization through LM Studio.

---

## Features

* Offline speech recognition with Vosk
* Natural voice synthesis using Yapper TTS
* Streaming responses from local or online LLMs

  * Online default: Gemini 1.5 Flash
  * Local default: LLaMA 3.2 (1B parameters) via LM Studio
  * Customize the local model by editing the LLM endpoint URL in `main.py`
* Retrieval-Augmented Generation (RAG) system for web-enhanced queries
* Terminal-based interface with boot animations and dynamic loading screens
* System-level command execution, such as:

  * Opening applications
  * Performing web searches
  * Managing files
  * Shutting down system

### Example Commands

```text
Jarvis open vscode
Jarvis google how to bake sourdough
Jarvis shutdown
Jarvis explain quantum entanglement
Jarvis delete the read me file
```

---

## Recommended Setup Before Installation

It is recommended to install and run Jarvis OS inside a Python virtual environment:

```bash
python -m venv jarvis-env
```

### Activate Environment

* **Windows**

  ```bash
  jarvis-env\Scripts\activate
  ```
* **Mac/Linux (POSIX)**

  ```bash
  source jarvis-env/bin/activate
  ```

---

## Installation

```bash
pip install jarvis-os
```

---

## Configuration

* Python version 3.8 or higher is required
* Ensure microphone input is enabled on your system
* To connect to an LLM backend (e.g., LM Studio), modify the API endpoint in `main.py`

---

## Additional Notes

* This package was initially built for Windows systems
* POSIX (Linux/Mac) support is partial and in progress

---

## License

This project is licensed under the Apache License 2.0. See the `LICENSE` file for details.

---

## Author

**Arvin Adeli**
