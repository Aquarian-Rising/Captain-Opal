# 🧭 Captain Opal  
> **The decentralized AI command bridge for creators.**  
> Orchestrate multiple AIs — ChatGPT, Gemini, Grok, KimiAI, DeepSeek — through a local “crew” of browser agents led by **Captain Opal’s Number One**, your first officer in cross-AI collaboration.

---

## 🚀 What It Is
Captain Opal is an experimental open-source ecosystem for coordinating multiple LLMs as creative collaborators.  
At its heart is a Chrome MV3 extension nicknamed **Number One**, which listens to structured commands (“OpalLink blocks”) from a controller app — **Captain Opal** — and then:

1. Switches to each AI chat tab (ChatGPT, Gemini, etc.)  
2. Types and submits prompts human-style  
3. Waits for full stable responses  
4. Returns those responses to the Captain Opal coordinator  

💡 *No cloud APIs. No subscriptions. Everything runs locally in your browser.*

---

## 🧩 How It Works
```
[ Captain Opal App ]
        ↓  (OpalLink blocks)
 ┌──────────────────────────────┐
 │  Captain Opal’s Number One   │
 │  ───────────────────────────  │
 │  ⟶ Opens AI tabs             │
 │  ⟶ Sends prompts             │
 │  ⟶ Reads responses           │
 │  ⟶ Relays back               │
 └──────────────────────────────┘
        ↓
[ Responses to Captain Opal ]
```

- **Captain Opal** acts as the command bridge (built with Google Opal Creator or another frontend).  
- **Number One** is the browser-side first officer that executes those commands.  
- Together they form a cooperative multi-AI crew.

---

## 🧠 Why It Matters
Generative projects increasingly span tools and models.  
Captain Opal makes those tools *work together* — coordinating models with complementary strengths (e.g. Grok → humor, ChatGPT → structure, Gemini → research).  
Think of it as a **browser-native LLM orchestra** you can conduct in real time.

---

## ⚙️ Quick Start
1. **Clone or download** the latest [release `.zip`](../../releases).  
2. Open **Chrome → Extensions** → enable *Developer mode* → “Load unpacked.”  
3. **Pin** *Captain Opal’s Number One* for easy access.  
4. Open tabs for each AI you want to coordinate.  
5. Run **`co-sim-regression.html`** to simulate Captain Opal and test interactions.

📘 See detailed setup and QA docs:  
- [`captain-opals-number-one/README.md`](./captain-opals-number-one/README.md)  
- [`captain-opals-number-one/QA_GUIDE.md`](./captain-opals-number-one/QA_GUIDE.md)

---

## 🧪 Current Release — v0.1.1 (Pilot Stable)
- Queue persistence + resume  
- Color-coded overlay (Idle 🟩 Busy 🟨 Error 🟥 Paused ⬜)  
- Config-driven AI handlers  
- Exponential backoff + CSP fallback  
- Built-in regression, stress & soak harnesses  

🔗 [View Release Notes →](../../releases/tag/v0.1.1-pilot-stable)

---

## 🧰 Built With
- **Chrome Extensions MV3**  
- **Vanilla JavaScript (ES Modules)**  
- **Google Opal Creator Integration Ready**  
- **No external dependencies**

---

## 🤝 Contributing
Pull requests, bug reports, and handler patches welcome!  

**To add support for a new AI:**
1. Copy `/handlers/template.js`.  
2. Update selectors + hotkeys.  
3. Test with the built-in regression suite.

---

## 🪩 Roadmap
| Version | Focus | Highlights |
|:--|:--|:--|
| **v0.1.2** | UX polish | Screenshots, demo video, live config reload |
| **v0.2.0** | Full Captain Opal frontend | Opal Creator integration, multi-agent dashboard |
| **v0.3.x** | Peer collaboration | Multiple COs sharing a fleet of NO agents |

---

## 🧾 License
**MIT** — free to use, modify, and remix.  
Credit appreciated: *“Built on the Captain Opal framework.”*

---

## 📣 Acknowledgments
✨ **Grok 4** for pair programming and QA validation  
💡 **Captain Opal (Opal Creator)** for inspiring the multi-AI command bridge  
🛠️ All testers helping refine the Pilot Stable release  

---

### 🧠 Next Up
Captain Opal Coordinator Prompt (“CO Simulator v2”) — full frontend integration via Google Opal Creator.  
Follow updates on [GitHub → Aquarian Rising / Captain-Opal](#)
