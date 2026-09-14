<p align="center">
  <img src="https://img.shields.io/badge/LanguageForge-Language%20Models%20Research%20Lab-6A5ACD?style=for-the-badge">
</p>

<h1 align="center">🔡 LanguageForge</h1>

<p align="center">
  <b>Forging an understanding of Large Language Models — one layer at a time.</b>
</p>

<p align="center">
  <i>
    From tokens and embeddings to Transformers, training, alignment, inference,
    evaluation, and the systems that make modern LLMs work.
  </i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/LLM-Internals-6A5ACD?style=flat-square">
  <img src="https://img.shields.io/badge/Transformers-Architecture-8A2BE2?style=flat-square">
  <img src="https://img.shields.io/badge/Training-Pretraining%20%26%20SFT-0ea5e9?style=flat-square">
  <img src="https://img.shields.io/badge/Alignment-RLHF%20%7C%20DPO-22c55e?style=flat-square">
  <img src="https://img.shields.io/badge/Inference-Efficiency-F97316?style=flat-square">
  <img src="https://img.shields.io/badge/Evaluation-Reliability-EF4444?style=flat-square">
</p>

---

  
## 🔡 What is LanguageForge?



</div>

**LanguageForge** is my self-directed research and learning archive for opening that box.

The repository follows language models from **first principles to modern LLM internals**, studying how text becomes numerical representations, how Transformers process context, how models learn through pretraining, how fine-tuning and alignment modify behavior, and how inference systems turn learned parameters into generated language.

<table>
<tr>
<td width="25%" align="center">

### 🧠 Understand

Architecture
Representations
Attention
Objectives

</td>
<td width="25%" align="center">

### 🏭 Train

Pretraining
Scaling
Fine-Tuning
Alignment

</td>
<td width="25%" align="center">

### ⚡ Infer

Decoding
KV Cache
Quantization
Efficiency

</td>
<td width="25%" align="center">

### 🔬 Evaluate

Quality
Reliability
Failure Modes
Interpretability

</td>
</tr>
</table>

<div align="center">

### The guiding question

## **What actually happens between text going in and intelligence appearing to come out?**

`LANGUAGE → REPRESENTATION → COMPUTATION → PREDICTION → LANGUAGE`

> **LanguageForge studies the model beneath the interface.**

</div>

---

# 🧭 The LLM Learning Forge

The roadmap progresses from first principles toward modern language-model engineering.

Each module is expandable so this README can grow with the repository without becoming a wall of text.

---

<details>
<summary><h2>🧠 Module 01 — Language Model Fundamentals</h2></summary>

<br>

### The starting point: what exactly is a language model?

**Core Concepts**

* What is a Language Model?
* Language Models vs Large Language Models
* Language Models vs Foundation Models
* Statistical language modeling
* Probability of token sequences
* Conditional probability
* Next-token prediction
* Autoregressive generation
* Parameters and model size
* Training vs inference
* Context and context windows
* Temperature intuition
* Why LLMs can generate coherent language
* Capabilities vs limitations of LLMs

### 📚 Articles & Notes

* **01:** 🧾 *“What Happens When You Ask an LLM a Question?”*   📘 [Read PDF](Docs/Transformers/ask_llm_question.pdf)

<br>

</details>

---

<details>
<summary><h2>✂️ Module 02 — Tokenization & Vocabulary</h2></summary>

<br>

### How does human language become something a neural network can process?

**Core Concepts**

* Why models cannot directly process text
* Tokens vs words vs characters
* Token IDs
* Vocabulary construction
* Unknown tokens
* Subword tokenization
* Byte Pair Encoding — BPE
* WordPiece
* Unigram Language Model tokenization
* SentencePiece
* Byte-level tokenization
* Special tokens
* BOS / EOS / PAD tokens
* Encoding and decoding
* Multilingual tokenization
* Vocabulary size trade-offs
* Tokenization efficiency
* Tokenization and context-window usage
* Tokenization and inference cost

