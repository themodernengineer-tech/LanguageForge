<div align="center">

# 🧠 LanguageForge

### `ENGINEERING LANGUAGE MODELS FROM TOKENS TO INTELLIGENCE`

Learning how modern language models represent, learn, generate, adapt, and process language.

`TEXT → TOKENS → EMBEDDINGS → ATTENTION → TRANSFORMERS → LLMs`

<br>

![Language Models](https://img.shields.io/badge/Language-Models-blue)
![Transformers](https://img.shields.io/badge/Architecture-Transformers-orange)
![PyTorch](https://img.shields.io/badge/Framework-PyTorch-red)
![Hugging Face](https://img.shields.io/badge/Ecosystem-HuggingFace-yellow)

</div>

---

## 🧭 About LanguageForge

**LanguageForge** is my learning and engineering repository for understanding **Language Models and Large Language Models**, from text representation and Transformer internals to training, post-training, evaluation, and inference.

`📘 NOTES → 💻 CODE → 🧪 EXPERIMENTS → 📊 BENCHMARKS → 🏗️ PROJECTS`

> These are learning domains, not completed skills. The repository evolves as I work through them.

📍 **Learning Path:** [View the complete Language Model Roadmap](ROADMAP.md)

---

## 🧠 Learning Domains

<details>
<summary><b>01 — 🔤 Text Representation & Tokenization</b></summary>

<br>

How raw language becomes numerical input for language models.

`Text & Unicode` · `Vocabulary` · `Tokenization` · `BPE` · `WordPiece` · `SentencePiece` · `Token IDs` · `Special Tokens` · `Padding` · `Truncation` · `Attention Masks`

### 📚 Published Work

| Topic | Artifact |
|---|---|
| Understanding Tokenizers in LLMs | [`understanding_tokenizers.pdf`](Docs/Transformers/understanding_tokenizers.pdf) |

</details>

<details>
<summary><b>02 — 📐 Embeddings & Language Representation</b></summary>

<br>

How discrete tokens become continuous vector representations.

`Token Embeddings` · `Embedding Matrices` · `Vector Representations` · `Embedding Dimensions` · `Cosine Similarity` · `Semantic Relationships` · `Input Embeddings` · `Output Embeddings` · `Weight Tying`

</details>

<details>
<summary><b>03 — 🧮 Neural Language Modeling</b></summary>

<br>

The mathematical and neural foundations behind language prediction.

`Probability` · `Neural Networks` · `Autoregressive Modeling` · `Next-Token Prediction` · `Logits` · `Softmax` · `Cross-Entropy` · `Perplexity` · `Causal Language Modeling`

</details>

<details>
<summary><b>04 — 👁️ Attention & Self-Attention</b></summary>

<br>

How language models dynamically exchange information across tokens.

`Attention` · `Queries` · `Keys` · `Values` · `Scaled Dot-Product Attention` · `Self-Attention` · `Causal Masking` · `Attention Matrices` · `Multi-Head Attention`

</details>

<details>
<summary><b>05 — 🏗️ Transformer Architecture</b></summary>

<br>

How attention, feed-forward networks, residual pathways, and normalization combine into Transformer architectures.

`Transformer Blocks` · `Self-Attention` · `Multi-Head Attention` · `Feed-Forward Networks` · `Residual Connections` · `Normalization` · `Positional Information` · `Encoder` · `Decoder` · `Encoder-Decoder` · `Cross-Attention`

### 📚 Published Work

| Topic | Artifact |
|---|---|
| Transformer Architecture & Self-Attention | [`transformers.pdf`](Docs/Transformers/transformers.pdf) |

</details>

<details>
<summary><b>06 — 🤖 Large Language Model Architecture</b></summary>

<br>

How Transformer components are assembled into modern large language models.

`Decoder-Only Models` · `Causal Attention` · `LM Head` · `Model Depth` · `Model Width` · `RoPE` · `RMSNorm` · `SwiGLU` · `MQA` · `GQA` · `Mixture of Experts`

### 📚 Published Work

| Topic | Artifact |
|---|---|
| What Happens When You Ask an LLM a Question? | [`ask_llm_question.pdf`](Docs/Transformers/ask_llm_question.pdf) |

</details>

<details>
<summary><b>07 — 📚 Pretraining & Data</b></summary>

<br>

How language models learn statistical structure from large text corpora.

`Pretraining Objectives` · `Training Corpora` · `Data Cleaning` · `Filtering` · `Deduplication` · `Tokenization Pipelines` · `Sequence Packing` · `Dataset Mixtures` · `Training Splits` · `Checkpoints` · `Scaling`

</details>

<details>
<summary><b>08 — 📉 LLM Training & Optimization</b></summary>

<br>

How language models are trained efficiently and reliably.

`AdamW` · `Learning Rate` · `Warmup` · `Schedulers` · `Batch Size` · `Gradient Accumulation` · `Gradient Clipping` · `Weight Decay` · `FP32` · `FP16` · `BF16` · `Training Stability`

</details>

<details>
<summary><b>09 — 💬 Instruction Tuning & Post-Training</b></summary>

<br>

How pretrained language models become instruction-following and conversational systems.

`Supervised Fine-Tuning` · `Instruction Data` · `Chat Templates` · `Conversation Formatting` · `Preference Data` · `Reward Modeling` · `RLHF` · `DPO` · `Post-Training`

</details>

<details>
<summary><b>10 — 🔧 Fine-Tuning & PEFT</b></summary>

<br>

How pretrained language models are adapted efficiently to new tasks and domains.

`Full Fine-Tuning` · `PEFT` · `Adapters` · `LoRA` · `Low-Rank Adaptation` · `Target Modules` · `QLoRA` · `Adapter Merging` · `Fine-Tuning Trade-offs`

</details>

<details>
<summary><b>11 — 🎲 Generation & Decoding</b></summary>

<br>

How model logits are transformed into generated language.

`Autoregressive Generation` · `Greedy Decoding` · `Sampling` · `Temperature` · `Top-k` · `Top-p` · `Beam Search` · `Repetition Control` · `Stopping Conditions`

</details>

<details>
<summary><b>12 — 📊 LLM Evaluation</b></summary>

<br>

How language-model quality, capability, and behavior are measured.

`Validation Loss` · `Perplexity` · `Task Metrics` · `Human Evaluation` · `Pairwise Preference` · `Hallucination` · `Robustness` · `Benchmark Contamination` · `Quality Trade-offs`

</details>

<details>
<summary><b>13 — 🚀 LLM Inference & Optimization</b></summary>

<br>

What happens when a trained language model processes prompts and generates tokens.

`Model Loading` · `Prefill` · `Decode` · `TTFT` · `Inter-Token Latency` · `Throughput` · `KV Cache` · `Context Length` · `Quantization` · `Inference Memory` · `Efficient Attention`

</details>

<details>
<summary><b>14 — 🔬 Modern LLM Analysis</b></summary>

<br>

How modern language-model architectures, internal states, and behavior can be systematically investigated.

`Hidden States` · `Attention Weights` · `Token Probabilities` · `Internal Tensors` · `Architecture Comparison` · `Long Context` · `Interpretability` · `Dense Models` · `Mixture of Experts`

</details>

---

<div align="center">

### 🧠 LanguageForge

`TOKENS → ATTENTION → TRANSFORMERS → LANGUAGE MODELS`

**Learning how language becomes computation.**

</div>
