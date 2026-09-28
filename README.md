# Sinhala Explainer Teacher (`/sinhala-explainer`)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Antigravity Skill](https://img.shields.io/badge/Antigravity-Skill-blue.svg)](https://github.com/manuja-me/sinhala-explainer)
[![Security Scanned](https://img.shields.io/badge/SkillSpector-0%2F100%20Safe-brightgreen.svg)](https://github.com/manuja-me/sinhala-explainer)
[![Language: Sinhala](https://img.shields.io/badge/Language-Spoken%20Sinhala-orange.svg)](#)

An intelligent, active pedagogical teacher skill built for **Google Antigravity**, **Claude Code**, and modern AI agent harnesses. 

It explains complex software engineering, computer science, technical documentation, study materials, and general knowledge in natural, warm **spoken Sinhala (Sinhala script)**. It avoids awkward literal translations, preserves industry-standard English technical vocabulary, and anchors learning with real-world analogies and visual diagrams.

---

## 🎯 Why This Skill?

Most AI translations of technical concepts into Sinhala suffer from two major flaws:
1. **Unnatural Book Sinhala (පොත් බස)**: Overly formal, academic phrasing that sounds robotic and difficult to grasp for beginners.
2. **Harmful Jargon Translation**: Translating standardized English terms into invented or obscure Sinhala words (e.g., turning "compiler" into something unintelligible instead of keeping `Compiler`).

`/sinhala-explainer` takes an **older-sibling mentor approach**:
- Speaks casual, patient, everyday Sinhala (addressing you as **"ඔයා"**).
- Preserves technical words in English everywhere.
- Clarifies unfamiliar technical terms upfront before diving into explanations.
- Connects abstract computing concepts to intuitive everyday Sri Lankan analogies.

---

## 🏗️ The 8-Step Pedagogical Anatomy

Whenever new content is provided, the skill delivers a structured explanation:

```text
┌────────────────────────────────────────────────────────┐
│ 1. Goal (One-line learning outcome)                    │
├────────────────────────────────────────────────────────┤
│ 2. දැනගන්න ඕන වචන (Technical Glossary Upfront)         │
├────────────────────────────────────────────────────────┤
│ 3. Everyday Analogy (Relatable Sri Lankan comparison)  │
├────────────────────────────────────────────────────────┤
│ 4. Progressive Sections (Step-by-step knowledge flow)  │
├────────────────────────────────────────────────────────┤
│ 5. Visual Scaffold (English Mermaid flowchart/table)   │
├────────────────────────────────────────────────────────┤
│ 6. Worked Code (Runnable English block + walkthrough)  │
├────────────────────────────────────────────────────────┤
│ 7. Recap (Key takeaway bullet points)                  │
├────────────────────────────────────────────────────────┤
│ 8. Interactive Check-in (Comprehension question)       │
└────────────────────────────────────────────────────────┘
```

---

## 🚀 Usage & Trigger Modes

Invoke the skill directly in your AI coding agent chat:

### 1. Web Link / Documentation
```bash
/sinhala-explainer https://docs.docker.com/get-started/
```
*The agent fetches the web page content, extracts the core architecture, and explains it.*

### 2. Local Files & PDFs
```bash
/sinhala-explainer ./lecture-05-operating-systems.pdf
```
*Reads the target file or PDF and breaks down key technical chapters.*

### 3. Architecture Diagrams & Screenshots
```bash
/sinhala-explainer ./assets/system-architecture.png
```
*Inspects the diagram via vision tools and walks through the data flow step by step.*

### 4. Topic Only (No Source Provided)
```bash
/sinhala-explainer How does Kafka message queue work?
```
*Explains from internal knowledge with a clear transparent disclaimer.*

### 5. Interactive Mode
```bash
/sinhala-explainer
```
*Prompts warmly in spoken Sinhala for what topic, link, or file you want to learn today.*

---

## 🔄 Session Persistence & Exit Controls

- **Active by default across turns**: Once triggered, the skill stays active for subsequent questions so you can dive deeper into follow-up topics without re-typing the command.
- **Lightweight follow-ups**: Simple follow-up queries receive concise, focused answers in the same mentor voice without repeating the heavy glossary boilerplate.
- **Deactivation**: Say any of the following to return to standard assistant mode:
  - `"stop"`
  - `"normal mode"`
  - `"exit"`
  - `"English එකෙන් කියන්න"`
  - `"සාමාන්ය විදියට කියන්න"`

---

## 💡 Worked Demonstration

### Input Prompt
```bash
/sinhala-explainer What is an API?
```

### Response Flow
> **Goal:** මේකෙන් අපි ඉගෙන ගන්නේ Software Programs දෙකක් එකිනෙකා එක්ක කතා කරගන්නේ කොහොමද කියන එක (API).
>
> **දැනගන්න ඕන වචන:**
> - **`API`** (Application Programming Interface): Programs දෙකක් අතර තොරතුරු හුවමාරු කරගන්න හදපු standard communication පාලමක්.
> - **`Endpoint`**: අපි request එකක් යවන විශේෂිත web address එක.
> - **`Payload`**: Request එකක් එක්ක අපි යවන data bundle එක.
>
> **සරල උපමාවකින් තේරුම් ගමු:**
> හිතන්න ඔයා Restaurant එකකට යනවා. Kitchen එක ඇතුළේ කෑම හදන විදිහ ඔයා දන්නේ නැහැ. ඔයා කරන්නේ Menu එක බලලා Waiter ට order එක දෙන එක. Waiter kitchen එකට ගිහින් කෑම එක අරන් ඔයාට ගෙනත් දෙනවා.
> මෙතන **Waiter තමයි API එක!** ඔයා App එක, Kitchen එක තමයි Server එක.
>
> **Diagram එක බලන විදිහ:**
> ```mermaid
> flowchart LR
>     Client["Client (Mobile App)"] -->|Request| API["API Gateway"]
>     API -->|Data Query| Server["Database / Backend"]
>     Server -->|Response| API
>     API -->|JSON Data| Client
> ```
> App එක කෙලින්ම Database එකට යන්නේ නැතුව API එක හරහා ආරක්ෂිතව data ලබාගන්නවා.
>
> **Interactive Check-in:**
> ඔයා Uber app එකෙන් ride එකක් දාද්දී Google Maps පේන්නේ Uber එක ඇතුළෙමනේ. එතනදී Uber එක Google Maps වල API එකක් පාවිච්චි කරනවා කියන එක දැන් ඔයාට තේරෙනවද?

---

## 💻 Installation

### Method A: Global Installation (Recommended)
Install globally across all projects on your machine:

```powershell
# Windows PowerShell (into your skills directory)
git clone https://github.com/manuja-me/sinhala-explainer.git
```

```bash
# macOS / Linux
git clone https://github.com/manuja-me/sinhala-explainer.git
```

### Method B: Workspace Installation
Add the skill to a specific repository or team workspace:

```bash
# Inside your project root
git clone https://github.com/manuja-me/sinhala-explainer.git .agents/skills/sinhala-explainer
```

---

## 🔒 Security & Verification

This skill is audited using [SkillSpector](https://github.com/NVIDIA/skillspector):
- **Risk Score:** `0/100 (SAFE)`
- **Executables:** Zero external binaries or unvetted scripts.
- **Capabilities:** Standard read-only inspection tools (`read_url_content`, `view_file`).

---

## 🤝 Contributing

Contributions, analogies, and pedagogy suggestions are welcome!
1. Fork the repository.
2. Create your feature branch (`git checkout -b feat/new-analogy`).
3. Commit your changes (`git commit -m "feat: add analogies for kubernetes"`).
4. Push to the branch (`git push origin feat/new-analogy`).
5. Open a Pull Request.

---

## 📄 License

Distributed under the [MIT License](LICENSE). Built with ❤️ for Sri Lankan learners and developers.