### 📚 Articles & Notes

* **01:** 🧾 *“Breaking Language into Pieces: Understanding Tokenizers in LLMs”*   📘 [Read PDF](Docs/Transformers/understanding_tokenizers.pdf)

<br>

</details>

---

<details>
<summary><h2>🧬 Module 03 — Embeddings & Language Representation</h2></summary>

<br>

### How does a model turn discrete tokens into mathematical representations?

**Core Concepts**

* One-hot encoding
* Distributed representations
* Word embeddings
* Word2Vec
* CBOW
* Skip-Gram
* GloVe
* Token embeddings
* Embedding matrices
* Embedding dimensions
* Semantic similarity
* Cosine similarity
* Contextual embeddings
* Static vs contextual embeddings
* Sentence embeddings
* Embedding spaces
* Representation geometry
* Why similar concepts cluster
* Input vs output embeddings
* Weight tying

<br>

</details>

---

<details>
<summary><h2>⏳ Module 04 — Sequence Modeling Before Transformers</h2></summary>

<br>

### What did language modeling look like before attention?

**Core Concepts**

* N-gram language models
* Markov assumptions
* Statistical sequence modeling
* Neural language models
* Recurrent Neural Networks
* Hidden states
* Backpropagation Through Time
* Vanishing gradients
* Exploding gradients
* Long Short-Term Memory — LSTM
* Gated Recurrent Units — GRU
* Bidirectional RNNs
* Sequence-to-sequence models
* Encoder-decoder architecture
* Bottlenecks in recurrent models
* Why recurrence struggles at scale
* Why Transformers replaced RNN-centric architectures

<br>

</details>

---

<details open>
<summary><h2>⚡ Module 05 — Transformer Architecture</h2></summary>

<br>

### The architecture that changed language modeling.

**Core Concepts**

* Transformer overview
* Encoder architecture
* Decoder architecture
* Encoder-decoder Transformers
* Decoder-only Transformers
* Self-attention
* Queries, Keys, and Values
* Attention scores
* Scaled Dot-Product Attention
* Softmax in attention
* Causal masking
* Multi-Head Attention
* Attention heads
* Positional information
* Sinusoidal positional encoding
* Learned positional embeddings
* Rotary Position Embeddings — RoPE
* ALiBi
* Feed-Forward Networks
* Residual connections
* Layer normalization
* Pre-Norm vs Post-Norm
* Transformer blocks
* BERT vs GPT
* Why modern LLMs are predominantly decoder-only

### 📚 Articles & Notes

* **01:** 🧾 *“Transformers Unpacked: The Architecture Behind Modern LLMs”*   📘 [Read PDF](Docs/Transformers/transformers.pdf)

<br>

</details>

---

<details>
<summary><h2>🎯 Module 06 — Attention: Inside the Core Mechanism</h2></summary>

<br>

### A deeper investigation into the mechanism at the heart of Transformers.

**Core Concepts**

* Attention intuition
* Query-Key matching
* Value aggregation
* Q, K, V projection matrices
* Attention matrix
* Attention weights
* Causal attention
* Cross-attention
* Self-attention complexity
* Attention head specialization
* Multi-Query Attention — MQA
* Grouped-Query Attention — GQA
* Multi-Head Attention — MHA
* Local attention
* Sliding-window attention
* Sparse attention
* FlashAttention intuition
* Attention bottlenecks
* Long-context attention

<br>

</details>

---

<details>
<summary><h2>🧮 Module 07 — Language Modeling Objectives</h2></summary>

<br>

### What objective actually teaches a model language?

**Core Concepts**

* Maximum likelihood estimation
* Cross-entropy loss
* Next-token prediction
* Autoregressive language modeling
* Causal language modeling
* Masked language modeling
* Prefix language modeling
* Teacher forcing
* Sequence probability
* Log-likelihood
* Per-token loss
* Perplexity
* BERT-style objectives
* GPT-style objectives
* Objective-function trade-offs

<br>

</details>

---

