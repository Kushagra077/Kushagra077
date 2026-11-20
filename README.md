# Kushagra Pandya

AI Engineer in Rajkot, India. I have spent 2.5+ years building production computer vision and document-AI systems (identity-document classification and extraction, liveness and deepfake detection), and I now build multi-agent LLM pipelines.

Most of my day job is client work I can't show, so this profile is the work I can: projects with measured results, and the trade-offs written down.

---

## Agentic and LLM projects

### [Multi-Agent Research Assistant](https://github.com/Kushagra077/multi-agent-research-assistant)
A planner splits a question into subtasks, parallel researchers search the web and answer from the pages, and a writer drafts a cited report. TypeSafe's Jev makes four small typed decisions (is a source useful, does an answer address its subtask, retry or escalate, is the draft ready). The run pauses for a person to approve, reject with feedback or take over, and survives a restart.
Measured: median 0.50 s per Jev decision over 42 calls; on 35 saved pages Jev and a Groq LLM judge each dropped all 7 off-topic ones (small sample, one topic).
`LangGraph` `FastAPI` `Streamlit` `SQLite` `Docker` `Groq` `Gemini` `Tavily`

### [SmartIngest](https://github.com/Kushagra077/SmartIngest): agentic document intelligence
Classifies an invoice, contract, resume or ID, extracts structured fields, validates them, and routes the document to auto-approve, review or reject. A deterministic router (not an LLM call), prompt-injection and PII guardrails, a grounding check, and an eval harness used as a CI gate with 72 tests. [90-second demo](https://youtu.be/DgXVG6Zd9wA)
`LangGraph` `Pydantic` `FastAPI` `Gemini` `LangSmith` `Docker`

### [RecruitRadar](https://github.com/Kushagra077/RecruitRadar): multi-agent recruitment screener
Screens a folder of resumes against a job description into a ranked shortlist, interview kits and outreach drafts. The 0 to 100 score is computed in Python, never emitted by the model, and every claimed skill must cite a verbatim resume quote that is fuzzy-verified. [Walkthrough](https://youtu.be/4_sv16UfuZM)
`CrewAI` `Gemini` `LiteLLM` `SQLite`

---

## Computer vision projects

### [football-detect-serve](https://github.com/Kushagra077/football-detect-serve): detection and serving
Four YOLO26 detectors (ball, goalkeeper, player, referee) served as speed/accuracy presets behind a batching FastAPI service: test mAP50-95 0.400 to 0.477 at 16 to 177 ms per 1080p frame on CPU. Benchmarked torch vs ONNX fp32 vs INT8, load-tested with Locust. [Live demo](https://huggingface.co/spaces/Kushagra77/football-detect-serve)

### [football-team-tracker](https://github.com/Kushagra077/football-team-tracker): tracking and team assignment
Stable player IDs and a two-team split from broadcast video. Seven trackers benchmarked with TrackEval on SoccerNet-Tracking: best is BoT-SORT with camera-motion compensation at 63.6 HOTA on my own detector's boxes (84.2 with perfect boxes). [2-minute demo](https://youtu.be/YrP9KGjes4g)

### [football-tactical-metrics](https://github.com/Kushagra077/football-tactical-metrics): tracking data to validated metrics
Two tracking-data providers behind one schema and one metrics layer (defensive line height, compactness, Voronoi space control, distance and sprints), checked against synthetic ground truth with known answers.

---

## At TSS Consultancy

KYC and identity-verification AI (numbers are from my own benchmarks and production logs):

- Identity-document classification and detection: 98.92% on a ~3K-image in-house benchmark, ~50K requests/day, ~0.5 s model inference
- Passive liveness detection: 89% average accuracy on held-out open datasets, ~0.5 s inference, used by a client at ~1,000 requests/day
- Aadhaar field extraction, photo match improvements, and a deepfake detector (92% on a curated open-data test set)

---

## Stack

**Languages** Python, SQL
**Vision** PyTorch, Ultralytics (YOLO), OpenCV, ONNX Runtime, PaddleOCR, TrackEval
**LLM / agents** LangGraph, LangChain, CrewAI, LangSmith, Pydantic, ChromaDB
**Serving / MLOps** FastAPI, Flask, Docker, Locust, GitHub Actions, MLflow, Weights & Biases

## Research and patents

- Two IEEE conference papers (first of six authors on both), including *Barcode and QR Code Object Detection: An Experimental Study on YOLOv8 Models* (INNOCOMP 2024)
- Four patent applications filed with IP India, all published, one granted (a navigational aid device for visually impaired people)
- [Google Scholar](https://scholar.google.com/citations?user=HXtTZCoAAAAJ&hl=en) · ORCID [0009-0007-7695-335X](https://orcid.org/0009-0007-7695-335X)

B.Tech, Computer Engineering (AI specialization), Marwadi University, 2024.

---

[Portfolio](https://www.kushagrapandya.in/) · [LinkedIn](https://www.linkedin.com/in/kushagra-pandya/) · [Hugging Face](https://huggingface.co/Kushagra77)
