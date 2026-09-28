# Sinhala Explainer Teacher (`/sinhala-explainer`)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Antigravity Skill](https://img.shields.io/badge/Antigravity-Skill-blue.svg)](https://github.com/manuja-me/sinhala-explainer)

An intelligent, active pedagogical skill for Google Antigravity and AI coding agents. It explains complex programming, computer science, technical documentation, and study materials in natural, conversational **spoken Sinhala** (කතා කරන සරල සිංහල) while keeping technical English terms intact and making concepts click with visuals and analogies.

---

## 🌟 Key Features

1. **Natural Spoken Sinhala (කතා කරන බස)**: Friendly older-sibling tone addressing the user as **"ඔයා"** without stiff textbook grammar or Singlish.
2. **Technical English Term Preservation**: Standard English technical words (`Variable`, `API`, `Thread`, `Cache`, `Async/Await`) stay in English.
3. **Upfront Glossary ("දැනගන්න ඕන වචන")**: Clarifies uncommon English words before diving into the explanation.
4. **Session Persistence**: Stays active across follow-up turns until explicitly deactivated with commands like `"stop"`, `"normal mode"`, or `"exit"`.
5. **Multi-Modal Intake with Fallbacks**:
   - **Web URLs**: Browses and reads web pages with automatic fallback tips if access is blocked.
   - **PDFs / Documents**: Reads local files or requests direct text copy when needed.
   - **Images & Diagrams**: Interprets screenshots and architecture graphs.
   - **Inline Text / Topics**: Directly explains raw text or provides a disclaimer for topic-only prompts.
6. **Robust Visual Scaffolding**: Uses Mermaid diagrams with **English node labels** (for universal rendering reliability) followed by a **Sinhala caption**.
7. **Clean Code Walkthroughs**: English code blocks that copy-paste and run cleanly, followed by numbered Sinhala line walkthroughs and expected output blocks.
8. **Real-Life Analogies**: Grounds abstract concepts in everyday Sri Lankan scenarios (tea stalls, buses, supermarkets).
9. **Interactive Check-in Challenges**: Concludes with an engaging comprehension question or thought puzzle.

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

### Exit Commands
To return to standard agent behavior at any time:
- `"stop"`
- `"normal mode"`
- `"exit"`
- `"English එකෙන් කියන්න"`
- `"සාමාන්ය විදියට කියන්න"`

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

Copy or clone this directory into your global Antigravity skills location:

```powershell
Copy-Item -Recurse -Path ".\sinhala-explainer" -Destination "$HOME\.gemini\config\skills\sinhala-explainer"
```

Once copied, `/sinhala-explainer` is immediately available in any Antigravity conversation.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