<details>
<summary><h2>🏭 Module 08 — LLM Pretraining</h2></summary>

<br>

### How does a model learn from massive amounts of text?

**Core Concepts**

* Pretraining pipeline
* Dataset collection
* Data cleaning
* Deduplication
* Data filtering
* Dataset mixtures
* Data quality
* Tokenized datasets
* Sequence packing
* Training batches
* Optimizers
* Adam / AdamW
* Learning-rate schedules
* Warmup
* Gradient accumulation
* Mixed-precision training
* BF16 / FP16
* Gradient clipping
* Checkpointing
* Training stability
* Compute budgets
* Chinchilla-style scaling intuition
* Parameters vs data vs compute
* Scaling laws

<br>

</details>

---

<details>
<summary><h2>📈 Module 09 — Scaling Laws & Model Size</h2></summary>

<br>

### What happens as models, datasets, and compute become larger?

**Core Concepts**

* Parameter scaling
* Dataset scaling
* Compute scaling
* Training FLOPs
* Compute-optimal training
* Kaplan scaling laws
* Chinchilla scaling laws
* Undertraining large models
* Data-to-parameter ratios
* Emergent behavior
* Scaling limitations
* Quality vs compute
* Cost-performance trade-offs
* Dense models
* Mixture-of-Experts intuition

<br>

</details>

---

<details>
<summary><h2>🎓 Module 10 — Fine-Tuning LLMs</h2></summary>

<br>

### Turning a general pretrained model into a specialized model.

**Core Concepts**

* Pretraining vs fine-tuning
* Full fine-tuning
* Supervised Fine-Tuning — SFT
* Instruction tuning
* Instruction datasets
* Prompt-response formatting
* Chat templates
* Domain adaptation
* Task-specific fine-tuning
* Dataset quality
* Training loss
* Validation loss
* Catastrophic forgetting
* Overfitting
* Fine-tuning evaluation


### 📚 Articles & Notes

* **01:** 🧾 *“From General Intelligence to Task Expert: Understanding Fine-Tuning in LLMs”*   📘 [Read PDF](Docs/Transformers/fine_tuning.pdf)

<br>

</details>

---

<details>
<summary><h2>🪶 Module 11 — Parameter-Efficient Fine-Tuning</h2></summary>

<br>

### How can massive models be adapted without retraining every parameter?

**Core Concepts**

* Why full fine-tuning is expensive
* Parameter-Efficient Fine-Tuning — PEFT
* Adapter methods
* Low-Rank Adaptation — LoRA
* Rank decomposition
* LoRA rank
* Alpha scaling
* Target modules
* Adapter merging
* Quantization-aware adaptation
* QLoRA
* 4-bit training
* NF4
* Memory savings
* Accuracy trade-offs
* Full fine-tuning vs LoRA vs QLoRA

<br>

</details>

---

<details>
<summary><h2>🤝 Module 12 — Alignment & Preference Learning</h2></summary>

<br>

### How does a pretrained model become a useful assistant?

**Core Concepts**

* What is alignment?
* Instruction following
* Human preferences
* Supervised Fine-Tuning
* Reward models
* Reinforcement Learning from Human Feedback — RLHF
* PPO intuition
* Preference datasets
* Direct Preference Optimization — DPO
* DPO vs RLHF
* Constitutional approaches
* Alignment tax
* Reward hacking
* Over-optimization
* Helpfulness
* Harmlessness
* Alignment limitations

<br>

</details>

---

<details>
<summary><h2>🎲 Module 13 — Decoding & Text Generation</h2></summary>

<br>

### Once the model predicts probabilities, how is the next token actually chosen?

**Core Concepts**

* Logits
* Softmax
* Probability distributions
* Greedy decoding
* Temperature
* Top-K sampling
* Top-P / nucleus sampling
* Min-P intuition
* Beam search
* Repetition penalties
* Frequency penalties
* Stop tokens
* EOS handling
* Deterministic vs stochastic generation
* Sampling trade-offs
* Generation quality
* Structured generation

