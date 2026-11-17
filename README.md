# PrepFree AI Navigator

> **Ask. Find. Navigate.**  
> An interactive, modern AI-powered navigation assistant designed specifically for the PrepFree student dashboard.

---

## 🚀 Live Demo & Quick Start
Open `index.html` or `AI_Navigation_Assistant_Prototype.html` directly in any web browser, or serve it locally:
```bash
python -m http.server 8085
```
Then visit: `http://localhost:8085`

---

## 📌 Problem & Concept

On the PrepFree student dashboard, the left sidebar displays **icons only without visible text labels** (for a compact, clean look). Because feature names are not visible:
* Students get confused when searching for specific tools like the **ATS Resume Checker**, **Resume Builder**, or **AI Mock Interview**.
* Students often ask questions like: *"Where can I upload my resume?"* without realizing the resume uploader is located inside the ATS Checker.

**PrepFree AI Navigator** bridges this gap by acting as a proactive discovery and transport guide.

---

## 🔄 The 5-Step Interaction Flow

1. **Student Asks a Question:**  
   Click the floating **AI Navigator** button (bottom right) or press `Ctrl + K`. Students can type natural language queries or select one of the quick suggestions:
   - *"I'm not able to find ATS Checker. Can you help me?"*
   - *"Where can I upload my resume?"*
   - *"I want to find jobs suitable for my skills."*
   - *"How do I access the AI Interview feature?"*
   - *"Where can I find my courses and webinars?"*

2. **AI Understands Student Intent:**  
   The assistant parses the query and displays an **Intent Breakdown Card**:
   - **Recognized Intent:** e.g. `Upload resume (PDF/DOCX) to scan ATS compatibility`
   - **Destination:** `ATS Checker`
   - **Navigation Path:** `Dashboard → Left Sidebar (4th icon: Sync 🔄) → ATS Checker`
   - **Confidence Score:** `98% Direct Match`

3. **Text-Based Guidance:**  
   Delivers friendly conversational instructions explaining the exact icon and position on the left rail, followed by two action choices:
   - `Highlight in menu`
   - `Take me to [Feature]`

4. **Visual Guidance ("Highlight in menu"):**  
   - Dims the background backdrop.
   - Highlights the specific icon on the left rail with a glowing animated pulse.
   - Displays a contextual floating tooltip anchored to the icon with its title, purpose, and a `"Take me there"` button.

5. **Guided Navigation ("Take me to [Feature]"):**  
   - Navigates smoothly to the destination feature page.
   - Shows an arrival guidance message explaining available actions.
   - For ATS Checker, displays the drag-and-drop resume upload zone, a sample resume loader (`Rahul_Sharma_FullStack.pdf`), and a live ATS score meter (84% – 89%).
   - **Safe & Consent-Governed:** The assistant only navigates; it never submits applications, uploads files, or alters student data without explicit confirmation.

---

## 🛠️ Tech Stack & Architecture

- **Vanilla HTML5, CSS3 & JavaScript** (Zero external runtime dependencies, 100% self-contained).
- **PrepFree Dark Theme Design:** Custom styling matching the PrepFree student dashboard palette (`#090d12` background, emerald green `#10b981` accents, radial glow cards).
- **Icon-Only Rail System:** SVG icon navigation rail with tooltips, matching the real PrepFree layout.
- **Client-Side Simulation Engine:** Rule-based NLP intent classifier and state management.

---

## 📄 License
MIT License. Created for the PrepFree Student Experience.
