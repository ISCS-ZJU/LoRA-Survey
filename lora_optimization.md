# LoRA System Optimization Paper Taxonomy

This file categorizes the papers mentioned in our survey **according to the taxonomy used in the paper**.

Source paper: *System Optimization for LoRA in LLMs: Advances, Challenges, and Opportunities*.

---

## ![截屏2026-04-16 15.20.13](/Users/ginko/Library/Application Support/typora-user-images/截屏2026-04-16 15.20.13.png)



## 1. Inference Optimization

### 1.1 Inference-Operator Optimization
- [**Punica: Multi-Tenant LoRA Serving**](https://proceedings.mlsys.org/paper_files/paper/2024/hash/054de805fcceb78a201f5e9d53c85908-Abstract-Conference.html) — Chen et al., 2024
- [**S-LoRA: SERVING THOUSANDS OF CONCURRENT LORA ADAPTERS**](https://proceedings.mlsys.org/paper_files/paper/2024/file/906419cd502575b617cc489a1a696a67-Paper-Conference.pdf) — Sheng et al., 2024
- [**Empower Vision Applications with LoRA LMM(VaLoRA)**](https://dl.acm.org/doi/10.1145/3689031.3717472) — Mi et al., 2025
- [**Dynamic Operator Optimization for Efficient Multi-Tenant LoRA Model Serving(Dop)**](https://ojs.aaai.org/index.php/AAAI/article/view/34453) — Zhou et al., 2025

### 1.2 Scheduling

#### Cluster-level Scheduling
- [**dLoRA: Dynamically Orchestrating Requests and Adapters for LoRA LLM Serving**](https://www.usenix.org/conference/osdi24/presentation/wu-bingyang) — Wu et al., 2024
- [**Toppings: CPU-Assisted, Rank-Aware Adapter Serving for LLM Inference**](https://www.usenix.org/conference/atc25/presentation/li-suyi-toppings) — Li et al., 2025c
- [**Serving Heterogeneous LoRA Adapters in Distributed LLM Inference Systems(LoRAServe)**](https://arxiv.org/abs/2511.22880) — Jaiswal et al., 2025

#### Instance-level Scheduling
- [**dLoRA: Dynamically Orchestrating Requests and Adapters for LoRA LLM Serving**](https://www.usenix.org/conference/osdi24/presentation/wu-bingyang) — Wu et al., 2024
- [**Chameleon: Adaptive Caching and Scheduling for Many-Adapter LLM Inference Environments**](https://dl.acm.org/doi/10.1145/3725843.3756083) — Iliakopoulou et al., 2025
- [**Cannikin: No Lagger of SLO in Concurrent Multiple LoRA LLM Serving**](https://ieeexplore.ieee.org/document/11082562/) — Zhu et al., 2025
- [**Empower Vision Applications with LoRA LMM(VaLoRA)**](https://dl.acm.org/doi/10.1145/3689031.3717472) — Mi et al., 2025

### 1.3 Automatic Parameter Tuning
- [**Data-driven ML approach for maximizing performance in LLM-adapter serving**](https://arxiv.org/abs/2508.08343) — Agullo et al., 2025

### 1.4 Cache Optimization

#### Memory Management
- [**S-LoRA: SERVING THOUSANDS OF CONCURRENT LORA ADAPTERS**](https://proceedings.mlsys.org/paper_files/paper/2024/file/906419cd502575b617cc489a1a696a67-Paper-Conference.pdf) — Sheng et al., 2024
- [**ELORA: Efficient LoRA and KV Cache Management for Multi-LoRA LLM Serving(FASTLIBRA)**](https://cse.hkust.edu.hk/~weiwa/papers/elora-hpca26.pdf) — Zhang et al., 2025a
- [**EdgeLoRA: An Efficient Multi-Tenant LLM Serving System on Edge Devices**](https://dl.acm.org/doi/10.1145/3711875.3729141) — Shen et al., 2025

#### I/O Optimization
- [**Toppings: CPU-Assisted, Rank-Aware Adapter Serving for LLM Inference**](https://www.usenix.org/conference/atc25/presentation/li-suyi-toppings) — Li et al., 2025c
- [**Katz: Efficient Workflow Serving for Diffusion Models with Many Adapters**](https://www.usenix.org/conference/atc25/presentation/li-suyi-katz) — Li et al., 2025d
- [**Rock: Serving Multimodal Models in Cloud with Heterogeneous-Aware Resource Orchestration for Thousands of LoRA Adapters**](https://ieeexplore.ieee.org/abstract/document/11186463) — Wu et al., 2025
- [**LoRATEE: A Secure and Efficient Inference Framework for Multi-Tenant LoRA LLMs Based on TEE**](https://ieeexplore.ieee.org/document/10890445) — Lin et al., 2025b
- [**Serving Heterogeneous LoRA Adapters in Distributed LLM Inference Systems(LoRAServe)**](https://arxiv.org/abs/2511.22880) — Jaiswal et al., 2025

#### KV Cache Reuse
- [**DroidSpeak: KV Cache Sharing Across Fine-tuned Model Variants**](https://www.usenix.org/conference/nsdi26/presentation/liu-yuhan) — Liu et al., 2026
- [**JointSerLoRA: Cache-Aware LoRA Inference Serving**](https://dl.acm.org/doi/10.1109/IWQoS65803.2025.11143270) — Li et al., 2025b
- [**MobiLoRA: Accelerating LoRA-based LLM Inference on Mobile Devices via Context-aware KV Cache Optimization**](https://aclanthology.org/2025.acl-long.1140/) — Li et al., 2025a

#### Parameter Sharing
- [**BlockLLM: Multi-tenant Finer-grained Serving for Large Language Models**](https://arxiv.org/abs/2404.18322) — Hu et al., 2024

### 1.5 Parallel Inference
- [**S-LoRA: SERVING THOUSANDS OF CONCURRENT LORA ADAPTERS**](https://proceedings.mlsys.org/paper_files/paper/2024/file/906419cd502575b617cc489a1a696a67-Paper-Conference.pdf) — Sheng et al., 2024
- [**MixLoRA: An Efficient Multi-Tenant Framework for Concurrently Serving Diverse LoRA Models in Large Language Models**](https://dl.acm.org/doi/10.1145/3754598.3754605) — Chen et al., 2025

---

## 2. Training Optimization

### 2.1 Cloud Training

#### Memory Management
- [**HyC-LoRA: Memory Efficient LoRA Fine-tuning with Hybrid Activation Compression**](https://mlsys.org/virtual/2025/poster/3254) — Wang et al., 2025b
- [**mTuner: Accelerating Parameter-Efficient Fine-Tuning on Multi-GPU Servers with Elastic Tensor**](https://www.usenix.org/conference/atc25/presentation/huang-kezhao) — Huang et al., 2025
- [**Jenga: Enhancing LLM Long-Context Fine-tuning with Contextual Token Sparsity**](https://www.usenix.org/system/files/atc25-wang-tuowei.pdf) — Wang et al., 2025a

#### Training-Operator Optimization
- [**LoRAFusion: A Crossbar-aware Multi-task Adaption Framework via Efficient Fusion of Pretrained LoRA Modules** ](https://dl.acm.org/doi/10.1145/3716368.3735213) Guo et al., 2025
- [**mLoRA: Fine-Tuning LoRA Adapters via Highly-Efficient Pipeline Parallelism in Multiple GPUs**](https://dl.acm.org/doi/abs/10.14778/3725688.3725718) — Ye et al., 2025
- [**PLoRA: Efficient LoRA Hyperparameter Tuning for Large Models**](https://arxiv.org/abs/2508.02932) — Yan et al., 2025

#### Distributed Training Orchestration
- [**mLoRA: Fine-Tuning LoRA Adapters via Highly-Efficient Pipeline Parallelism in Multiple GPUs**](https://dl.acm.org/doi/abs/10.14778/3725688.3725718) — Ye et al., 2025
- [**LoRAFusion: A Crossbar-aware Multi-task Adaption Framework via Efficient Fusion of Pretrained LoRA Modules** ](https://dl.acm.org/doi/10.1145/3716368.3735213) Guo et al., 2025
- [**PLoRA: Efficient LoRA Hyperparameter Tuning for Large Models**](https://arxiv.org/abs/2508.02932) — Yan et al., 202
- [**LobRA: Multi-Tenant Fine-Tuning over Heterogeneous Data**](https://dl.acm.org/doi/abs/10.14778/3742728.3742752) — Lin et al., 2025a
- [**Communication-Efficient MoE Fine-Tuning with Locality-Aware Expert Placement(VELA)**](https://ieeexplore.ieee.org/document/11183830) — Hu et al., 2025

### 2.2 Edge-Cloud Collaborative Training

#### Model Splitting
- [**SplitLoRA: A Split Parameter-Efficient Fine-Tuning Framework for Large Language Models**](https://arxiv.org/abs/2407.00952) — Lin et al., 2024
- [**HSplitLoRA: A Heterogeneous Split Parameter-Efficient Fine-Tuning Framework for Large Language Models**](https://www.computer.org/csdl/journal/tm/5555/01/11474523/2fo8nIVsnE4) — Lin et al., 2025c
- [**SplitLLM: Hierarchical Split Learning for Large Language Model over Wireless Network**](https://ieeexplore.ieee.org/document/11100350/) — Zhang et al., 2025b
- [**Efficient Split Federated Learning for Large Language Models over Communication Networks(SflLLM)**](https://arxiv.org/abs/2504.14667) — Zhao et al., 2025

#### Parameter Scale Adaptation
- [**HSplitLoRA: A Heterogeneous Split Parameter-Efficient Fine-Tuning Framework for Large Language Models**](https://www.computer.org/csdl/journal/tm/5555/01/11474523/2fo8nIVsnE4) — Lin et al., 2025c
- [**SplitLLM: Hierarchical Split Learning for Large Language Model over Wireless Network**](https://ieeexplore.ieee.org/document/11100350/) — Zhang et al., 2025b
- [**Automated Federated Pipeline for Parameter-Efficient Fine-Tuning of Large Language Models(FedPipe)**](https://ieeexplore.ieee.org/document/11320816) — Fang et al., 2024

#### Heterogeneous LoRA Aggregation
- [**FedALT: Federated Fine-Tuning through Adaptive Local Training with Rest-of-World LoRA**](https://ojs.aaai.org/index.php/AAAI/article/view/39054) — Bian et al., 2025
- [**HeLoRA: LoRA-heterogeneous Federated Fine-tuning for Foundation Models**](https://dl.acm.org/doi/10.1145/3723877) — Fan et al., 2025
- [**HSplitLoRA: A Heterogeneous Split Parameter-Efficient Fine-Tuning Framework for Large Language Models**](https://www.computer.org/csdl/journal/tm/5555/01/11474523/2fo8nIVsnE4) — Lin et al., 2025c

---

## 3. Co-Serving Optimization
- [**FlexLLM: Token-Level Co-Serving of LLM Inference and Finetuning with SLO Guarantees**](https://www.usenix.org/conference/nsdi26/presentation/oliaro) — Oliaro et al., 2026
- [**Loquetier: A Virtualized Multi-LoRA Framework for Unified LLM Fine-tuning and Serving**](https://neurips.cc/virtual/2025/loc/san-diego/poster/119974) — Zhang et al., 2025c
- [**Resource Multiplexing in Tuning and Serving Large Language Models(LLMStation)**](https://www.usenix.org/conference/atc25/presentation/he-yongjun) — He et al., 2025
- [**Symbiosis: Multi-Adapter Inference and Fine-Tuning**](https://dl.acm.org/doi/10.1145/3772052.3772230) — Gupta et al., 2025

---

## 4. Same Papers Appearing in Multiple Categories

These papers span multiple system concerns and therefore appear in more than one category.

- **dLoRA** — Cluster-level Scheduling; Instance-level Scheduling
- **S-LoRA** — Inference-Operator Optimization; Memory Management; Parallel Inference
- **VaLoRA** — Inference-Operator Optimization; Instance-level Scheduling
- **Toppings** — Cluster-level Scheduling; I/O Optimization
- **LoRAServe** — Cluster-level Scheduling; I/O Optimization
- **mLoRA** — Training-Operator Optimization; Distributed Training Orchestration
- **LoRAFusion** — Training-Operator Optimization; Distributed Training Orchestration
- **HSplitLoRA** — Model Splitting; Parameter Scale Adaptation; Heterogeneous LoRA Aggregation

---

## 5. Compact Table Version

| Top-level Category | Subcategory | Papers |
|---|---|---|
| Inference | Inference-Operator Optimization | Punica; S-LoRA; VaLoRA; Dop |
| Inference | Cluster-level Scheduling | dLoRA; Toppings; LoRAServe |
| Inference | Instance-level Scheduling | dLoRA; Chameleon; Cannikin; VaLoRA |
| Inference | Automatic Parameter Tuning | Data-driven |
| Inference | Memory Management | S-LoRA; FASTLIBRA; EdgeLoRA |
| Inference | I/O Optimization | Toppings; Katz; Rock; LoRATEE; LoRAServe |
| Inference | KV Cache Reuse | DroidSpeak; JointSerLoRA; MobiLoRA |
| Inference | Parameter Sharing | BlockLLM |
| Inference | Parallel Inference | S-LoRA; MixLoRA |
| Training | Memory Management | HyC-LoRA; mTuner; Jenga |
| Training | Training-Operator Optimization | LoRAFusion; mLoRA; PLoRA |
| Training | Distributed Training Orchestration | mLoRA; LoRAFusion; PLoRA; LobRA; VELA |
| Edge-Cloud Collaborative Training | Model Splitting | SplitLoRA; HSplitLoRA; SplitLLM; SflLLM |
| Edge-Cloud Collaborative Training | Parameter Scale Adaptation | HSplitLoRA; SflLLM; FedPipe |
| Edge-Cloud Collaborative Training | Heterogeneous LoRA Aggregation | FedALT; HeLoRA; HSplitLoRA |
| Co-Serving | Co-Serving Optimization | FlexLLM; Loquetier; LLMStation; Symbiosis |