<br>

</details>

---

<details>
<summary><h2>🚀 Module 14 — LLM Inference</h2></summary>

<br>

### What happens after training when a model serves real requests?

**Core Concepts**

* Training vs inference
* Prefill phase
* Decode phase
* Autoregressive inference
* KV cache
* KV-cache memory
* Time to First Token — TTFT
* Time per Output Token — TPOT
* Inter-Token Latency — ITL
* Throughput
* Requests per second
* Tokens per second
* Batch inference
* Dynamic batching
* Continuous batching
* Memory bandwidth
* Compute-bound vs memory-bound operations
* GPU utilization
* Inference bottlenecks
* Latency-throughput trade-offs

<br>

</details>

---

<details>
<summary><h2>⚙️ Module 15 — Efficient LLM Inference</h2></summary>

<br>

### How do inference engines make large models faster and cheaper?

**Core Concepts**

* Inference engines
* Model serving architecture
* PagedAttention
* Continuous batching
* KV-cache management
* Prefix caching
* Chunked prefill
* Speculative decoding
* Tensor parallelism
* Pipeline parallelism
* Data parallel inference
* Quantized inference
* Kernel optimization
* CUDA kernels
* FlashAttention
* vLLM concepts
* TensorRT-LLM concepts
* Throughput optimization
* Latency optimization

<br>

</details>

---

<details>
<summary><h2>📦 Module 16 — Quantization & Model Compression</h2></summary>

<br>

### How can large models consume less memory and compute?

**Core Concepts**

* Numerical precision
* FP32
* FP16
* BF16
* INT8
* INT4
* Weight quantization
* Activation quantization
* Post-Training Quantization — PTQ
* Quantization-Aware Training — QAT
* GPTQ
* AWQ
* GGUF concepts
* Calibration
* Memory reduction
* Accuracy degradation
* Quantization vs throughput
* Quantization vs latency

<br>

</details>

---

<details>
<summary><h2>🧠 Module 17 — Context Windows & Long-Context LLMs</h2></summary>

<br>

### What does it actually mean for a model to have context?

**Core Concepts**

* Context windows
* Sequence length
* Attention complexity
* Position representations
* RoPE
* Context extension
* Sliding-window attention
* Long-context training
* Lost-in-the-middle behavior
* Context utilization
* KV-cache growth
* Memory requirements
* Long-context inference cost
* Context compression
* Long-context evaluation

<br>

</details>

---

<details>
<summary><h2>🧩 Module 18 — Mixture of Experts</h2></summary>

<br>

### Can a model have enormous capacity without activating every parameter?

**Core Concepts**

* Dense vs sparse models
* Mixture of Experts — MoE
* Experts
* Routing networks
* Top-K routing
* Sparse activation
* Active parameters
* Total parameters
* Load balancing
* Expert capacity
* Communication overhead
* Expert parallelism
* Training MoE models
* MoE inference
* Efficiency trade-offs

<br>

</details>

---

<details>
<summary><h2>🔬 Module 19 — LLM Evaluation</h2></summary>

<br>

### How do we know whether a language model is actually good?

**Core Concepts**

* Evaluation methodology
* Training vs validation vs test sets
* Perplexity
* Exact match
* F1
* BLEU
* ROUGE
* Benchmark evaluation
* MMLU-style evaluation
* Reasoning benchmarks
* Code benchmarks
* Human evaluation
* LLM-as-a-judge
* Pairwise evaluation
* Elo-style ranking
* Evaluation contamination
* Benchmark saturation
* Domain-specific evaluation
* Regression testing
* Statistical significance

<br>

</details>

---

<details>
<summary><h2>🛡️ Module 20 — Reliability, Hallucinations & Failure Modes</h2></summary>

<br>

### Where do language models fail — and why?

**Core Concepts**

