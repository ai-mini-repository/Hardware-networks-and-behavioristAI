# The Chronicles of Lab 404: Hardware, Networks & Behaviorist AI — Stage 2 Markdown V2.0

> **Team:** Whoisosy
> **Module:** Hardware, Networks, and Behaviorist AI
> **Snapshot date:** 7 November 2026
> **Latest commit:** b7143fa 
> **Repository:** https://github.com/ai-mini-repository/Hardware-networks-and-behavioristAI

## Team members

| Member | GitHub username |
|---|---|
| Sat Aruzhan | Sataruzhan |
| Richie Maynard 蔡宗震 | richie-maynard |
| Weizel Aurelius | weizelaurelius |
| Seitenaly Akerke | akerkeseyt |
| Raul Mammadzada | verrby |
| Atantayev Sultan | Sultan456-oss |
| Pernebay Akhmet | ahmetpernebai |

## Project purpose

This repository is the shared Markdown source for our team's learning resources on computer hardware, computer networks and behaviorist AI. The content here is used to produce three Stage 2 resources:

- the **Study Guide and Test Bank** — *The Chronicles of Lab 404*,
- the **PPT Slides**, and
- the **Video Tutorials** (one per part: Hardware, Networks, Behaviorist AI).

When an error is found in any resource, we correct it here first and then update every affected resource.

## Intended learners

Beginners with basic computer literacy who can use a computer and a web browser. No prior experience with hardware assembly, network configuration, programming or AI is assumed.

## What changed since Stage 1 (V1.0 → V2.0)

- **Stage 1** contained the module outline and one developed topic (*How data travels from your computer to a website*).
- **V2.0** develops all core topics into **eight full modules** (Topics 1–21). Each module has learning objectives, explanations, worked examples, diagrams, activities with answers, a summary, a glossary and references.
- Superseded drafts were removed, so each topic has one source version.

## Where to find the materials

The core learning content is in `content/The Chronicles of Lab 404: Hardware, Networks & Behaviorist AI/`, in study-guide order.

| Part | File | Topics |
|---|---|---|
| **A — Hardware** | `Module_01_Number_Systems_and_Digital_Data_Representation.md` | Number systems; digital data representation |
| | `Module_02_Core_Computer_Components_and_Memory_Hierarchy.md` | 3 Core components & Von Neumann model · 4 RAM vs. storage & memory hierarchy |
| | `Module_03_System_Startup_and_Application_Execution.md` | 5 From power-on to sign-in · 6 From program file to running process |
| | `Module_04_System_Buses_Interrupts_DMA_and_Hardware_Labs.md` | 7 System buses, interrupts and DMA · 8 Hardware labs |
| **B — Networks** | `Module_05_Network_Fundamentals_Devices_and_Protocols.md` | 9 Network fundamentals and types · 10 Devices and transmission media · 11 Addresses and protocols |
| | `Module_06_Web_Journey_Firewalls_and_Network_Labs.md` | 12 How data travels to a website · 13 Firewalls · 14 Safe troubleshooting · 15 Network labs |
| **C — Behaviorist AI** | `Module_07_Behaviorist_AI_MDP_and_Q_Learning.md` | 16 What is behaviorist AI? · 17 Agent–environment loop & MDPs · 18 Learning from rewards (Q-learning) |
| | `Module_08_Reward_Design_Rule_Based_Learning_Agents_and_AI_Myths.md` | 19 Reward design & reward hacking · 20 Rule-based vs. learning agents · 21 Applications, limitations & myths |

Other files:

- `content/module-outline.md` — the original module outline, learning outcomes and scope (Stage 1).
- `content/*.md` (standalone topic files) — earlier topic drafts. Their content has been developed into the modules above, and they are kept for traceability.
- `BH 4, Why must a learning agent sometimes try an action that looks worse?.md` — supporting note on exploration vs. exploitation (Module 07).
- `Remarks about AI made during research.md` — record of AI responses used during research.
- `asset/` — supporting assets.

## Folder structure

