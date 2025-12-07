<!--What i propose.md-->

# backend first, frontend second
We must separate **infrastructure** from **curation**.
* **The Backend (Centralized):** A shared, geo-redundant server cluster (e.g., Nodes in Paris, Frankfurt, Warsaw) handling the heavy lifting: storage, transcoding, and streaming. This is purely technical and non-political.
* **The Frontend (Decentralized):** National broadcasters retain full control over their apps and editorial decisions. The "Tagesschau" app remains the "Tagesschau" app, but it fetches video assets from the Aletheia API. This preserves cultural independence while solving technical inefficiency.

# app/web first strategy
The system is designed for the digital native.
* **Just-in-Time Transmuxing:** Content is stored in high-fidelity Master Files and converted instantly to streaming formats (DASH/HLS) suitable for the user's device.
* **Mobile-Centric:** The architecture prioritizes low-latency mobile streaming and offline capabilities.
* **Universal API:** A single, documented API allows third-party developers (and national broadcasters) to build diverse interfaces on top of the same library.

# AI in public broadcasting
AI is not used to generate fake content, but to make real content accessible.
* **The Ingest Pipeline:** Every uploaded video is automatically processed:
    * **Auto-Transcription:** Generating searchable text for accessibility.
    * **Translation & Dubbing:** AI generates synthetic audio tracks in all 24 official EU languages, preserving the original speaker's timbre.
    * **Upscaling:** Legacy archive footage is upscaled to 1080p/4K to meet modern viewing standards.
* **History X-Ray:** An NLP-based layer that provides context for historical content (e.g., outdated language) without censorship.

# open source as foundation of trust
In an era of deepfakes and algorithmic manipulation, public media must be transparent.
* **Public Code:** The entire backend infrastructure is Open Source. Anyone can audit how the news feed is assembled or how the recommendation algorithm works.
* **Security:** "Security through transparency." We invite the global security community to harden our infrastructure.
* **Provenance:** All content is cryptographically signed (C2PA) to prove it comes from a trusted public source and has not been altered.

# public money, public content
We propose a radical shift in licensing: **"Pay Once, Own Forever."**
* **No DRM:** Content fully financed by public funds should be free of Digital Rights Management.
* **Download Rights:** Citizens have the right to download high-quality Matroska (.mkv) files of public content for private archiving, remixing, and education.
* **The Asset:** We provide multi-track files (Original Audio + AI Dubs + Subtitles) so the content remains a living cultural asset, not a rental product.