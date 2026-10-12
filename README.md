# 👋 Hi, I'm Almajir MASSALABI OUMAROU

🇲🇦 **Data Science & AI Engineering Student** based in Morocco — Building intelligent systems for real-world impact.

---

## 🚀 Featured Projects

| Project | Description | Stack | Status |
|---------|-------------|-------|--------|
| **[lumina-rag](https://github.com/amassalabi-spec/lumina-rag)** | 🇲🇦 RAG Assistant for Erasmus+ Maroc — 100% local, sovereign data, hybrid semantic search, semantic caching, admin dashboard | `FastAPI` `React` `ChromaDB` `Phi-3` `Docker` `Python` `TypeScript` | 🟢 Active |
| **[validateur-dgi](https://github.com/amassalabi-spec/validateur-dgi)** | 🇲🇦 Fiscal Compliance Validator (CGI Morocco) — Invoice extraction, hybrid Gemini/Regex parsing, DGI audit engine (6 rules), PDF generation | `Spring Boot 3.4` `Thymeleaf` `MySQL` `Java 17` `Maven` `Flying Saucer` | 🟢 Active |
| **[sira-predictive-logistics](https://github.com/amassalabi-spec/sira-predictive-logistics)** | 🚚 Predictive Logistics Dashboard — Real-time analytics, shipment predictions, crisis management, Vercel deployment | `Next.js 14` `TypeScript` `Tailwind` `shadcn/ui` `Vercel` `Genkit` | 🟢 Active |
| **[learning-journey](https://github.com/amassalabi-spec/learning-journey)** | 📚 Learning Monorepo — Python fundamentals → Data Science labs → ML projects (web scraping, Streamlit, NLP) | `Python` `Pandas` `Streamlit` `Selenium` `Transformers` `Jupyter` | 📚 Archived |

---

## 🧪 Chatbot Architecture Lab (Current Focus)

> **Expérimentation active** — Test de différentes architectures pour un chatbot intelligent, avec accès GPU dédié.

| Architecture | Approche | Stack Testée | Statut | Notes |
|--------------|----------|--------------|--------|-------|
| **Local LLM** | Phi-3 Mini / Llama-3 / Mistral via `llama-cpp-python` / `vLLM` | GGUF 4-bit, quantization, KV-cache tuning | 🟢 En cours | Latence ~0s, privacy totale, RAM/GPU VRAM limit |
| **API LLM** | OpenAI / Anthropic / Mistral API / Groq / Together | REST + Streaming (SSE), function calling | 🟢 Testé | Qualité supérieure, coût/latence réseau, dépendance externe |
| **Agentic (ReAct/Plan-Execute)** | LangGraph / CrewAI / AutoGen / custom orchestrator | Tools (search, code exec, RAG), multi-step reasoning | 🟡 Prototypage | Puissant pour tâches complexes, overhead tokens/latence |
| **Fine-tuning (LoRA/QLoRA)** | Unsloth / Axolotl / HuggingFace TRL sur dataset custom | QLoRA 4-bit, gradient checkpointing, Flash Attention 2 | 🔴 Planifié | Besoin dataset curaté, eval rigoureuse, GPU hours |

### 🎯 Objectifs d'Évaluation

| Critère | Local LLM | API LLM | Agent | Fine-tuned |
|---------|-----------|---------|-------|------------|
| **Qualité réponses** | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ (domaine) |
| **Latence** | ⚡⚡⚡ | ⚡⚡ | ⚡ | ⚡⚡⚡ |
| **Coût inférence** | 💰 (GPU owned) | 💰💰💰/1M tokens | 💰💰💰 | 💰 (GPU owned) |
| **Privacy / Data Sovereignty** | ✅ Total | ❌ Externe | ✅/❌ selon tools | ✅ Total |
| **Personnalisation domaine** | Prompt/RAG | Prompt/RAG | Tools + Prompt | **Poids du modèle** |
| **Maintenance** | Modèle + Infra | Clé API | Orchestration + Tools | Dataset + Training + Eval |

### 🔬 Setup Expérimental Actuel

```yaml
# GPU Disponible
GPU: NVIDIA RTX 3090 / A10G (24GB VRAM)  # ou similaire
VRAM: 24GB → supporte jusqu'à 13B params Q4_K_M / 7B Q8_0

# Stack Test
- vLLM / TGI pour serving haute performance (continuous batching)
- LangGraph pour agents stateful (checkpointing, human-in-the-loop)
- Unsloth pour QLoRA 2-4x plus rapide (Flash Attention 2)
- RAGAS / LangSmith pour évaluation (faithfulness, answer_relevancy)
- Weights & Biases / MLflow pour tracking expériences
```

### 📋 Prochaines Étapes

- [ ] Finaliser benchmark comparatif (latence, qualité, coût) sur 50+ queries représentatives
- [ ] Construire dataset d'évaluation *golden set* (Q/A + contexts + expected)
- [ ] Tester **RAG + Fine-tuning hybride** : LoRA sur adaptateurs de domaine + RAG pour connaissance fraîche
- [ ] Implémenter **guardrails** (NeMo Guardrails / LangChain output parsers) pour sécurité
- [ ] Documenter architecture retenue dans repo dédié `chatbot-architecture-lab`

---

## 🛠 Tech Stack

**AI/ML & Data**
`Python` `PyTorch` `Transformers` `LangChain` `LangGraph` `Sentence-Transformers` `ChromaDB` `Phi-3/GGUF` `Llama-3` `Mistral` `scikit-learn` `Pandas` `NumPy` `Jupyter` `Unsloth` `vLLM` `RAGAS`

**Backend & APIs**
`FastAPI` `Spring Boot 3` `Java 17` `MySQL` `PostgreSQL` `REST` `SSE` `Docker` `Docker Compose`

**Frontend & Web**
`React 18` `Next.js 14` `TypeScript` `Tailwind CSS` `shadcn/ui` `Chart.js` `Vite` `Vercel`

**DevOps & Tools**
`Git` `GitHub Actions` `Maven` `npm/pnpm` `Linux` `VS Code` `IntelliJ` `Cloudflare Tunnel` `Weights & Biases` `MLflow`

---

## 📊 GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=amassalabi-spec&show_icons=true&theme=tokyonight&hide_border=true&count_private=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=amassalabi-spec&layout=compact&theme=tokyonight&hide_border=true)

---

## 🎯 Current Learning Focus

- 🔬 **RAG Systems** — Local-first LLMs, hybrid search, evaluation frameworks (RAGAS)
- 🇲🇦 **Fiscal Tech** — Moroccan tax compliance automation (CGI/DGI)
- 📈 **Predictive Analytics** — Time-series forecasting, logistics optimization
- 🏗 **Software Architecture** — Clean architecture, domain-driven design, modular monoliths
- 🤖 **LLM Ops** — Serving (vLLM/TGI), Fine-tuning (QLoRA), Agents (LangGraph), Evaluation

---

## 📫 Connect

[![Email](https://img.shields.io/badge/Email-amassalabi%40gmail.com-red?style=flat-square&logo=gmail)](mailto:amassalabi@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/amassalabi)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat-square&logo=github)](https://github.com/amassalabi-spec)

---

## 💡 Philosophy

> *"Build systems that work offline, respect privacy, and solve real problems."*

**Approach**: Local-first • Sovereign data • Incremental delivery • Measurable impact • **Learn by building**

---

![Profile Views](https://komarev.com/ghpvc/?username=amassalabi-spec&color=blueviolet&style=flat-square&label=Profile+Views)