* Hallucinations
* Factuality
* Calibration
* Confidence vs correctness
* Distribution shift
* Prompt sensitivity
* Context failures
* Reasoning failures
* Repetition
* Degeneration
* Knowledge limitations
* Temporal limitations
* Bias
* Robustness
* Adversarial inputs
* Failure-mode analysis
* Reliability evaluation

<br>

</details>

---

<details>
<summary><h2>🔭 Module 21 — Modern LLM Architecture Patterns</h2></summary>

<br>

### How are contemporary language models evolving beyond the original Transformer?

**Core Concepts**

* Decoder-only architectures
* RMSNorm
* SwiGLU
* RoPE
* Grouped-Query Attention
* Multi-Query Attention
* Sliding-window attention
* Sparse attention
* Mixture of Experts
* Shared experts
* Attention variants
* State-space model intuition
* Hybrid architectures
* Architectural efficiency
* Memory-efficient architectures
* Modern design trade-offs

<br>

</details>

---

<details>
<summary><h2>🔎 Module 22 — Interpretability & Understanding Model Behavior</h2></summary>

<br>

### Can we understand what happens inside billions of learned parameters?

**Core Concepts**

* Black-box behavior
* Neural representations
* Feature visualization
* Attention visualization
* Probing
* Activation analysis
* Logit lens intuition
* Sparse autoencoders
* Superposition
* Feature circuits
* Mechanistic interpretability
* Representation analysis
* Model internals
* Interpretability limitations

<br>

</details>

---

<details>
<summary><h2>🏗️ Module 23 — LLM Systems Thinking</h2></summary>

<br>

### Connecting model architecture with the systems required to run it.

**Core Concepts**

* Model architecture ↔ hardware
* Parameter count ↔ memory
* Precision ↔ memory footprint
* Tokens ↔ compute
* Context length ↔ KV cache
* Batch size ↔ throughput
* GPU memory ↔ model capacity
* Memory bandwidth ↔ decoding performance
* Parallelism ↔ scaling
* Quantization ↔ deployment
* Latency ↔ user experience
* Throughput ↔ serving economics
* Model quality ↔ infrastructure cost
* Training architecture vs inference architecture

> This module forms the bridge between **LanguageForge** and my AI infrastructure studies in **InfraNerve**.

<br>

</details>

---

# 🧰 Tools & Frameworks

<div align="center">

<img src="https://skillicons.dev/icons?i=python,pytorch,tensorflow" />

<br><br>

<img src="https://img.shields.io/badge/Hugging%20Face-Transformers-FFD21E?style=flat-square">
<img src="https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=flat-square&logo=jupyter&logoColor=white">
<img src="https://img.shields.io/badge/vLLM-Inference-4B8BBE?style=flat-square">
<img src="https://img.shields.io/badge/PEFT-LoRA%20%7C%20QLoRA-8A2BE2?style=flat-square">

</div>

---

# 📌 The LanguageForge Principle

<div align="center">

```text id="r19tdh"
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                     DON'T JUST ASK THE MODEL                     │
│                              │                                  │
│                              ▼                                  │
│                   ASK HOW THE MODEL WORKS                       │
│                              │                                  │
│             ┌────────────────┼────────────────┐                 │
│             ▼                ▼                ▼                 │
│         STRUCTURE         LEARNING         BEHAVIOR             │
│             │                │                │                 │
│             ▼                ▼                ▼                 │
│       Transformers       Training          Inference            │
│       Attention          Alignment         Evaluation           │
│             │                │                │                 │
│             └────────────────┼────────────────┘                 │
│                              ▼                                  │
│                       UNDERSTANDING                             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### **LanguageForge is not a collection of LLM buzzwords.**

It is a growing record of my attempt to answer one question:

## **“What actually happens between text going in and intelligence appearing to come out?”**

<br>

`TEXT → TOKENS → VECTORS → ATTENTION → PREDICTION → LANGUAGE`

<br>

> **Don't stop at the output. Trace the computation.**

---

⭐ **Maintained by Kartik Saroop**

*Learning Language Models from first principles to modern LLM internals.*

</div>
