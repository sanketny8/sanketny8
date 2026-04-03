<div align="center">

  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=32&duration=2800&pause=2000&color=8A2BE2&center=true&vCenter=true&width=940&lines=Hi+%F0%9F%91%8B%2C+I'm+Sanket+Nyayadhish;AI+Engineer+%7C+LLM+Inference+%2B+Backend+%2B+Infra;Building+Production+LLM+Systems" alt="Typing SVG" />

  <a href="https://twitter.com/Ny8Sanket"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter" /></a>
  <a href="https://linkedin.com/in/ny8sanket"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://sanketny8.github.io"><img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio" /></a>

  [![AI Daily Digest](https://img.shields.io/badge/AI_Daily_Digest-Trending_Papers_%7C_Repos_%7C_Blogs-8A2BE2?style=for-the-badge)](https://github.com/sanketny8/ai-daily-digest)

</div>

---

## About Me

I'm an AI Engineer working at the intersection of **LLM inference systems**, **distributed backends**, and **cloud-native infrastructure**. I focus on taking models from research to production -- building the serving layers, orchestration pipelines, and GPU infrastructure that make LLM systems work at scale.

**Currently working on:**

- Low-latency, fault-tolerant backends for LLM and GenAI workloads
- LLM serving infrastructure -- vLLM, TensorRT-LLM, KV cache optimization
- GPU workload orchestration on Kubernetes with autoscaling and workload-aware scheduling
- Agentic AI backends with multi-agent orchestration, tool use, and planning
- MCP (Model Context Protocol) servers and integrations for tool-augmented LLMs
- Observability for AI systems -- latency, drift, GPU utilization

---

<details>
<summary><strong>Core Competencies</strong> &mdash; Systems, LLMs, Infrastructure</summary>

<br>

**Distributed Systems & Backend**

- **System Design** -- microservices, event-driven architecture, CQRS, domain-driven design
- **Scalability** -- horizontal sharding, consistent hashing, load balancing, distributed caching (Redis, Memcached)
- **Performance** -- gRPC and protobuf for low-latency communication, async I/O, connection pooling, concurrency patterns
- **Resilience** -- circuit breakers, bulkhead isolation, rate limiting, exponential backoff, graceful degradation
- **Observability** -- distributed tracing (OpenTelemetry, Jaeger), metrics (Prometheus, Grafana), structured logging

**LLMs & GenAI**

- **RAG Systems** -- hybrid retrieval (dense + sparse), cross-encoder reranking, query decomposition, evaluation with RAGAS
- **Fine-tuning** -- LoRA, QLoRA, RLHF, DPO, dataset curation, evaluation pipelines, experiment tracking (MLflow, W&B)
- **LLM Agents** -- multi-agent orchestration, ReAct and plan-and-execute patterns, tool use, sandboxed code execution
- **MCP** -- Model Context Protocol server development, tool registries, context injection, integration with Claude and GPT
- **Inference Optimization** -- vLLM, TGI, TensorRT-LLM, KV cache tuning, continuous batching, speculative decoding, quantization (GPTQ, AWQ)

</details>

---

<details>
<summary><strong>Technical Stack</strong> &mdash; Languages, Frameworks, Infrastructure</summary>

<br>

**AI / ML**

- **Languages:** Python (primary), some C++ for performance-critical paths
- **Frameworks:** PyTorch, Transformers, LlamaIndex, LangChain, LangGraph
- **Agents:** MCP servers, CrewAI, AutoGen, Claude Agent SDK, PydanticAI
- **Inference:** vLLM (PagedAttention), TGI, ONNX Runtime, Triton Inference Server, TensorRT-LLM
- **Training:** PEFT (LoRA/QLoRA), DeepSpeed ZeRO, bitsandbytes quantization, Unsloth
- **Evaluation:** RAGAS, LangSmith, custom eval harnesses

**Backend & Distributed Systems**

- **Languages:** Go (high-throughput services), Python (FastAPI, async services)
- **Messaging:** Apache Kafka (event streaming), Redis Streams, RabbitMQ
- **Protocols:** gRPC with protobuf, REST/OpenAPI, WebSockets for real-time
- **Patterns:** Microservices, event-driven, CQRS, saga pattern for distributed transactions
- **Observability:** OpenTelemetry (traces + metrics), Prometheus, Grafana, Jaeger, structured JSON logging

**Cloud & Infrastructure**

- **Orchestration:** Kubernetes (EKS, GKE), Helm charts, Kustomize
- **IaC:** Terraform for multi-cloud provisioning, Pulumi
- **Cloud:** AWS (primary -- EC2, EKS, S3, SageMaker), GCP (GKE, Vertex AI)
- **Model Serving:** KServe, Ray Serve, vLLM Operator, Triton
- **GPU Ops:** NVIDIA GPU Operator, DCGM exporter, MIG partitioning, node affinity for GPU types (T4, A10G, A100)
- **GitOps:** ArgoCD for continuous deployment, GitHub Actions for CI

**Data & Storage**

- **Vector DBs:** Weaviate (primary), Qdrant, Pinecone, pgvector -- used for RAG, semantic search, similarity retrieval
- **Databases:** PostgreSQL (OLTP), MongoDB (document store), Redis (caching + session store)
- **Processing:** Kafka Streams for real-time ETL, Apache Airflow for batch orchestration
- **Search:** Elasticsearch for hybrid retrieval (BM25 + dense vectors)

</details>

---

<details open>
<summary><strong>Featured Projects</strong></summary>

<br>

<details>
<summary><strong>Enterprise RAG System</strong> &mdash; Production-grade retrieval-augmented generation platform</summary>

<br>

Production RAG platform designed for accuracy and cost efficiency at scale.

- **Hybrid retrieval pipeline** combining BM25 sparse search with dense vector embeddings, followed by cross-encoder reranking for precision
- **Multi-LLM router** supporting OpenAI, Anthropic, and local models (vLLM) with automatic fallback and cost-aware routing
- **Advanced chunking strategies** -- recursive splitting, semantic chunking, and parent-child document linking for context preservation
- **Evaluation framework** using RAGAS (faithfulness, answer relevancy, context precision) with automated regression testing
- **Semantic caching layer** with Redis to deduplicate similar queries and reduce LLM API costs by ~40%
- **Guardrails** for hallucination detection, PII filtering, and output validation

**Tech:** Python, FastAPI, LangChain, Weaviate, vLLM, Redis, RAGAS

[View Repository →](https://github.com/sanketny8/enterprise-rag-system)

</details>

<details>
<summary><strong>Autonomous LLM Agents</strong> &mdash; Multi-agent orchestration with MCP integration</summary>

<br>

Multi-agent system implementing production agentic AI patterns with tool use and planning.

- **Agent patterns** -- ReAct (reason + act), plan-and-execute with dynamic replanning, reflection loops for self-correction
- **MCP server integration** enabling agents to access external tools (file systems, databases, APIs) through Model Context Protocol
- **Dynamic tool registry** allowing runtime tool discovery, schema validation, and permission-scoped execution
- **Multi-tier memory** -- short-term (conversation buffer), episodic (vector store), and long-term (knowledge graph) for context management
- **Sandboxed execution environment** with Docker containers for safe code execution, resource limits, and state snapshotting
- **Multi-agent communication** using a supervisor pattern with specialized sub-agents for research, coding, and review tasks

**Tech:** Python, LangGraph, MCP, GPT-4, Claude, Weaviate, Docker

[View Repository →](https://github.com/sanketny8/autonomous-llm-agents)

</details>

<details>
<summary><strong>LLM Fine-tuning Platform</strong> &mdash; End-to-end fine-tuning with experiment tracking and deployment</summary>

<br>

Platform for fine-tuning LLMs from dataset preparation to production deployment.

- **Parameter-efficient fine-tuning** with LoRA and QLoRA, supporting 4-bit quantization for training on consumer GPUs
- **Dataset pipeline** -- ingestion, deduplication, quality filtering, instruction formatting (Alpaca, ShareGPT, ChatML)
- **Comprehensive evaluation suite** -- perplexity, BLEU, ROUGE, human-eval, task-specific benchmarks with statistical significance testing
- **Experiment tracking** via MLflow and Weights & Biases -- hyperparameter sweeps, loss curves, GPU utilization monitoring
- **Auto-deployment pipeline** converting fine-tuned checkpoints to vLLM-compatible format with automated A/B testing
- **Multi-GPU training** support through DeepSpeed ZeRO Stage 2/3 for models that don't fit on a single GPU

**Tech:** PyTorch, Transformers, PEFT, DeepSpeed, MLflow, Weights & Biases, vLLM

[View Repository →](https://github.com/sanketny8/llm-finetuning-platform)

</details>

<details>
<summary><strong>AI Gateway Microservices</strong> &mdash; High-performance Go backend for LLM routing and observability</summary>

<br>

Go-based API gateway designed for routing, caching, and observing LLM traffic at scale.

- **Multi-provider routing** with weighted load balancing across OpenAI, Anthropic, and self-hosted models, with automatic failover on errors or latency spikes
- **Semantic caching** using embedding similarity to serve cached responses for semantically equivalent queries, reducing costs
- **Token-based rate limiting** with per-user and per-organization quotas, sliding window counters, and burst allowances
- **Full OpenTelemetry instrumentation** -- request tracing across services, latency histograms, token usage metrics, cost attribution per tenant
- **gRPC inter-service communication** with protobuf schemas, connection pooling, and circuit breakers for downstream service protection
- **Admin dashboard** with real-time metrics, usage analytics, and cost breakdowns per model and per tenant

**Tech:** Go, gRPC, Redis, PostgreSQL, OpenTelemetry, Prometheus, Docker

[View Repository →](https://github.com/sanketny8/ai-gateway-microservices)

</details>

<details>
<summary><strong>GPU Kubernetes Platform</strong> &mdash; Production K8s infrastructure for GPU workloads and model serving</summary>

<br>

Terraform-provisioned Kubernetes platform optimized for GPU-intensive ML workloads.

- **Multi-tier GPU node pools** -- T4 (dev/inference), A10G (fine-tuning), A100 (large-scale training) with workload-aware scheduling
- **Model serving stack** -- KServe for autoscaling inference endpoints, vLLM Operator for LLM-specific serving, Triton for multi-model serving
- **GPU monitoring** via DCGM exporter -- utilization, memory, temperature, power metrics flowing to Prometheus/Grafana dashboards
- **MIG (Multi-Instance GPU) partitioning** on A100s to run multiple smaller models on a single GPU for cost efficiency
- **GitOps workflow** with ArgoCD for declarative cluster state, Helm charts for service packaging, automated rollbacks on health check failures
- **Cost optimization** -- spot instance integration, cluster autoscaler with GPU-aware binpacking, idle GPU detection and scale-down

**Tech:** Terraform, Kubernetes, Helm, ArgoCD, KServe, vLLM Operator, NVIDIA GPU Operator, Prometheus

[View Repository →](https://github.com/sanketny8/gpu-kubernetes-platform)

</details>

<details>
<summary><strong>LLM Engineering Fundamentals</strong> &mdash; Complete transformer from scratch, tokenization to generation</summary>

<br>

Educational implementation building a transformer from the ground up in pure NumPy.

- **BPE tokenizer** implemented from scratch -- byte-pair encoding with vocabulary training, merge rules, and special token handling
- **Positional encodings** -- RoPE (Rotary Position Embeddings) and ALiBi (Attention with Linear Biases) with mathematical derivations
- **Multi-head attention** with causal masking, scaled dot-product, KV caching for efficient autoregressive generation
- **Decoding strategies** -- greedy, beam search (with length normalization), top-k sampling, nucleus (top-p) sampling, temperature scaling
- **Full training loop** with AdamW optimizer, learning rate warmup + cosine decay, gradient clipping, and checkpointing
- **148+ passing tests** across 10 project modules covering tokenization, embeddings, attention, FFN, training, and generation

**Tech:** Python, NumPy (zero external ML dependencies)

[View Repository →](https://github.com/sanketny8/llm-engineering-fundamentals)

</details>

</details>

---

<details>
<summary><strong>Research</strong> &mdash; Exploring attention variants in minimal GPT</summary>

<br>

### Attention Variants in Minimal GPT

Systematic comparison of **6 attention mechanisms** in a zero-dependency GPT implementation (~12K parameters) across 3 rounds of experiments.

**Variants tested:**

- Standard multi-head attention (baseline)
- Gated value attention -- learnable gates on value projections
- Relational scoring -- explicit pairwise token relationship modeling
- Salience weighting -- dynamic importance scoring before softmax
- Context-augmented attention -- global context vector injected into attention computation
- Difference attention -- attention based on token difference vectors

**Key findings:**

- The **gated-context variant** consistently outperformed standard attention on character-level generation (lower loss, faster convergence)
- Salience weighting showed the most improvement on longer sequences but added ~15% overhead
- Difference attention underperformed on small models but may scale better (untested at larger scales)
- All experiments run with identical hyperparameters, seeds, and training data for fair comparison

[Code & Results →](https://github.com/sanketny8/MyProfile)

</details>

---

## Let's Connect

- **Twitter/X:** [@Ny8Sanket](https://twitter.com/Ny8Sanket)
- **LinkedIn:** [ny8sanket](https://linkedin.com/in/ny8sanket)
- **Portfolio:** [sanketny8.github.io](https://sanketny8.github.io)
- **Daily Digest:** [ai-daily-digest](https://github.com/sanketny8/ai-daily-digest) -- auto-curated trending AI papers, repos & blogs

### 🔍 [Enterprise RAG System](https://github.com/sanketny8/enterprise-rag-system)

[![Stars](https://img.shields.io/github/stars/sanketny8/enterprise-rag-system?style=social)](https://github.com/sanketny8/enterprise-rag-system)
[![Forks](https://img.shields.io/github/forks/sanketny8/enterprise-rag-system?style=social)](https://github.com/sanketny8/enterprise-rag-system)

Production-grade **RAG platform** with advanced chunking, hybrid search, and multi-LLM support.

**🎯 Key Features:**
- ⚡ Hybrid retrieval with cross-encoder reranking
- 🔀 Multi-LLM router (OpenAI, Anthropic, local)
- 📊 Comprehensive evaluation (RAGAS)
- 💰 Cost optimization & semantic caching

**🛠️ Tech:** Python • FastAPI • LangChain • Weaviate • vLLM

</td>
<td width="50%">

### 🤖 [Autonomous LLM Agents](https://github.com/sanketny8/autonomous-llm-agents)

[![Stars](https://img.shields.io/github/stars/sanketny8/autonomous-llm-agents?style=social)](https://github.com/sanketny8/autonomous-llm-agents)
[![Forks](https://img.shields.io/github/forks/sanketny8/autonomous-llm-agents?style=social)](https://github.com/sanketny8/autonomous-llm-agents)

Multi-agent system with **agentic AI patterns**, tool use, planning & orchestration.

**🎯 Key Features:**
- 🧠 ReAct pattern with self-reflection
- 🔧 Dynamic tool registry
- 💾 Multi-tier memory system
- 🛡️ Sandboxed execution

**🛠️ Tech:** Python • LangGraph • GPT-4 • Claude • Weaviate

</td>
</tr>

<tr>
<td width="50%">

### 🎓 [LLM Fine-tuning Platform](https://github.com/sanketny8/llm-finetuning-platform)

[![Stars](https://img.shields.io/github/stars/sanketny8/llm-finetuning-platform?style=social)](https://github.com/sanketny8/llm-finetuning-platform)

End-to-end platform for **fine-tuning LLMs** with experiment tracking & deployment.

**🎯 Key Features:**
- 🔧 LoRA/QLoRA fine-tuning
- 📊 Comprehensive evaluation
- 📈 MLflow + W&B tracking
- 🚀 Auto-deployment to vLLM

**🛠️ Tech:** PyTorch • Transformers • PEFT • MLflow • vLLM

</td>
<td width="50%">

### ⚡ [AI Gateway Microservices](https://github.com/sanketny8/ai-gateway-microservices)

[![Stars](https://img.shields.io/github/stars/sanketny8/ai-gateway-microservices?style=social)](https://github.com/sanketny8/ai-gateway-microservices)

High-performance **Go backend** for LLM routing, caching & observability.

**🎯 Key Features:**
- 🔀 Multi-provider routing
- ⚡ Semantic caching
- 🎫 Token-based rate limiting
- 📊 Sub-10ms p99 latency

**🛠️ Tech:** Go • gRPC • Redis • PostgreSQL • OpenTelemetry

</td>
</tr>

<tr>
<td width="50%">

### 🏗️ [GPU Kubernetes Platform](https://github.com/sanketny8/gpu-kubernetes-platform)

[![Stars](https://img.shields.io/github/stars/sanketny8/gpu-kubernetes-platform?style=social)](https://github.com/sanketny8/gpu-kubernetes-platform)

Production **K8s infrastructure** optimized for GPU workloads & model serving.

**🎯 Key Features:**
- 🎮 GPU node pools (T4, A10G, A100)
- 🚀 KServe + vLLM operator
- 📊 DCGM monitoring
- 🔄 GitOps with ArgoCD

**🛠️ Tech:** Terraform • Kubernetes • Helm • ArgoCD • KServe

</td>
<td width="50%">

### 📚 More Projects

**🔗 Explore all my repositories:**

[![GitHub Repos](https://img.shields.io/badge/View%20All%20Repos-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sanketny8?tab=repositories)

**⭐ Additional Projects:**
- Vector DB Benchmarks
- LLM Evaluation Framework
- Prompt Engineering Library
- AI Cost Optimizer

</td>
</tr>
</table>

---

## 📝 Latest Blog Posts

<!-- BLOG-POST-LIST:START -->
<!-- This section is auto-updated by GitHub Actions -->
<!-- BLOG-POST-LIST:END -->

---

## ⚡ Recent GitHub Activity

<!--START_SECTION:activity-->
1. ℹ️ Labeled issue [#1673](https://github.com/fastly/cli/issues/1673) in [fastly/cli](https://github.com/fastly/cli)
<!--END_SECTION:activity-->

---

## 📈 Learning Journey & Current Focus

<div align="center">

### 🎯 Current Focus Areas

![Building](https://img.shields.io/badge/Building-Agentic_Workflows_%7C_Multi--Agent_Systems-8A2BE2?style=flat-square)
![Optimizing](https://img.shields.io/badge/Optimizing-Production_RAG_%7C_Distributed_Systems-FF6E96?style=flat-square)
![Exploring](https://img.shields.io/badge/Exploring-RLHF_%7C_DPO_%7C_Alignment-00D9FF?style=flat-square)
![Researching](https://img.shields.io/badge/Researching-GPU_Cost_Optimization_%7C_System_Design-FFA500?style=flat-square)

<br/>

### 🔬 Research Implementation

![Graph RAG](https://img.shields.io/badge/Graph_RAG-Implemented_✅-success?style=flat-square)
![HyDE](https://img.shields.io/badge/HyDE-Implemented_✅-success?style=flat-square)
![Reflexion](https://img.shields.io/badge/Reflexion-In_Progress_🚧-yellow?style=flat-square)
![Constitutional AI](https://img.shields.io/badge/Constitutional_AI-Planned_📋-blue?style=flat-square)

</div>

### 📚 Continuous Learning

- 🔬 **Experimenting** with cutting-edge techniques (Graph RAG, Corrective RAG, Constitutional AI)
- 📝 **Writing** about lessons learned building GenAI systems at scale
- 🛠️ **Contributing** to open-source AI projects (vLLM, LangChain, Transformers)
- 🎓 **Implementing** recent AI research papers (RAPTOR, HyDE, Reflexion)
- 💬 **Sharing** insights on prompt engineering, RAG optimization, and LLMOps

---

## 🔖 AI Bookmarks

Curated AI resources, tools, and references — open for everyone.

### LLM Courses & Learning
| Resource | Description |
|----------|-------------|
| [LLM Course](https://github.com/mlabonne/llm-course) | Comprehensive course to get into LLMs with roadmaps and Colab notebooks |
| [LLMs from Scratch](https://github.com/rasbt/LLMs-from-scratch) | Implement a ChatGPT-like LLM in PyTorch from scratch |
| [ML Engineering Open Book](https://github.com/stas00/ml-engineering) | ML engineering best practices and infrastructure |
| [Fine-Tuning LLMs Guide](https://arxiv.org/html/2408.13296v1) | Exhaustive review of fine-tuning technologies and best practices |
| [Zero to Mastery PyTorch](https://www.learnpytorch.io/) | Learn PyTorch for deep learning from zero to mastery |
| [Dive into Deep Learning](https://d2l.ai/) | Interactive deep learning book with code, math, and discussions |

### GPU Programming & CUDA
| Resource | Description |
|----------|-------------|
| [LeetGPU](https://leetgpu.com/) | Practice GPU programming with hands-on challenges |
| [100 Days of GPU Programming](https://github.com/julienokumu/100DaysOfGPUProgramming) | Day-by-day GPU programming challenge |
| [GPU Glossary (Modal)](https://modal.com/gpu-glossary/readme) | Comprehensive GPU computing glossary |
| [CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html) | Official NVIDIA CUDA programming guide |
| [PyTorch Internals](https://blog.ezyang.com/2019/05/pytorch-internals/) | Deep dive into PyTorch's internal architecture |
| [Making Deep Learning Go Brrrr](https://horace.io/brrr_intro.html) | First principles GPU performance optimization |

### AI Tools & Inference
| Resource | Description |
|----------|-------------|
| [vLLM](https://github.com/vllm-project/vllm) | High-throughput LLM inference and serving engine |
| [Petals](https://petals.dev/) | Run LLMs at home, BitTorrent-style |
| [turbopuffer](https://turbopuffer.com/) | Fast vector database for search and retrieval |
| [ML Resources](https://ml-resources.vercel.app/) | Curated ML tools and references |
| [Deep-ML](https://www.deep-ml.com/) | Practice platform for ML problems |
| [Modal Blog](https://modal.com/blog) | Engineering blog on serverless GPU infrastructure |

### Agents & Architectures
| Resource | Description |
|----------|-------------|
| [AI Agents for Beginners](https://github.com/microsoft/ai-agents-for-beginners) | Microsoft's open course on building AI agents |
| [LangChain Agents from Scratch](https://github.com/langchain-ai/agents-from-scratch) | Build LLM agents with LangChain/LangGraph |
| [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) | Visual explanation of the Transformer architecture |
| [Berkeley LLM Agents Course](https://rdi.berkeley.edu/llm-agents/f24) | UC Berkeley CS 194/294-196 on LLM Agents |
| [Stanford Self-Improving AI Agents](https://cs329a.stanford.edu/) | Stanford CS329A course |

### Research & Blogs
| Resource | Description |
|----------|-------------|
| [Transformer Inference Arithmetic](https://kipp.ly/transformer-inference-arithmetic/) | Math behind transformer inference performance |
| [Visual Guide to Quantization](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-quantization) | Illustrated quantization guide |
| [StreamingLLM](https://hanlab.mit.edu/blog/streamingllm) | Attention sinks for stable long-context streaming |
| [DeepSeek Papers](https://huggingface.co/collections/Presidentlin/deepseek-papers-674c536aa6acddd9bc98c2ac) | Curated DeepSeek research papers |
| [Sander Dieleman's Blog](https://sander.ai/posts/) | Generative modelling and deep learning research |

### Robotics & Embodied AI
| Resource | Description |
|----------|-------------|
| [LeRobot (Hugging Face)](https://github.com/huggingface/lerobot) | Open-source AI for robotics |
| [Gradient Robotics](https://cheaprobotarm.com/) | Affordable robot arm for experimentation |
| [Awesome LLM Robotics](https://github.com/GT-RIPL/Awesome-LLM-Robotics) | Curated LLM-powered robotics resources |

---

## 📫 Let's Connect!

<div align="center">

### 💬 I'm always open to interesting conversations and collaborations!

![Collaborations](https://img.shields.io/badge/Collaborations-Open_Source_%7C_Research_%7C_Consulting-FF6E96?style=flat-square)
![Discussions](https://img.shields.io/badge/Discussions-System_Design_%7C_Backend_Arch_%7C_LLMs-8A2BE2?style=flat-square)
![Community](https://img.shields.io/badge/Community-Knowledge_Sharing_%7C_Mentorship-00D9FF?style=flat-square)

<br/>

### 🌐 Find Me On

<a href="https://twitter.com/Ny8Sanket">
  <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter" />
</a>
<a href="https://linkedin.com/in/ny8sanket">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
<a href="https://sanketny8.github.io">
  <img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio" />
</a>

<br/><br/>

### 💝 Support My Work

⭐ **Star** repositories you find useful • 📢 **Share** projects with your network • 🤝 **Contribute** to open-source • 💬 **Connect** for collaborations

</div>

---

<div align="center">
  
  **"Building the future of AI, one production system at a time"**
  
  ![Made with Love](https://img.shields.io/badge/Made%20with-❤️-red?style=for-the-badge)
  ![Built for Production](https://img.shields.io/badge/Built%20for-Production-green?style=for-the-badge)
  
  ⭐️ From [sanketny8](https://github.com/sanketny8) with 💜
  
</div>
