# Awesome-AI-Model-Serving-Inference-Infrastructure

# Top AI Model Serving & Inference Infrastructure Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on High-Throughput LLM Inference Engines, Distributed Model Serving, GPU Kernels, Quantized Local Runtimes & Kubernetes Inference Orchestration*  
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Model Serving & Inference Infrastructure**. These tools maximize tokens-per-second throughput, minimize time-to-first-token (TTFT) latency via PagedAttention, RadixAttention, and FP8/INT4 quantization, and scale multi-model AI inference across consumer GPUs, Apple Silicon, and multi-node Kubernetes clusters.

**Examples** include Groq Cloud, Together AI, Fireworks AI, Baseten, Anyscale, NVIDIA NIM / Lepton AI (formerly OctoAI), vLLM, TensorRT-LLM, DeepSpeed-FastGen, Triton Inference Server, and Lightning-AI/LitServe (the category leaders). 

**Open-source emphasis**: This section is heavily expanded with every major active project for high-throughput LLM serving engines (`vLLM`, `SGLang`, `TensorRT-LLM`, `TGI`), flexible Python/multi-model serving frameworks (`LitServe`, `BentoML`, `Ray Serve`, `Triton`, `KServe`), and portable/edge runtimes (`llama.cpp`, `Ollama`, `MLX`, `ONNX Runtime`) — ideal for MLOps engineers, inference infrastructure architects, and AI researchers.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Groq Cloud](https://groq.com)**  
  Ultra-low-latency AI inference cloud powered by custom Language Processing Units (LPUs) delivering deterministic, high-speed token generation for open-weight models.

- **[Together AI](https://together.ai)**  
  Cloud inference, fine-tuning, and dedicated GPU cluster platform providing sub-second APIs for open-weight LLMs, diffusion models, and custom enterprise deployments.

- **[Fireworks AI](https://fireworks.ai)**  
  High-speed generative AI inference platform engineered for production compound AI systems with custom CUDA kernels, fast structured outputs, and dedicated GPU endpoints.

- **[Baseten](https://baseten.co)**  
  Enterprise ML model deployment and serverless inference infrastructure featuring autoscaling GPU clusters, Truss packaging, and optimized TensorRT-LLM runtimes.

- **[Anyscale](https://anyscale.com)**  
  Managed cloud platform built by the creators of Ray for scaling distributed AI inference, Ray Serve model routing, and fine-tuning across multi-cloud GPU clusters.

- **[NVIDIA NIM & Lepton AI (formerly OctoAI)](https://nvidia.com)**  
  Cloud-native inference microservices and serverless GPU platform offering pre-optimized TensorRT-LLM/vLLM containers and unified APIs for enterprise AI deployment.

- **[Cerebras Inference Cloud](https://cerebras.ai)**  
  Wafer-Scale Engine (`WSE-3`) cloud inference service delivering thousands of tokens per second for large open-weight reasoning and coding models.

- **[SambaNova Cloud](https://sambanova.ai)**  
  Reconfigurable Dataflow Unit (RDU) cloud inference platform providing high-speed serving for large open-source LLMs and multimodal models.

- **[Modal](https://modal.com)**  
  Serverless cloud compute platform enabling AI engineers to deploy custom vLLM, SGLang, and Triton GPU inference endpoints in Python with sub-second cold starts.

- **[Replicate](https://replicate.com)**  
  Developer-centric cloud API and model hub enabling one-line deployment and autoscaling of thousands of open-source language, image, video, and audio models via Cog containers.


## Open-Source GitHub Projects

- **[LitServe (`Lightning-AI/LitServe`)](https://github.com)**  
  Fast, lightweight open-source (`Apache-2.0`) AI model serving engine built on FastAPI by Lightning AI featuring automatic batching, streaming, GPU autoscaling, and multi-model composition.

- **[vLLM (`vllm-project/vllm`)](https://github.com)**  
  Industry-standard open-source (`Apache-2.0`) high-throughput, memory-efficient LLM inference and serving engine powered by PagedAttention, continuous batching, speculative decoding, and FP8/AWQ/GPTQ quantization.

- **[SGLang (`sgl-project/sglang`)](https://github.com)**  
  Blazing-fast open-source (`Apache-2.0`) serving framework for LLMs and VLMs featuring RadixAttention prefix caching, zero-overhead CPU scheduling, and constrained structured decoding.

- **[NVIDIA TensorRT-LLM (`NVIDIA/TensorRT-LLM`)](https://github.com)**  
  Open-source (`Apache-2.0`) library from NVIDIA compiling state-of-the-art LLMs into highly optimized TensorRT engines with custom attention kernels, in-flight batching, and FP8/FP4 quantization.

- **[NVIDIA Triton Inference Server (`triton-inference-server/server`)](https://github.com)**  
  Enterprise-grade open-source (`BSD-3-Clause`) multi-framework inference serving software supporting TensorRT-LLM, vLLM, PyTorch, ONNX Runtime, and dynamic model ensembles on GPUs and CPUs.

- **[DeepSpeed & DeepSpeed-MII (`deepspeedai/DeepSpeed` / `deepspeedai/DeepSpeed-MII`)](https://github.com)**  
  Open-source (`Apache-2.0`) deep learning optimization and low-latency inference suite from Microsoft featuring blocked KV-cache (`DeepSpeed-FastGen`), tensor parallelism, and kernel injection.

- **[Text Generation Inference / TGI (`huggingface/text-generation-inference`)](https://github.com)**  
  Production-ready open-source (`Apache-2.0`) Rust/Python inference server from Hugging Face powering HuggingChat and Inference Endpoints with FlashAttention, PagedAttention, and quantization.

- **[llama.cpp (`ggml-org/llama.cpp`)](https://github.com)**  
  Foundational open-source (`MIT`) C/C++ LLM inference engine enabling quantized GGUF models to run at high speed across CPU, NVIDIA CUDA, Apple Metal, AMD ROCm, and Vulkan hardware.

- **[Ollama (`ollama/ollama`)](https://github.com)**  
  Developer-favorite open-source (`MIT`) local model runner and OpenAI-compatible inference server simplifying GGUF packaging, GPU offloading, and cross-platform model management.

- **[Ray Serve (`ray-project/ray`)](https://github.com)**  
  Scalable open-source (`Apache-2.0`) model-serving library built on Ray for deploying multi-model inference graphs, fractional GPU sharing, and distributed autoscaling clusters.

- **[BentoML (`bentoml/BentoML`) & OpenLLM (`bentoml/OpenLLM`)](https://github.com)**  
  Open-source (`Apache-2.0`) unified inference platform enabling teams to package, compose, and serve open-weight LLMs and custom ML models across Kubernetes and cloud GPUs.

- **[KServe (`kserve/kserve`)](https://github.com)**  
  Cloud-native open-source (`Apache-2.0`) serverless ML and generative AI inference platform on Kubernetes offering scale-to-zero, canary rollouts, and native vLLM/Triton runtimes.

- **[MLX & MLX-LM (`ml-explore/mlx` / `ml-explore/mlx-lm`)](https://github.com)**  
  Apple's open-source (`MIT`) array framework and LLM inference toolkit engineered specifically for unified-memory Apple Silicon (`M1/M2/M3/M4`) chips with 4-bit/8-bit quantization.

- **[ONNX Runtime & ONNX Runtime GenAI (`microsoft/onnxruntime-genai`)](https://github.com)**  
  Cross-platform open-source (`MIT`) high-performance inference engine accelerating generative AI models across NVIDIA GPUs, DirectML Windows PCs, CPUs, and mobile NPUs.

- **[ExLlamaV2 (`turboderp-org/exllamav2`) & Aphrodite Engine (`PygmalionAI/aphrodite-engine`)](https://github.com)**  
  High-speed open-source (`MIT` / `AGPL-3.0`) inference libraries specialized in EXL2 dynamic quantization and ultra-fast single-user and multi-user GPU serving.

- **[LocalAI (`mudler/LocalAI`)](https://github.com)**  
  Self-hosted open-source (`MIT`) drop-in OpenAI API replacement running LLMs, embeddings, voice TTS/STT, and image generation locally on consumer CPUs and GPUs without internet access.

### Additional Strong Open-Source Options

- **[NVIDIA Dynamo (`ai-dynamo/dynamo`)](https://github.com)** and **[Mooncake (`kvcache-ai/Mooncake`)](https://github.com)** for disaggregated prefill/decode distributed inference architectures and KVCache-centric cluster scheduling.
- **[FlashInfer (`flashinfer-ai/flashinfer`)](https://github.com)** and **[FlashAttention (`Dao-AILab/flash-attention`)](https://github.com)** for core open-source CUDA attention kernels powering modern high-throughput LLM serving engines.
- **[ktransformers (`kvcache-ai/ktransformers`)](https://github.com)** and **[AirLLM (`lyogavin/airllm`)](https://github.com)** for CPU/GPU hybrid MoE offloading and layer-wise memory optimization enabling massive 70B–671B models on limited VRAM.
- **[Cog (`replicate/cog`)](https://github.com)** for packaging custom Python/CUDA ML models into standardized, reproducible Docker inference containers.
- **[LiteLLM Proxy (`BerriAI/litellm`)](https://github.com)** and **[TensorZero (`tensorzero/tensorzero`)](https://github.com)** for load-balancing, rate-limiting, and routing traffic across multiple self-hosted inference replicas.
