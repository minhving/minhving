# Minh Vi Nguyen (MinhViNguyen) — AI Engineer / Applied ML

I build **production-minded AI systems**: data → models → evaluation → APIs → deployment.  
Current focus: **Computer Vision pipelines**, **RAG/LLM systems**, and **MLOps** (Docker, CI/CD).

- 📍 Melbourne, Australia
- 🎓 BCompSci (AI), La Trobe University (GPA 91/100) | Provost’s Commendation 2024
- 🔭 Interested in: CV, RAG, agents, evaluation, deployment, responsible AI

## Quick Links
- GitHub: https://github.com/minhving
- LinkedIn: https://www.linkedin.com/in/minhvinguyen
- Portfolio: https://www.minhvinguyen.com
- Email: minhvi176@gmail.com

---

## Tech Stack (Engineering-Focused)

### Languages
- **Python**, JavaScript/TypeScript, SQL

### ML / AI
- **PyTorch**, scikit-learn (and exposure to TensorFlow)
- **Computer Vision**: detection, segmentation, depth estimation
- **LLMs**: OpenAI / Claude / Gemini
- **RAG**: embeddings, chunking, retrieval, grounding & evaluation

### LLM / Agent Frameworks
- LangChain, LlamaIndex, LangGraph, CrewAI

### Data & Search
- Pandas, NumPy
- Vector DB: FAISS, Pinecone

### Backend & Infra
- **FastAPI**
- **Docker**
- CI/CD: GitHub Actions
- Cloud exposure: **AWS** (S3, Lambda, SageMaker, Bedrock), Azure, GCP

---

## What I’m Good At (Signals)
- Designing **end-to-end AI workflows** (not just notebooks)
- Building **modular pipelines** (clear interfaces between stages)
- Shipping models behind **APIs** with reproducibility (Docker)
- Doing **evaluation properly**: metrics, ablations, error analysis, iteration loops
- Communicating with stakeholders: turning vague needs into measurable outputs

---

## Featured Projects

### 1) Freshtify — Shelf Stock-Level Estimation (CV Pipeline)
**Goal:** detect products on shelves and estimate stock/availability reliably in real-world store conditions.

**Pipeline (multi-stage):**
- **Detection**: Grounding DINO (prompt-guided object detection)
- **Segmentation**: SAM2 for instance masks (better boundary precision)
- **Depth**: Depth-Anything-V2 for depth cues (improves portion/volume inference)
- **Reasoning / Post-processing**: LLM-assisted logic for aggregation rules & edge cases
- **Serving**: FastAPI inference service + Docker for reproducibility

**Results (reported):**
- ~**88% detection accuracy**
- ~**85% stock-level accuracy**

**Engineering highlights:**
- Modular stages to allow swapping models independently
- Batch inference utilities for benchmarking & regression checks
- Designed for integration into downstream product experiences

---

### 2) Food Calorie Estimation (CV + RAG)
**Goal:** estimate calories from a food image by combining vision geometry with nutrition knowledge.

**Approach:**
- **Segmentation** (SAM2) → food mask
- **Depth estimation** (Depth-Anything-V2) → relative volume cues
- **RAG** → density/nutrition lookup for calorie estimation
- Evaluation across **~90 food types**

**Results (reported):**
- ~**95% detection accuracy**
- Calorie error within **±50 kcal** (target range)

**Engineering highlights:**
- Clear separation of “perception” (CV) vs “knowledge” (RAG)
- Evaluation loops: failure modes by lighting/angle/occlusion

---

### 3) Hand-Gesture YouTube Search (Realtime UX + Retrieval)
**Goal:** translate hand gestures into intent and retrieve relevant YouTube videos.

**System:**
- **Gesture sensing**: MediaPipe (~1s)
- **Retrieval**: embeddings over titles + vector search
- **Intent refinement**: GPT-4o to map gesture → query + rerank

**Engineering highlights:**
- Latency-conscious pipeline
- Retrieval-first design, LLM used where it adds value (intent/rerank)

---

## Experience Snapshot

### AI Engineering — Centre for Data Analytics and Cognition (La Trobe)
- Built and iterated on **CV pipelines** for ingredient detection & calorie estimation
- Reproducible experimentation via **Docker**
- Stakeholder iteration: requirements → prototype → evaluation → improvements

### Researcher — Tien Giang University
- Compared baseline vs improved approaches for classification workflows
- Evaluated ACUTE and improved SVM classification via **Twin Vector** methods
- Focused on controlled experimentation and validation

---

## How I Like to Build (My Default Workflow)
1. **Define success** (metric + acceptable error)
2. **Baseline fast** (simple pipeline, measurable)
3. **Instrument** (logging, dataset versioning, eval scripts)
4. **Iterate** (ablation + error analysis)
5. **Deploy** (API + Docker)
6. **Monitor** (drift/quality checks where applicable)

---

## Repository Notes
This is my **GitHub profile README**.  
Pinned repos highlight end-to-end AI builds (CV/RAG) with:
- reproducible environments
- clear architecture
- evaluation and reporting

---

## Contact
If you’re hiring for **AI Engineer / Applied ML / CV / RAG** roles, feel free to reach out:
- minhvi176@gmail.com
- https://www.linkedin.com/in/minhvinguyen
