Healthcare-ZeroStream
An offline-first AI public health triage and medical accessibility tool designed for low-connectivity, zero-resource clinics.
Built with a $0 budget using free-tier cloud resources and local on-device machine learning.
UN SDG Alignment: This project aligns directly with the following United Nations Sustainable Development Goals. SDG 3:

Good Health and Well-being — Democratizing immediate medical triage guidance in remote villages. SDG 10:
Reduced Inequalities — Bridging the digital divide by ensuring life-saving software works without paid data streaming.

The Zero-Budget Tech Stack
| Layer | Technology | Cost | Why It Is Chosen |

|Frontend UI |HTML5, Tailwind CSS, Vanilla JS | $0 | Lightweight, fast loading, and completely beginner-friendly|

|Local AI Engine |Hugging Face Transformers.js | $0 |Runs open-source AI models entirely inside the browser cache|

|AI Model |Xenova/Qwen1.5-0.5B-Chat | $0 |An ultra-lightweight text model optimized for local mobile CPUs|

|Local Storage |Browser IndexedDB API | $0 |Saves local patient history securely on-device without cloud costs|

|Hosting & CDN |GitHub Pages | $0 | Free global web hosting directly from this repository|

Architecture & Data Flow Because Healthcare ZeroStream is offline-first, it completely bypasses traditional cloud servers

[ User Browser ]
│
├───► [ UI Layer: HTML/JS ] ───────► Captures symptoms & scale fonts for accessibility
│
├───► [ Engine: Transformers.js ] ─► Processes chat requests locally on device CPU
│
└───► [ Storage: IndexedDB ] ──────► Permanent local cache of the 0.5B AI Model

The Initial Load Mechanic
1. A community health worker opens the app URL once while connected to internet at a regional base.
2. The browser automatically downloads the static web page and the compressed AI model weights.
3. The browser permanently caches these files.
4. The worker travels deep into a remote clinic with zero cellular signal. The app remains 100% functional.

8-Week Implementation Roadmap

Weeks 1–2: Visual Foundation & Accessibility
* Create a responsive user interface with high-contrast text layout for outdoor readability.
* Add text-scaling accessibility options for visually impaired users.
* Design a clean chat interface for inputting symptom profiles.

Weeks 3–4: Browser AI Core
* Import the Transformers.js engine into the application scripts.
* Implement initialization logic to fetch and load the light 0.5B parameter language model.
* Build a dynamic download progress tracker to inform workers of installation status.

Weeks 5–6: Triage Logic & Secure Storage
* Prompt engineer the local AI engine to act strictly as a first-aid sorting assistant (not a diagnosing doctor).
* Set up standard IndexedDB tables to store date-stamped triage logs.
* Ensure maximum client-side data privacy with absolute zero network leakage.

Weeks 7–8: Field Simulation & Deployment
* Benchmark performance by throttling execution speeds to emulate low-end mobile hardware.
* Finalize project open-source documentation.
* Activate GitHub Pages for automated public deployment.

How to Run Locally
1. Clone this repository or download the source code.
2. Open the `index.html` file in any modern web browser (Chrome, Edge, Safari, Firefox).
3. Allow the initial AI engine to download into your local browser cache.
4. Disconnect your internet completely and test the system!
5. 
[1] [https://www.hass-agent.io](https://www.hass-agent.io/2.2/contributing/docs/editing-files/)

[2] [https://book.the-turing-way.org](https://book.the-turing-way.org/collaboration/github-novice/github-novice-firststeps/)
