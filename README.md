# Kushagra Pandya

Software Engineer (AI) at [TSS Consultancy](https://www.tssconsultancy.com/), Rajkot. I build production computer vision systems and multi-agent LLM pipelines.

Most of my day job ships behind a RegTech product and stays private, so this profile is mostly the work I can show: agentic pipelines with real evaluation harnesses, and CV work I rebuild in the open.

**Current focus:** multimodal vision-agent systems, where video understanding meets agentic reasoning.

---

## What I work on at TSS

KYC and compliance infrastructure for a WestBridge-backed RegTech product (SOC 2 Type 2, ISO 27001).

- Face liveness detection API running in production, tuned for sub-second p99 under real request load
- Object detection and multilingual OCR across 8 Indian languages
- Ongoing research into deepfake and forged document detection

---

## Projects

### [SmartIngest](https://github.com/Kushagra077/SmartIngest) — agentic document intelligence

Upload an invoice, contract, resume or ID. It classifies the document, extracts structured fields, validates them against business rules, and routes it to auto-approve, review, or reject.

LangGraph orchestration, Gemini vision, Pydantic-typed extraction, prompt-injection and PII guardrails, grounding checks with a confidence-triggered retry loop, deterministic YAML routing, LangSmith tracing end to end.

`Python 3.12` `LangGraph` `FastAPI` `Gemini` `Pydantic` `Docker` `LangSmith`
72 tests, eval harness wired as a CI gate. [90-second demo](https://youtu.be/DgXVG6Zd9wA)

### [RecruitRadar](https://github.com/Kushagra077/RecruitRadar) — multi-agent recruitment screener

Drop in a job description and a folder of resumes. Get a ranked shortlist with auditable 0 to 100 scores, tailored interview kits, and drafted outreach.

Five CrewAI agents with an embedding pre-filter. Scoring is computed in Python with weighted sums, never emitted by the model, and every matched skill has to cite a verbatim resume quote verified with rapidfuzz.

`Python` `CrewAI` `Gemini` `LiteLLM` `rapidfuzz` `SQLModel` `SQLite`
[Full walkthrough](https://youtu.be/4_sv16UfuZM)

More at **[kushagrapandya.in](https://kushagrapandya.in)**.

---

## Stack

**Languages** Python, Java
**CV** PyTorch, OpenCV, YOLO, Vision Transformers, ONNX
**LLM / agents** LangGraph, LangChain, CrewAI, LangSmith, ChromaDB
**Backend** FastAPI, Flask, Docker, Azure, SQLModel

---

## Research and IP

- 2 IEEE conference papers, including *Barcode and QR Code Object Detection: An Experimental Study on YOLOv8 Models* (INNOCOMP 2024)
- 4 patent applications filed with IP India, 1 granted: a navigational aid device for the visually impaired
- Earlier research on sign language translation and myoelectric prosthetic control
- ORCID: [0009-0007-7695-335X](https://orcid.org/0009-0007-7695-335X)

## Writing

I publish roughly weekly on [Medium](https://medium.com/@p.kushagra22), mostly notes from building agent systems: structured output, middleware, evaluation, and what breaks in practice.

## Education

B.Tech, Computer Engineering (AI specialization), Marwadi University, 2024. CGPA 8.51.

---

[Portfolio](https://kushagrapandya.in) · [LinkedIn](https://www.linkedin.com/in/kushagra-pandya/) · [Medium](https://medium.com/@p.kushagra22) · [Hugging Face](https://huggingface.co/Kushagra77)
