<div align="center">

# AMIT × JACE

### Building a real-world personal AI system, one subsystem at a time.

**AI · Computer Vision · Spatial Interfaces · Automation · Hardware**

*Inspired by the idea behind Tony Stark's lab: technology that understands the room, responds naturally, remembers context, and turns intent into action.*

[![GitHub](https://img.shields.io/badge/GitHub-amitwjace--creator-181717?style=for-the-badge&logo=github)](https://github.com/amitwjace-creator)
[![JACE](https://img.shields.io/badge/PROJECT-JACE-00AEEF?style=for-the-badge)](https://github.com/amitwjace-creator/JACE)

</div>

---

## JACE

> **A modular, real-world AI system — not just a chatbot.**

JACE is my long-term attempt to build the kind of computing environment that made Tony Stark's workshop so compelling: voice, vision, memory, spatial interaction, automation and hardware behaving like parts of one system.

The goal is not to recreate a movie prop. It is to take that interaction philosophy and see how much of it can be built with real hardware and software.

```text
                         ┌──────────────┐
                         │     JACE     │
                         │ intelligence │
                         └──────┬───────┘
                                │
        ┌───────────────┬───────┼───────┬───────────────┐
        ▼               ▼       ▼       ▼               ▼
     PERCEPTION        VOICE   MEMORY  SPATIAL        AUTOMATION
   cameras + CV       speech   context  gestures      room + tools
        │               │       │       │               │
        └───────────────┴───────┼───────┴───────────────┘
                                ▼
                         REAL-WORLD ACTION
```

### The system I am working toward

| System | Direction |
| :--- | :--- |
| 👁️ **Perception** | Cameras, object detection, people, presence and scene understanding |
| 🎙️ **Voice** | Wake word, speech recognition, reasoning and natural responses |
| 🧠 **Memory** | Searchable long-term context, vector retrieval and Obsidian |
| 🖐️ **Spatial control** | Hand tracking, pointing, pinch, drag, swipe and two-hand interaction |
| 🏠 **Smart room** | Presence-aware devices, routines and physical-world automation |
| 📽️ **Interface** | A projected, spatial JARVIS-style workspace |
| ⌚ **Wearable** | A future always-available endpoint and memory capture layer |
| 🔌 **Integrations** | Connecting JACE to the software and services around me |

---

## What exists today

### 🖐️ Spatial Gesture Lab

This is the most developed physical-interface part of JACE so far.

The current prototypes use **OpenCV + MediaPipe** for real-time hand tracking and support pointing, pinch, drag, swipe, point-hold context and two-hand transformations.

Current tuned target:

```text
CAM      29–30 FPS
AI       27–30 FPS
UI       58–61 FPS
LATENCY  ~45–65 ms result age
```

I am also experimenting with **OpenVINO** optimization and a precision-focused Object Pointer prototype.

[![Explore barehands](https://img.shields.io/badge/EXPLORE-barehands-111827?style=for-the-badge&logo=github)](https://github.com/amitwjace-creator/barehands)

### 🤖 Agent infrastructure

If autonomous agents are doing useful work, I want to know what they are doing without babysitting terminals.

**codex-session-monitor** explores that layer: monitoring sessions, surfacing state, usage and completion, and making background agent work visible.

[![View codex-session-monitor](https://img.shields.io/badge/VIEW-codex--session--monitor-111827?style=for-the-badge&logo=github)](https://github.com/amitwjace-creator/codex-session-monitor)

---

## The lab

JACE is being built as a physical system as much as a software project.

The long-term picture is a room where cameras provide perception, microphones provide voice input, local machines run services, displays/projectors provide spatial feedback, and custom electronics become physical endpoints.

```text
            CAMERA ─────────────┐
            MICROPHONES ────────┤
            WEARABLE ───────────┤
                                ▼
                         ┌─────────────┐
                         │    JACE     │
                         │ local brain │
                         └──────┬──────┘
                                │
             ┌──────────────────┼──────────────────┐
             ▼                  ▼                  ▼
        PROJECTED UI       SMART ROOM         COMPUTERS
        + gestures         + devices          + agents
```

### From inspiration → workshop → system

I am documenting the build as it develops: the room, server setup, electronics, prototypes, failures, redesigns and the moments where something that felt like science fiction starts working on a real desk.

> **This section is intentionally ready for original workshop/progress photography.**
> Personal room photos will be added here rather than using images I do not own.

---

## Build log

JACE is not a finished product. That is the point.

```text
IDEA
  ↓
rough prototype
  ↓
make it work
  ↓
measure what is bad
  ↓
rebuild it
  ↓
connect it to JACE
  ↓
repeat
```

### Current direction

- [x] Establish the JACE repository and architecture
- [x] Recover and organize the gesture-control prototypes
- [x] Build a tuned real-time Gesture Lab
- [x] Build the Object Pointer precision prototype
- [x] Start OpenVINO optimization work
- [ ] Reliable always-on voice interface
- [ ] Long-term memory + Obsidian/vector retrieval
- [ ] Perception pipeline for the room
- [ ] Smart-room control layer
- [ ] Projected spatial interface
- [ ] Wearable JACE endpoint
- [ ] Connect the subsystems into one continuous experience

---

## How I think about building

I am interested in the point where **AI stops being a tab in a browser and becomes infrastructure around you**.

I like projects where software has to interact with messy reality: cameras, latency, microphones, local machines, physical spaces, human gestures and imperfect hardware.

My loop is simple:

**build → use → notice friction → measure → improve → connect**

I would rather have an imperfect prototype running in my room than a perfect idea sitting in a document.

---

## Tools & technologies

<p align="center">
<img src="https://skillicons.dev/icons?i=python,js,nodejs,git,github,windows,linux,vscode&perline=8" alt="Tools and technologies" />
</p>

**Currently exploring:** computer vision · MediaPipe · OpenCV · OpenVINO · AI agents · local-first systems · vector search · automation · spatial interfaces · embedded hardware

---

## Beyond JACE

I also experiment with agent workflows and small tools that remove friction from how I build.

The common thread is **leverage**: giving one person better ways to see, think, build and control complex systems.

### Public projects

| Project | What it explores |
| :--- | :--- |
| **[barehands](https://github.com/amitwjace-creator/barehands)** | Camera-based gesture and spatial interaction |
| **[codex-session-monitor](https://github.com/amitwjace-creator/codex-session-monitor)** | Visibility and monitoring for coding-agent sessions |

*The main JACE repository is private because the project has a strict boundary between public code and personal data.*

---

## Principles

```text
01  Build things I genuinely want to use.
02  Prototype before over-planning.
03  Measure latency, reliability and real-world behavior.
04  Keep personal data local and private by default.
05  Make each subsystem useful on its own.
06  Then connect the pieces.
07  Keep shipping the progress, not just the final result.
```

---

## Connect

I am interested in meeting people working on **AI agents, computer vision, HCI, spatial computing, robotics, embedded systems, local AI and unusual human-computer interfaces**.

If you are building something in that world, exploring similar ideas, or think two projects should collide, I would like to hear about it.

[![Instagram](https://img.shields.io/badge/Instagram-@amitbenshachar-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/amitbenshachar/)
[![GitHub](https://img.shields.io/badge/GitHub-@amitwjace--creator-181717?style=for-the-badge&logo=github)](https://github.com/amitwjace-creator)

**Instagram:** [@amitbenshachar](https://www.instagram.com/amitbenshachar/) · **GitHub:** [@amitwjace-creator](https://github.com/amitwjace-creator)

---

<div align="center">

### *“Build the interface you wish existed.”*

**JACE is the long game. This profile is the build log.**

</div>
