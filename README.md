# Sinhala Explainer Teacher (`/sinhala-explainer`)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Antigravity Skill](https://img.shields.io/badge/Antigravity-Skill-blue.svg)](https://github.com/manuja-me/sinhala-explainer)

An intelligent, active pedagogical skill for Google Antigravity and AI coding agents. It explains complex programming, computer science, technical documentation, and study materials in natural, conversational **spoken Sinhala** (කතා කරන සරල සිංහල) while preserving English technical terms and leveraging visual diagrams.

---

## 🌟 Key Features

1. **Natural Spoken Sinhala (කතා කරන බස)**: Explains concepts cleanly without stiff, artificial book Sinhala.
2. **Technical English Term Preservation**: Avoids confusing translations (e.g. keeps `Function`, `Variable`, `Database`, `API`, `Thread`, `Cache`).
3. **Upfront Glossary**: Clarifies uncommon or advanced English words upfront with short, plain definitions.
4. **Multi-Modal Content Intake (Dual Mode)**:
   - **Web URLs**: Browses and digests articles or docs via `read_url_content`.
   - **Files & PDFs**: Reads and explains local PDFs, Markdown docs, and code files.
   - **Images & Diagrams**: Interprets screenshots, architecture graphs, and slides.
   - **Direct Prompts**: Accepts inline text or topics directly.
5. **Visual Scaffolding**: Automatically generates Mermaid flowcharts, sequence diagrams, and markdown tables.
6. **Real-Life Analogies**: Grounds complex concepts in relatable everyday scenarios (e.g. Sri Lankan tea stalls, buses, supermarkets).
7. **Interactive Check-ins**: Concludes with a brief comprehension question or challenge.

---

## 🚀 Usage

Trigger the skill manually in Antigravity chat:

```bash
# Mode 1: With a Web URL
/sinhala-explainer https://docs.docker.com/get-started/

# Mode 2: With a local file or PDF
/sinhala-explainer C:/path/to/lecture-notes.pdf

# Mode 3: With a programming concept or topic
/sinhala-explainer How does Kafka message queue work?

# Mode 4: Interactive mode (no arguments)
/sinhala-explainer
```

---

## 📂 Project Structure

```
sinhala-explainer/
├── SKILL.md                              # Main Antigravity skill definition
├── README.md                             # Project overview and usage
├── LICENSE                               # MIT License
└── references/
    └── examples-and-scenarios.md         # Reference worked examples & scenarios
```

---

## 🛠️ Installation in Antigravity

Clone or copy this folder into your global Antigravity skills directory:

```powershell
# Copy to global Antigravity skills directory
Copy-Item -Recurse -Path ".\sinhala-explainer" -Destination "$HOME\.gemini\config\skills\sinhala-explainer"
```

Once installed, `/sinhala-explainer` is immediately available in any Antigravity conversation.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
