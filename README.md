# Prompt-injection-detector- 

# 🛡️ Prompt Injection Detector

A lightweight and visual tool that detects possible **Prompt Injection attacks** in user input, protecting LLM-powered apps from malicious prompt overrides.

---

## 🚀 Demo

Here’s how the UI works:

<table>
  <tr>
    <td><img src="screenshots/safe_input.png" alt="Safe input" width="100%"/></td>
    <td><img src="screenshots/injection_detected.png" alt="Injection warning" width="100%"/></td>
  </tr>
</table>

---

## 📌 What is Prompt Injection?

Prompt injection is a form of attack where a user manipulates an AI model by injecting hidden instructions into a prompt. This can override system prompts, expose data, or lead the model to behave in unintended ways.

It’s similar to how **SQL injection** works for databases — but here, the attack vector targets natural language instructions in LLMs (Large Language Models).

---

## 🧠 Motivation

While exploring LLM security, I realized that **Prompt Injection** is one of the most under-discussed yet dangerous vulnerabilities in AI systems.

This project aims to:
- Visualize how LLMs may be tricked
- Educate others about safe prompt design
- Offer a basic tool to **flag suspicious user input**

---

## 🛠️ Tech Stack

- **Frontend**: React (or plain HTML/CSS/JS if applicable)
- **Backend**: Python with basic pattern matching
- **Detection Logic**: Heuristic checks for command-like structures

---

## 🧪 How It Works

1. User types input into the interface.
2. The system checks for:
   - Imperative commands (e.g., *“Ignore previous instructions…”*)
   - Modify/replace instructions (e.g., *“Replace the word X with Y”*)
   - Suspicious tokens like `--`, `{}`, or escape characters
3. Returns a visual warning if injection is likely.

---

## 📂 Folder Structure
