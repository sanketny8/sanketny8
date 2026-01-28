# Hi there, I'm Sanket Nyayadhish 👋

<div align="center">
  
  **Senior AI Engineer | LLMs × GenAI × Backend × Cloud Infrastructure**
  
  Building production LLM systems, scalable backends, and AI-optimized infrastructure
  
  [![Twitter Follow](https://img.shields.io/twitter/follow/Ny8Sanket?style=social)](https://twitter.com/Ny8Sanket)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://linkedin.com/in/ny8sanket)
  
</div>

---

## 🚀 About Me

I'm a senior engineer passionate about building production-grade AI systems at the intersection of LLMs, distributed backends, and cloud-native infrastructure. My work focuses on taking cutting-edge AI research and transforming it into reliable, scalable systems that solve real-world problems.

I believe in learning by building, sharing knowledge openly, and pushing the boundaries of what's possible with modern AI technology.

---

## 💡 Core Competencies

### 🤖 LLMs & GenAI
- **RAG Systems**: Advanced retrieval, hybrid search, reranking, multi-modal support
- **Fine-tuning**: LoRA/QLoRA, RLHF, DPO for domain-specific models
- **Prompt Engineering**: Chain-of-Thought, ReAct, self-reflection patterns
- **LLM Agents**: Multi-agent orchestration, tool use, planning & execution
- **Vector Databases**: Weaviate, Qdrant, Pinecone, pgvector

### 🧠 AI/ML Stack
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![Transformers](https://img.shields.io/badge/🤗_Transformers-FFD21E?style=flat)
![LangChain](https://img.shields.io/badge/🦜_LangChain-339933?style=flat)
![vLLM](https://img.shields.io/badge/vLLM-00599C?style=flat)

- Hugging Face Transformers, PEFT, TRL
- LangChain, LlamaIndex, LangGraph
- vLLM, TGI, ONNX Runtime
- MLflow, Weights & Biases
- sentence-transformers, OpenAI/Anthropic APIs

### ⚙️ Backend & Services
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=flat&logo=google&logoColor=white)

- Go: High-performance microservices, gRPC, concurrency
- Python: FastAPI, async programming, data pipelines
- Event-Driven Architecture: NATS, Kafka, Redis Streams
- API Design: REST, gRPC, GraphQL
- Observability: OpenTelemetry, Prometheus, Jaeger

### ☁️ AI Infrastructure & MLOps
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

- Kubernetes: GPU scheduling, model serving (KServe), Ray clusters
- Terraform: Multi-cloud IaC, GPU node pools
- GitOps: ArgoCD, Flux CD
- Model Serving: vLLM operator, Triton, KServe
- GPU Optimization: NVIDIA GPU Operator, DCGM, MIG

### 🗄️ Data & Databases
- PostgreSQL (with pgvector for embeddings)
- Redis (caching, queues, semantic cache)
- Vector Stores: Weaviate, Qdrant
- ElasticSearch (hybrid search)

---

## 🎯 Featured Projects

### 🔍 [Enterprise RAG System](https://github.com/sanketny8/enterprise-rag-system)
Production-grade Retrieval Augmented Generation platform with advanced chunking, hybrid search, and multi-LLM support.

**Key Features:**
- Hybrid retrieval (dense + sparse) with cross-encoder reranking
- Multi-LLM router (OpenAI, Anthropic, local models)
- Streaming responses with citation tracking
- Comprehensive RAG evaluation framework (RAGAS)
- Cost optimization and semantic caching

**Tech:** Python, FastAPI, LangChain, Weaviate, vLLM, Redis, ElasticSearch

---

### 🤖 [Autonomous LLM Agents](https://github.com/sanketny8/autonomous-llm-agents)
Multi-agent system demonstrating agentic AI patterns with tool use, planning, memory, and orchestration.

**Key Features:**
- ReAct pattern with self-reflection and planning
- Dynamic tool registry (web search, code execution, APIs)
- Multi-tier memory system (short-term, long-term, episodic)
- Sandboxed execution environment
- Human-in-the-loop for critical actions

**Tech:** Python, LangGraph, GPT-4, Claude, Weaviate, Redis

---

### 🎓 [LLM Fine-tuning Platform](https://github.com/sanketny8/llm-finetuning-platform)
End-to-end platform for fine-tuning open-source LLMs with experiment tracking, evaluation, and deployment.

**Key Features:**
- LoRA/QLoRA fine-tuning for Llama 3, Mistral, Phi models
- Comprehensive evaluation (MMLU, HellaSwag, custom benchmarks)
- MLflow + W&B experiment tracking
- Automatic deployment to vLLM inference
- Resource optimization and cost analysis

**Tech:** PyTorch, Transformers, PEFT, bitsandbytes, MLflow, vLLM

---

### ⚡ [AI Gateway Microservices](https://github.com/sanketny8/ai-gateway-microservices)
High-performance Go backend for LLM service routing, request management, and observability.

**Key Features:**
- Multi-provider LLM routing with failover
- Semantic caching for cost reduction
- Token-based rate limiting and billing
- Priority queue with batch processing
- Sub-10ms p99 latency for cache hits

**Tech:** Go, gRPC, Redis, PostgreSQL, OpenTelemetry, Prometheus

---

### 🏗️ [GPU Kubernetes Platform](https://github.com/sanketny8/gpu-kubernetes-platform)
Production Kubernetes infrastructure optimized for GPU workloads and model serving with GitOps.

**Key Features:**
- Terraform modules for GPU node pools (T4, A10G, A100)
- KServe + vLLM operator for scalable inference
- Ray on Kubernetes for distributed training
- DCGM monitoring and cost optimization
- GitOps deployment with ArgoCD

**Tech:** Terraform, Kubernetes, Helm, ArgoCD, NVIDIA GPU Operator, KServe, Ray

---

## 📊 LLM/GenAI Expertise

<div align="center">

### Supported Models & Frameworks

| Category | Technologies |
|----------|-------------|
| **Proprietary LLMs** | GPT-4, GPT-4 Turbo, Claude 3 (Opus/Sonnet/Haiku), Gemini Pro |
| **Open Source LLMs** | Llama 3/3.1, Mistral 7B/8x7B, Phi-3, Qwen 2, Gemma 2 |
| **Embedding Models** | OpenAI Ada-002, Cohere, sentence-transformers, BGE, E5 |
| **Inference Engines** | vLLM, TGI (Text Generation Inference), ONNX Runtime, Triton |
| **Frameworks** | LangChain, LlamaIndex, LangGraph, CrewAI, Transformers |

</div>

---

## 📈 Learning Journey

I'm committed to continuous learning and sharing knowledge about production AI systems:

- 🔬 **Experimenting** with cutting-edge techniques (Graph RAG, Corrective RAG, Constitutional AI)
- 📝 **Writing** about lessons learned building GenAI systems at scale
- 🛠️ **Contributing** to open-source AI projects (vLLM, LangChain, Transformers)
- 🎓 **Implementing** recent AI research papers (RAPTOR, HyDE, Reflexion)
- 💬 **Sharing** insights on prompt engineering, RAG optimization, and LLMOps

---

## 🌱 Current Focus

- Building agentic workflows with multi-agent collaboration
- Optimizing RAG systems for production (latency, cost, quality)
- Exploring RLHF and DPO for LLM alignment
- GPU cost optimization strategies for model serving
- Responsible AI practices and bias mitigation

---

## 📫 Let's Connect!

I'm always interested in connecting with fellow engineers, researchers, and builders in the AI space.

- 🐦 **Twitter/X**: [@Ny8Sanket](https://twitter.com/Ny8Sanket)
- 💼 **LinkedIn**: [in/ny8sanket](https://linkedin.com/in/ny8sanket)
- 📧 **Email**: Available on LinkedIn
- 💬 **Open to**: Collaboration, technical discussions, mentorship

---

## 📊 GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=sanketny8&show_icons=true&theme=radical&hide_border=true&include_all_commits=true&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=sanketny8&layout=compact&theme=radical&hide_border=true&langs_count=8)

---

<div align="center">
  
  **"Building the future of AI, one system at a time"**
  
  ⭐️ From [sanketny8](https://github.com/sanketny8)
  
</div>

