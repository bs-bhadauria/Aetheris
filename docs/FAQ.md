# Frequently Asked Questions (FAQ)

### 1. What is Aetheris?
Aetheris is an Extended Reality (XR) spatial computing operating environment engineered specifically for deep scientific and academic research. Instead of treating research papers as flat 2D PDFs or uploading them to disconnected chatbots, Aetheris renders documents in interactive 3D space, tracking reader gaze, pointer coordinates, and voice queries to provide instant, grounded contextual assistance.

---

### 2. How does Aetheris differ from tools like NotebookLM, ChatPDF, or Elicit?
Generic PDF tools suffer from **prompt fatigue**: you have to stop reading, switch tabs, and type elaborate explanations describing which equation or graph you need help with. 
Aetheris utilizes **deictic spatial interaction**: you simply look at an equation and say *"explain this"*. Aetheris instantly resolves the visual referent using sub-100ms gaze raycasting and anchors an interactive 3D spatial note directly beside the equation in world space.

---

### 3. Which hardware devices are supported?
* **Desktop / Laptop Browsers**: Supported via Three.js with full 3D spatial orbit controls, mouse raycasting, and speech recognition.
* **XR Headsets**: Supported on **Meta Quest 3 / Quest 3S / Quest Pro** (via Meta Quest Browser / WebXR) and **Apple Vision Pro** (via Safari Spatial Computing).
* **Upcoming**: Native VisionOS (SwiftUI + RealityKit) and OpenXR/Unity runtimes.

---

### 4. Which AI models power Aetheris?
The platform architecture utilizes a pluggable provider boundary:
* **Google Gemini**: Deeply integrated with Gemini 2.0 Flash and 1.5 Pro for multimodal visual reasoning and scientific document comprehension.
* **OpenAI**: Supports GPT-4o and GPT-4o-mini.
* **Local Models (Private / Air-Gapped)**: Native support for Ollama and vLLM (e.g., DeepSeek-R1, Llama 3) for confidential enterprise research labs.
* **Deterministic Grounded Stub**: Zero-cost, network-free local testing and offline fallback.

---

### 5. Is my research data and reading history private?
Yes. In the core engine:
* Reading sessions, gaze heatmaps, and spatial notes are stored privately on local infrastructure.
* For enterprise and defense research labs, Aetheris supports 100% offline local inference using local LLMs (e.g., via Ollama/vLLM), ensuring zero data leaves your local machine.

---

### 6. Why is the core codebase kept in a private repository?
Aetheris contains proprietary spatial raycasting heuristics, document layout boundary decomposition algorithms, and specialized deictic disambiguation logic. This repository (`Aetheris-Showcase`) provides public specifications, architectural overviews, and interactive demonstrations, while the production backend and deployment scripts are maintained under `aetheris-core`.

---

### 7. How can I request early access or partner with the team?
We are actively working with select academic research labs, PhD candidates, and deep-tech engineers. To request early access or explore collaboration:
* **Email**: [bhoopendrasinghbhadauria5@gmail.com](mailto:bhoopendrasinghbhadauria5@gmail.com)
* **Lead Researcher**: Bhoopendra Singh Bhadauria