```text
.
├── README.md
├── BH 4, Why must a learning agent sometimes try an action that looks worse?.md
├── Remarks about AI made during research.md
├── asset/
│   └── modem
└── content/
    ├── The Chronicles of Lab 404: Hardware, Networks & Behaviorist AI/
    │   ├── Module_01_Number_Systems_and_Digital_Data_Representation.md
    │   ├── Module_02_Core_Computer_Components_and_Memory_Hierarchy.md
    │   ├── Module_03_System_Startup_and_Application_Execution.md
    │   ├── Module_04_System_Buses_Interrupts_DMA_and_Hardware_Labs.md
    │   ├── Module_05_Network_Fundamentals_Devices_and_Protocols.md
    │   ├── Module_06_Web_Journey_Firewalls_and_Network_Labs.md
    │   ├── Module_07_Behaviorist_AI_MDP_and_Q_Learning.md
    │   └── Module_08_Reward_Design_Rule_Based_Learning_Agents_and_AI_Myths.md
    ├── module-outline.md
    ├── addresses-and-protocols.md
    ├── application-launch-professional.md
    ├── computer-startup.md
    ├── core-components.md
    ├── how-an-ai-agent-learns.md
    ├── how-data-travels.md
    ├── how-devices-communicate-on-a-local.md
    ├── how-firewalls-control-network-traffic.md
    ├── information check.md
    ├── learning-from-rewards-and-penalties.md
    ├── network-fundamentals.md
    ├── network-hardware-explained.md
    ├── ram-vs-storage.md
    ├── reward-design.md
    └── safety-and-troubleshooting.md
```

## Content status

**Status key:** `Drafted` = substantive content exists · `Needs review` = a member other than the author must check it · `Checked` = reviewed, with the outcome recorded in the Stage 2 logs.

| Module | Status | Reviewer (non-author) | Notes |
|---|---|---|---|
| 01 Number Systems & Data | Drafted — needs review | *(add name)* | |
| 02 Components & Memory | Drafted — needs review | *(add name)* | |
| 03 Startup & App Execution | Drafted — needs review | *(add name)* | |
| 04 Buses, Interrupts, DMA | Drafted — needs review | *(add name)* | Knowledge Check needs an answer key |
| 05 Network Fundamentals | Drafted — needs review | *(add name)* | Knowledge Check needs an answer key |
| 06 Web Journey & Firewalls | Drafted — needs review | *(add name)* | No local images; one diagram fix (see task list) |
| 07 Behaviorist AI & Q-Learning | Drafted — needs review | *(add name)* | |
| 08 Reward Design & AI Myths | Drafted — needs review | *(add name)* | |

Change a row to `Checked` only after the review has actually been done and recorded.

## Task list

- [x] Develop all core topics into Modules 01–08
- [x] Remove superseded drafts and fix the misspelled filename
- [x] Export the readable PDF copy of the V2.0 content
- [ ] Peer-review each module (reviewer ≠ author) and record the results in the Stage 2 logs
- [ ] Learner-test at least one explanation or activity and record what changed
- [ ] Download hotlinked images into `asset/` and switch to local paths, so they display offline and in the PDF
- [ ] Add answer keys to the Knowledge Checks in Modules 04 and 05
- [ ] Module 06: in the stateful-firewall sequence diagram, change `No matching state; evaluate inbound policy` to use a comma — the semicolon stops the diagram from rendering
- [ ] Merge or archive the older standalone files in `content/` so they cannot conflict with the modules
- [ ] Use descriptive commit messages instead of "Add files via upload"

## How to view the content

- **On GitHub:** open any module file. GitHub renders the Mermaid diagrams and the expandable answer blocks.
- **Offline:** use the readable PDF in the submission package. Images that are still hotlinked show as labelled figure boxes until they are moved into `asset/`.

## AI use and academic integrity

We used AI tools (ChatGPT, Gemini and Claude) during research and preparation. Significant AI assistance, how we verified it, and the decisions we made are recorded in the Stage 2 project and personal logs, beside or below the relevant entries. All team members are responsible for fact-checking the content and being able to explain it. Reviews and contributions are recorded only once they have actually happened.
