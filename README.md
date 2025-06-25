# VirtualBar – ChatGPT-Powered Bartender Simulation in Unity
A proof-of-concept game that brings generative AI into a 3D bar scene.  
Walk up to **Shreyi**, the bartender NPC, type (or speak) a question, and get a real-time response from OpenAI’s GPT-4o-mini model. The project shows how modern AI can replace rigid dialogue trees with unscripted, context-aware conversations.

---

## Key Features
| Feature | Description |
|---------|-------------|
| **Real-time AI dialogue** | Player messages are streamed to the ChatGPT API; replies are displayed bubble-by-bubble while the bartender “talks.” |
| **Immersive bar environment** | Ready Player Me avatars, Mixamo animations, URP lighting, ambient patrons and music. |
| **Seamless state switch** | Proximity trigger opens the chat UI, locks player controls, and plays a talking animation. Closing the UI instantly returns gameplay control. |
| **Prompt-engineered persona** | System prompt keeps Shreyi “in character”—friendly, helpful, never breaking the fourth wall. |
| **Extensible architecture** | Decoupled scripts for AI calls, UI, and gameplay make it easy to add more AI NPCs or migrate to local models later. |

---

## Demo
*(Short GIF or video link here, if you have one)*

---

##  Tech Stack
| Area | Tool / Package |
|------|----------------|
| Game engine | **Unity 2021.3 LTS** (URP) |
| Player controller | Unity **Starter Assets** (Third-Person) |
| Camera | **Cinemachine** FreeLook |
| Characters | **Ready Player Me** avatars + **Mixamo** animations |
| AI backend | **OpenAI ChatGPT** (GPT-4o-mini) |
| Networking | `UnityWebRequest` + async/await |
| Version control | **Git LFS** for large assets |

---

##  Quick Start

> **Prerequisites**
> * Unity 2021.3 LTS (or newer)  
> * Git + Git LFS  
> * An OpenAI API key with Chat Completions access

```bash
# 1  Clone (with LFS) 
git lfs install          # one-time Git LFS setup
git clone https://github.com/09gauravsingh/ChatGPT_Unity_Integration.git
cd ChatGPT_Unity_Integration

# 2  Open the project in Unity Hub
#    → Scenes/BarScene.unity

