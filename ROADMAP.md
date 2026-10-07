<div align="center">

# 🧭 LanguageForge Roadmap

### `ENGINEERING LANGUAGE MODELS FROM FIRST PRINCIPLES TO PRODUCTION`

A chronological engineering journey through how modern language models represent text, learn patterns, generate language, adapt to instructions, retrieve knowledge, use tools, scale across hardware, and operate in production.

`TEXT → TOKENS → REPRESENTATIONS → ATTENTION → TRANSFORMERS → TRAINING → GENERATION → POST-TRAINING → EVALUATION → INFERENCE → RAG → SERVING → PRODUCTION`

</div>

---

# 🎯 How to Use This Roadmap

LanguageForge follows a **chronological, prerequisite-driven path**.

Each phase uses a standard technical topic as its title.

Inside the phase, questions drive the actual learning:

```text
TECHNICAL DOMAIN
      ↓
QUESTIONS TO ANSWER
      ↓
CONCEPTS TO STUDY
      ↓
DOCUMENTATION
      ↓
IMPLEMENTATION / INVESTIGATION
      ↓
BENCHMARK / PROJECT
      ↓
EVIDENCE + CONCLUSIONS
```

Artifact types:

```text
📘 DOCUMENTATION
Explain one coherent engineering question or tightly coupled subsystem.

💻 IMPLEMENTATION
Rebuild an important mechanism to understand how it works.

🧪 INVESTIGATION
Answer a technical question experimentally.

📊 BENCHMARK
Compare measurable quality, latency, memory, throughput, or scaling.

🏗️ PROJECT
Combine multiple concepts into a reusable engineering artifact.

🔬 FAILURE STUDY
Deliberately create controlled failures and diagnose them.

📋 RUNBOOK
Document operational diagnosis, mitigation, and recovery.
```

Not every phase requires every artifact type.

---

# 📍 Progress Tracker

| # | Phase | Status |
|---:|---|:---:|
| 01 | 🧠 Language Model Fundamentals | ⬜ |
| 02 | 🧮 Mathematics for Language Models | ⬜ |
| 03 | 🐍 Python, NumPy & PyTorch Foundations | ⬜ |
| 04 | 🔤 Text Representation, Unicode & UTF-8 | ⬜ |
| 05 | ✂️ Tokenization Fundamentals | ⬜ |
| 06 | 🧩 Tokenization Algorithms & Vocabulary Design | ⬜ |
| 07 | 🔢 Transformer Inputs, Batching & Masking | ⬜ |
| 08 | 📐 Token Embeddings & Representation | ⬜ |
| 09 | 🧠 Neural Network Foundations | ⬜ |
| 10 | 📖 Autoregressive Language Modeling | ⬜ |
| 11 | 👁️ Attention Fundamentals | ⬜ |
| 12 | ⚡ Self-Attention & Causal Attention | ⬜ |
| 13 | 🧠 Multi-Head Attention | ⬜ |
| 14 | 📍 Positional Encoding & RoPE | ⬜ |
| 15 | 🏗️ Transformer Block Architecture | ⬜ |
| 16 | 🔄 Transformer Architecture Families | ⬜ |
| 17 | 🤖 Decoder-Only LLM Architecture | ⬜ |
| 18 | 🎲 Autoregressive Generation & Decoding | ⬜ |
| 19 | 🏗️ Language Model From Scratch | ⬜ |
| 20 | 📚 LLM Pretraining | ⬜ |
| 21 | 🗃️ LLM Data Engineering | ⬜ |
| 22 | 📉 Training Optimization & Stability | ⬜ |
| 23 | ⚡ Training Precision & GPU Memory | ⬜ |
| 24 | 🌐 Distributed LLM Training | ⬜ |
| 25 | 💾 Checkpointing & Training Recovery | ⬜ |
| 26 | 💬 Instruction Tuning & Chat Models | ⬜ |
| 27 | 🔧 Fine-Tuning, LoRA & PEFT | ⬜ |
| 28 | 🎯 Preference Alignment & DPO | ⬜ |
| 29 | 📊 LLM Evaluation | ⬜ |
| 30 | 🚀 LLM Inference Fundamentals | ⬜ |
| 31 | 💾 KV Cache & Generation Memory | ⬜ |
| 32 | 📦 Quantization & Model Compression | ⬜ |
| 33 | ⚡ Efficient Attention | ⬜ |
| 34 | 🧬 Modern LLM Architecture Patterns | ⬜ |
| 35 | 🧩 Mixture of Experts | ⬜ |
| 36 | 📏 Long-Context Language Models | ⬜ |
| 37 | 🔎 Retrieval-Augmented Generation | ⬜ |
| 38 | 🛠️ Tool Use & Agent Fundamentals | ⬜ |
| 39 | 🌐 LLM Serving | ⬜ |
| 40 | 📦 Batching, Scheduling & Serving Performance | ⬜ |
| 41 | 📊 LLM Observability | ⬜ |
| 42 | 🔐 LLM Application Security | ⬜ |
| 43 | 🩺 LLM Reliability & Troubleshooting | ⬜ |
| 44 | 🏭 Production LLM Systems | ⬜ |

`⬜ Planned` · `🟡 In Progress` · `✅ Completed`

---

# PART I — FOUNDATIONS

<details>
<summary><b>Phase 01 — 🧠 Language Model Fundamentals</b></summary>

### 🎯 Objective

Build the mental model required for everything that follows.

### ❓ Questions to Answer

#### 1. What is a language model predicting?

Study:

`Language Modeling` · `Sequences` · `Tokens` · `Vocabulary` · `Conditional Probability` · `Next-Token Prediction`

#### 2. How can repeatedly predicting one token produce paragraphs?

Study:

`Autoregression` · `Context` · `Logits` · `Probability Distribution` · `Token Selection`

#### 3. What exactly is stored inside a trained model?

Study:

`Parameters` · `Weights` · `Model Configuration` · `Checkpoint`

#### 4. What changes during training but remains fixed during inference?

Study:

`Forward Pass` · `Loss` · `Backpropagation` · `Parameter Updates` · `Inference`

#### 5. What happens between receiving a prompt and returning generated text?

Study:

`Prompt` · `Tokenizer` · `Token IDs` · `Embeddings` · `Transformer` · `Logits` · `Decoding`

### 📖 Sources to Study

- Jurafsky & Martin — *Speech and Language Processing*
- Hugging Face LLM Course
- Hugging Face Transformers documentation

### 📘 Documentation Plan

#### `language_model_fundamentals.pdf`

**Question:** What does a language model learn?

**Cover Together**

`Language Modeling` · `Sequences` · `Tokens` · `Vocabulary` · `Conditional Probability` · `Next-Token Prediction` · `Autoregression` · `Context` · `Parameters`

**Do Not Include**

Transformer internals, attention equations, tokenizer algorithms, or optimization.

#### `training_vs_inference.pdf`

**Question:** What changes between learning a model and using one?

**Cover Together**

`Forward Pass` · `Loss` · `Backward Pass` · `Parameter Updates` · `Checkpoints` · `Frozen Parameters`

#### `llm_request_lifecycle.pdf`

**Question:** What happens when a user asks an LLM a question?

**Cover Together**

`PROMPT → TOKENIZATION → TOKEN IDs → EMBEDDINGS → TRANSFORMER → LOGITS → DECODING → TEXT`

Keep this document architectural rather than mathematical.

### 🧪 Investigation — **PromptPerturb: Next-Token Probability Investigation with Python, PyTorch & Hugging Face Transformers**

**Research Question**

How much can a small prompt modification alter the model's next-token probability distribution?

**Build**

Create:

```text
Labs/Foundations/promptperturb/
├── README.md
├── analyze.py
└── results/
```

**Tools**

`Python` · `PyTorch` · `Hugging Face Transformers`

**Steps**

1. Load a small causal language model.
2. Tokenize a prompt.
3. Run one forward pass.
4. Extract the final token-position logits.
5. Apply softmax.
6. Display the top 10 candidates.
7. Modify one part of the prompt.
8. Repeat.
9. Compare probability changes.

Test:

```text
The capital of France is
The capital of France was
The capital of France might be
The capital of France is definitely
```

**Record**

```text
prompt
input tokens
top-10 predicted tokens
probabilities
probability change
```

### ✅ Exit Criteria

- [ ] Explain next-token prediction.
- [ ] Explain autoregressive generation.
- [ ] Distinguish training and inference.
- [ ] Trace a prompt through the high-level LLM pipeline.

</details>

<details>
<summary><b>Phase 02 — 🧮 Mathematics for Language Models</b></summary>

### 🎯 Objective

Learn the mathematics required to understand later LLM mechanisms.

### ❓ Questions to Answer

#### 1. Why are model representations vectors and matrices?

Study:

`Scalars` · `Vectors` · `Matrices` · `Tensors` · `Dimensions` · `Shapes`

#### 2. Why does matrix multiplication appear throughout Transformers?

Study:

`Dot Product` · `Matrix Multiplication` · `Transpose` · `Linear Transformations`

#### 3. How do arbitrary scores become probabilities?

Study:

`Logits` · `Exponentials` · `Softmax`

#### 4. How is prediction error measured?

Study:

`Logarithms` · `Entropy` · `Cross-Entropy` · `KL Divergence`

#### 5. How can output error modify earlier parameters?

Study:

`Derivatives` · `Partial Derivatives` · `Chain Rule` · `Gradients`

### 📖 Sources to Study

- 3Blue1Brown — Linear Algebra
- Dive into Deep Learning
- PyTorch Tensor documentation

### 📘 Documentation Plan

#### `linear_algebra_for_language_models.pdf`

Cover together:

`Vectors` · `Matrices` · `Tensors` · `Shapes` · `Dot Products` · `Transpose` · `Matrix Multiplication` · `Norms`

#### `probability_and_information_theory_for_llms.pdf`

Cover together:

`Probability` · `Conditional Probability` · `Logits` · `Softmax` · `Entropy` · `Cross-Entropy` · `KL Divergence`

#### `gradients_and_learning_math.pdf`

Cover together:

`Derivatives` · `Partial Derivatives` · `Chain Rule` · `Gradients` · `Gradient Descent`

Do not include AdamW or distributed optimization.

### 💻 Implementation — **MathCore: LLM Mathematical Operations From Scratch with Python & NumPy**

Implement:

```python
dot_product()
matrix_multiply()
stable_softmax()
cross_entropy()
```

Then validate against NumPy and PyTorch equivalents.

### 🧪 Investigation — **SoftmaxUnderPressure: Numerical Stability & Temperature Experiment with NumPy and PyTorch**

Test increasingly large logits.

Compare:

```text
naive softmax
numerically stable softmax
```

Then test:

```text
temperature = 0.25
temperature = 0.5
temperature = 1.0
temperature = 2.0
temperature = 4.0
```

Measure changes in probability concentration and entropy.

### 📦 Artifacts

```text
Code/Foundations/mathcore/
Labs/Foundations/softmax-under-pressure/
```

### ✅ Exit Criteria

- [ ] Calculate tensor dimensions correctly.
- [ ] Implement stable softmax.
- [ ] Explain cross-entropy.
- [ ] Explain gradient-based learning.

</details>

<details>
<summary><b>Phase 03 — 🐍 Python, NumPy & PyTorch Foundations</b></summary>

### 🎯 Objective

Develop the tensor-programming skills required for Transformer implementation.

### ❓ Questions to Answer

#### 1. How do Python, NumPy, and PyTorch represent numerical data differently?

Study:

`Python Collections` · `NumPy Arrays` · `PyTorch Tensors`

#### 2. How do tensor dimensions represent batches, tokens, heads, and hidden dimensions?

Study:

`Shape` · `Reshape` · `View` · `Transpose` · `Permute`

#### 3. How does PyTorch calculate gradients?

Study:

`Autograd` · `Computation Graph` · `requires_grad` · `.backward()`

#### 4. What makes an object a trainable PyTorch model?

Study:

`nn.Module` · `Parameter` · `state_dict` · `train()` · `eval()`

### 📖 Sources to Study

- Python documentation
- NumPy documentation
- PyTorch tutorials
- PyTorch API documentation

### 📘 Documentation Plan

#### `python_numpy_for_llm_engineering.pdf`

Cover:

`Python Data Structures` · `Functions` · `Classes` · `NumPy Arrays` · `Vectorized Operations`

Keep this concise if Python is already familiar.

#### `pytorch_tensor_fundamentals.pdf`

Cover:

`Tensor Creation` · `Shapes` · `Indexing` · `Broadcasting` · `Reshape` · `Transpose` · `dtype` · `device`

#### `pytorch_autograd_and_modules.pdf`

Cover:

`Autograd` · `Computation Graph` · `Gradients` · `nn.Module` · `Parameters` · `state_dict`

### 💻 Implementation — **TensorGym: Transformer Tensor-Shape Exercises with Python & PyTorch**

Create:

```python
B = 2
T = 8
C = 64
H = 4
D = C // H
```

Transform:

```text
[B,T,C]
→ [B,T,H,D]
→ [B,H,T,D]
→ [B,H,T,T]
→ [B,H,T,D]
→ [B,T,C]
```

Assert every expected shape.

### 🧪 Investigation — **GradientTrace: Neural Gradient Inspection Experiment with PyTorch Autograd**

Build a two-layer network.

Record per step:

```text
loss
parameter
gradient
gradient norm
parameter after optimizer step
```

### 📦 Artifacts

```text
Labs/PyTorch/tensor-gym/
Labs/PyTorch/gradient-trace/
```

### ✅ Exit Criteria

- [ ] Manipulate `[B,T,C]` tensors.
- [ ] Explain broadcasting.
- [ ] Inspect gradients.
- [ ] Build and save an `nn.Module`.

</details>

<details>
<summary><b>Phase 04 — 🔤 Text Representation, Unicode & UTF-8</b></summary>

### 🎯 Objective

Understand how text exists computationally before tokenization.

### ❓ Questions to Answer

#### 1. Is a character the same as a byte?

Study:

`Characters` · `Code Points` · `Bytes`

#### 2. Why can visually similar strings have different representations?

Study:

`Unicode` · `UTF-8` · `Normalization`

#### 3. Why do different characters require different numbers of bytes?

Study:

`Variable-Length Encoding`

#### 4. Why can't a model simply create one vocabulary item for every word?

Study:

`Word Vocabulary` · `Character Vocabulary` · `Byte Vocabulary` · `Vocabulary Explosion`

### 📖 Sources to Study

- Unicode Standard
- Python Unicode HOWTO

### 📘 Documentation Plan

#### `text_unicode_and_utf8.pdf`

Cover together:

`Characters` · `Code Points` · `Unicode` · `UTF-8` · `Bytes` · `Normalization`

#### `language_model_vocabulary_problem.pdf`

Cover:

`Words` · `Characters` · `Bytes` · `Vocabulary Size` · `Unknown Words` · `Subword Motivation`

### 🧪 Investigation — **ByteLens: Multilingual Unicode & UTF-8 Representation Explorer with Python**

Build a CLI:

```bash
python inspect.py "café"
```

Display:

```text
original text
characters
Unicode code points
UTF-8 bytes
character count
byte count
```

Test:

`English` · `Arabic` · `Hindi` · `Chinese` · `Japanese` · `Emoji` · `Code` · `Combining Characters`

### 📦 Artifact

```text
Labs/Text/bytelens/
```

### ✅ Exit Criteria

- [ ] Distinguish characters, code points, and bytes.
- [ ] Explain UTF-8.
- [ ] Explain why vocabulary design is necessary.

</details>

---

# PART II — TOKENIZATION & REPRESENTATION

<details>
<summary><b>Phase 05 — ✂️ Tokenization Fundamentals</b></summary>

### 🎯 Objective

Understand how raw text becomes discrete model input.

### ❓ Questions to Answer

#### 1. Why can't an LLM simply read words directly?

Study:

`Vocabulary` · `Open Vocabulary Problem` · `Subwords` · `Token IDs`

#### 2. Why can comparable information require different token counts?

Study:

`Token Boundaries` · `Vocabulary Coverage` · `Whitespace` · `Numbers` · `Code` · `Multilingual Text`

#### 3. What happens between raw text and `input_ids`?

Study:

`Normalization` · `Pre-Tokenization` · `Tokenizer Model` · `Post-Processing` · `Encoding`

#### 4. Why are special tokens necessary?

Study:

`BOS` · `EOS` · `PAD` · `UNK` · `Control Tokens`

#### 5. Can tokenizer design make some languages more expensive?

Study:

`Tokens/Character` · `Bytes/Token` · `Context Consumption`

### 📖 Sources to Study

- Hugging Face Tokenizers
- Hugging Face Transformers tokenizer documentation

### 📘 Documentation Plan

#### `tokenization_fundamentals.pdf`

Cover:

`Tokens` · `Vocabulary` · `Token IDs` · `Encoding` · `Decoding` · `Subword Motivation`

#### `tokenizer_processing_pipeline.pdf`

Cover:

`Normalization → Pre-Tokenization → Tokenizer Model → Post-Processing → IDs`

#### `special_tokens_padding_and_truncation.pdf`

Cover:

`BOS` · `EOS` · `PAD` · `UNK` · `Control Tokens` · `Padding` · `Truncation`

Do not include BPE training algorithms.

### 🏗️ Project — **TokenLens: Multilingual Tokenization Efficiency Analyzer with Python, Hugging Face Transformers, Pandas & Matplotlib**

**Problem**

Measure how efficiently different tokenizers represent different languages and workloads.

Test:

```text
English
French
Spanish
Arabic
Hindi
Chinese
Japanese
emoji
Python
JavaScript
JSON
URLs
UUIDs
numbers
```

For every sample:

```text
characters
UTF-8 bytes
tokens
characters/token
bytes/token
tokenizer
content type
```

Generate:

```text
CSV results
token-count comparison charts
characters/token charts
language comparison charts
code vs prose comparison
```

### 📦 Artifact

```text
Projects/tokenlens/
├── README.md
├── benchmark.py
├── datasets/
├── results/
└── plots/
```

### ✅ Exit Criteria

- [ ] Explain the tokenizer pipeline.
- [ ] Inspect token IDs.
- [ ] Measure tokenizer efficiency.
- [ ] Explain tokenization's effect on cost and context.

</details>

<details>
<summary><b>Phase 06 — 🧩 Tokenization Algorithms & Vocabulary Design</b></summary>

### 🎯 Objective

Understand how subword vocabularies are learned.

### ❓ Questions to Answer

#### 1. How can frequent character sequences become reusable tokens?

Study:

`BPE` · `Pair Frequencies` · `Merge Rules`

#### 2. Why are multiple tokenizer algorithms used?

Study:

`BPE` · `Byte-Level BPE` · `WordPiece` · `Unigram` · `SentencePiece`

#### 3. What changes when vocabulary size increases?

Study:

`Sequence Length` · `Embedding Parameters` · `Coverage`

#### 4. How does tokenizer training data influence the vocabulary?

Study:

`Corpus Distribution` · `Language Coverage` · `Domain Coverage`

### 📖 Sources to Study

- Hugging Face Tokenizers
- SentencePiece
- tokenizer algorithm papers

### 📘 Documentation Plan

#### `bpe_and_byte_level_bpe.pdf`

Cover:

`Initial Symbols` · `Pair Counting` · `Merging` · `Merge Rules` · `Encoding` · `Byte-Level BPE`

#### `wordpiece_unigram_and_sentencepiece.pdf`

Cover:

`WordPiece` · `Unigram` · `SentencePiece` · `Algorithm Differences`

#### `tokenizer_vocabulary_engineering.pdf`

Cover:

`Training Corpus` · `Vocabulary Size` · `Coverage` · `Special Tokens` · `Sequence-Length Trade-offs`

### 💻 Implementation — **MergeCraft: Byte Pair Encoding Tokenizer From Scratch with Python**

Implement:

```python
build_initial_vocab()
count_pairs()
find_best_pair()
merge_pair()
train()
encode()
decode()
```

Do not use a tokenizer library for the core algorithm.

### 📊 Benchmark — **VocabScale: Tokenizer Vocabulary-Size Benchmark with Python, Hugging Face Tokenizers, Pandas & Matplotlib**

Train:

```text
1K
2K
4K
8K
```

vocabularies on the same corpus.

Measure:

```text
training time
average tokens/document
characters/token
vocabulary size
implied embedding parameters
```

Add the trained tokenizers to TokenLens.

### 📦 Artifacts

```text
Code/Tokenization/mergecraft/
Benchmarks/Tokenization/vocabscale/
Projects/tokenlens/
```

### ✅ Exit Criteria

- [ ] Implement BPE.
- [ ] Explain BPE, WordPiece, and Unigram.
- [ ] Train a tokenizer.
- [ ] Explain vocabulary-size trade-offs.

</details>

<details>
<summary><b>Phase 07 — 🔢 Transformer Inputs, Batching & Masking</b></summary>

### 🎯 Objective

Understand the tensors entering a Transformer.

### ❓ Questions to Answer

#### 1. What does `input_ids` contain?

Study:

`Token IDs` · `Batch Dimension` · `Sequence Dimension`

#### 2. How can variable-length sequences share a batch?

Study:

`Padding` · `Attention Mask`

#### 3. How is future-token visibility prevented?

Study:

`Causal Mask`

#### 4. Why aren't all positions necessarily included in the loss?

Study:

`Labels` · `Ignore Index` · `Loss Masking`

### 📘 Documentation Plan

#### `transformer_model_inputs.pdf`

Cover:

`input_ids` · `position_ids` · `labels` · `Batch Shapes` · `Tensor dtypes`

#### `padding_attention_and_loss_masks.pdf`

Cover:

`Padding` · `Attention Mask` · `Causal Mask` · `Loss Masking`

### 🧪 Investigation — **MaskScope: Transformer Visibility & Loss-Masking Visualizer with Python, PyTorch & Matplotlib**

Build a program displaying:

```text
tokens
padding mask
causal mask
combined visibility matrix
loss mask
```

Test batches containing different sequence lengths.

### 📦 Artifact

```text
Labs/Transformers/maskscope/
```

### ✅ Exit Criteria

- [ ] Explain common input tensors.
- [ ] Construct causal masks.
- [ ] Explain padding masks.
- [ ] Explain loss masking.

</details>

<details>
<summary><b>Phase 08 — 📐 Token Embeddings & Representation</b></summary>

### 🎯 Objective

Understand how discrete token IDs become continuous vectors.

### ❓ Questions to Answer

#### 1. Why can't meaningful computation be performed directly on arbitrary token IDs?

Study:

`Categorical IDs` · `Continuous Representations`

#### 2. What is an embedding lookup?

Study:

`Embedding Matrix` · `Vocabulary Dimension` · `Hidden Dimension`

#### 3. Does geometric proximity always imply semantic similarity?

Study:

`Cosine Similarity` · `Vector Geometry`

#### 4. Why are input embeddings and output weights sometimes shared?

Study:

`LM Head` · `Weight Tying`

### 📘 Documentation Plan

#### `token_embeddings.pdf`

Cover:

`Embedding Matrix` · `Lookup` · `Vocabulary Size` · `Hidden Size` · `Parameters`

#### `embedding_geometry_and_similarity.pdf`

Cover:

`Cosine Similarity` · `Nearest Neighbors` · `Vector Geometry` · `Interpretation Limitations`

#### `embedding_weight_tying.pdf`

Cover:

`Input Embeddings` · `Output Projection` · `Tied Weights`

### 🧪 Investigation — **EmbedScope: Token Embedding Geometry Explorer with Python, PyTorch & Hugging Face Transformers**

1. Load an open model.
2. Extract its embedding matrix.
3. Inspect dimensions.
4. Retrieve selected token vectors.
5. Calculate cosine similarities.
6. Find nearest token embeddings.
7. Compare intuitive and surprising neighbors.

### 📦 Artifact

```text
Labs/Embeddings/embedscope/
```

### ✅ Exit Criteria

- [ ] Explain embedding lookup.
- [ ] Calculate embedding parameter count.
- [ ] Calculate cosine similarity.
- [ ] Explain weight tying.

</details>

---

# PART III — NEURAL LANGUAGE MODELING

<details>
<summary><b>Phase 09 — 🧠 Neural Network Foundations</b></summary>

### 🎯 Objective

Understand the trainable mechanisms used throughout Transformers.

### ❓ Questions to Answer

#### 1. What does a linear layer calculate?

Study:

`Weights` · `Bias` · `Matrix Multiplication`

#### 2. Why are nonlinear functions necessary?

Study:

`Activations` · `ReLU` · `GELU`

#### 3. How does output error reach earlier layers?

Study:

`Loss` · `Backpropagation` · `Chain Rule`

#### 4. How do gradients modify parameters?

Study:

`Optimizer` · `Learning Rate` · `Parameter Updates`

### 📘 Documentation Plan

#### `neural_network_forward_computation.pdf`

Cover:

`Linear Layers` · `Weights` · `Biases` · `Activations` · `Forward Pass`

#### `backpropagation_and_parameter_learning.pdf`

Cover:

`Loss` · `Computation Graph` · `Backpropagation` · `Gradients` · `Parameter Updates`

### 🏗️ Project — **CharForge: Character-Level Neural Language Predictor with Python & PyTorch**

Build:

```text
CHARACTER
   ↓
EMBEDDING
   ↓
LINEAR
   ↓
ACTIVATION
   ↓
LINEAR
   ↓
NEXT CHARACTER
```

Train on a small text corpus.

Record:

```text
training loss
validation loss
generated sequences
parameter count
```

### 📦 Artifact

```text
Projects/charforge/
```

### ✅ Exit Criteria

- [ ] Explain forward/backward passes.
- [ ] Inspect gradients.
- [ ] Train a neural predictor.

</details>

<details>
<summary><b>Phase 10 — 📖 Autoregressive Language Modeling</b></summary>

### 🎯 Objective

Connect neural prediction with sequence modeling.

### ❓ Questions to Answer

#### 1. How is sequence probability decomposed into next-token probabilities?

Study:

`Chain Rule` · `Autoregressive Factorization`

#### 2. How are training examples created from token sequences?

Study:

`Context Windows` · `Shifted Targets` · `Teacher Forcing`

#### 3. Why is cross-entropy used?

Study:

`Logits` · `Target Token` · `Cross-Entropy`

#### 4. What does perplexity measure?

Study:

`Negative Log-Likelihood` · `Perplexity` · `Tokenizer Dependence`

### 📘 Documentation Plan

#### `autoregressive_language_modeling.pdf`

Cover:

`Sequence Probability` · `Autoregressive Factorization` · `Causal LM` · `Teacher Forcing`

#### `next_token_loss_and_perplexity.pdf`

Cover:

`Shifted Labels` · `Cross-Entropy` · `Token Loss` · `Perplexity`

### 🏗️ Project — **BigramForge: Statistical & Neural Bigram Language Model Comparison with Python, NumPy & PyTorch**

Implement:

1. count-based bigram model;
2. neural bigram model.

Compare:

```text
loss
perplexity
parameter count
generated text
```

### 📦 Artifact

```text
Projects/bigramforge/
```

### ✅ Exit Criteria

- [ ] Explain autoregressive factorization.
- [ ] Create shifted targets.
- [ ] Explain perplexity.
- [ ] Train a basic LM.

</details>

---

# PART IV — ATTENTION

<details>
<summary><b>Phase 11 — 👁️ Attention Fundamentals</b></summary>

### 🎯 Objective

Understand attention as content-based information retrieval.

### ❓ Questions to Answer

#### 1. How can one representation search for relevant information?

Study:

`Query` · `Key` · `Similarity`

#### 2. How are similarity scores converted into importance?

Study:

`Dot Product` · `Softmax`

#### 3. How is information combined after relevant positions are found?

Study:

`Value` · `Weighted Sum` · `Context Vector`

### 📖 Sources to Study

- *Attention Is All You Need*
- Dive into Deep Learning

### 📘 Documentation Plan

#### `attention_fundamentals.pdf`

Cover the complete mechanism:

`Query → Key Comparison → Scores → Softmax → Weighted Values → Context`

### 💻 Implementation — **AttentionByHand: Scaled Dot-Product Attention From Scratch with Python, NumPy & PyTorch**

Create small Q/K/V matrices.

Calculate the result manually.

Then reproduce it in Python.

Print every intermediate tensor.

### 📦 Artifact

```text
Code/Attention/attention-by-hand/
```

### ✅ Exit Criteria

- [ ] Explain Q/K/V.
- [ ] Calculate attention manually.
- [ ] Explain weighted aggregation.

</details>

<details>
<summary><b>Phase 12 — ⚡ Self-Attention & Causal Attention</b></summary>

### 🎯 Objective

Implement causal self-attention.

### ❓ Questions to Answer

#### 1. How can every token produce its own Q, K, and V?

Study:

`Input X` · `Wq` · `Wk` · `Wv`

#### 2. Why divide attention scores by √d?

Study:

`Score Magnitude` · `Variance` · `Softmax Saturation`

#### 3. How is future information hidden?

Study:

`Causal Mask`

#### 4. Why does attention become expensive with long sequences?

Study:

`T × T Matrix` · `Quadratic Scaling`

### 📘 Documentation Plan

#### `self_attention_mechanics.pdf`

Cover:

`X` · `Wq/Wk/Wv` · `Q/K/V` · `QKᵀ` · `Scaling` · `Softmax` · `Value Aggregation`

#### `causal_self_attention.pdf`

Cover:

`Autoregressive Constraint` · `Triangular Mask` · `Future Information Leakage`

#### `self_attention_compute_and_memory.pdf`

Cover:

`Sequence Length` · `Attention Matrix` · `Quadratic Compute/Memory`

### 💻 Implementation — **SelfAttentionZero: Causal Self-Attention From Scratch with Python & PyTorch**

Do not use:

```text
nn.MultiheadAttention
scaled_dot_product_attention
```

Implement the operations directly.

### 🧪 Investigation — **AttentionScope I: Token-Level Attention Perturbation Experiment with PyTorch & Matplotlib**

1. Run a short sequence.
2. Save the attention matrix.
3. Change exactly one token.
4. Run again.
5. Calculate attention-weight differences.
6. Visualize both matrices.
7. Explain which relationships changed.

### 📦 Artifacts

```text
Code/Attention/self-attention-zero/
Projects/attentionscope/
```

### ✅ Exit Criteria

- [ ] Implement self-attention.
- [ ] Explain scaling.
- [ ] Implement causal masking.
- [ ] Explain quadratic scaling.

</details>

<details>
<summary><b>Phase 13 — 🧠 Multi-Head Attention</b></summary>

### 🎯 Objective

Understand parallel attention heads and tensor transformations.

### ❓ Questions to Answer

#### 1. Why perform multiple attention operations?

Study:

`Representation Subspaces` · `Parallel Attention`

#### 2. How is hidden size divided between heads?

Study:

`Model Dimension` · `Head Count` · `Head Dimension`

#### 3. How are heads recombined?

Study:

`Concatenation` · `Output Projection`

### 📘 Documentation Plan

#### `multi_head_attention.pdf`

Cover:

`Head Count` · `Head Dimension` · `QKV Projection` · `Head Splitting` · `Per-Head Attention` · `Concatenation` · `Output Projection`

### 💻 Implementation — **MultiHeadZero: Multi-Head Causal Attention From Scratch with Python & PyTorch**

Trace:

```text
[B,T,C]
→ [B,T,H,D]
→ [B,H,T,D]
→ [B,H,T,T]
→ [B,H,T,D]
→ [B,T,C]
```

### 🏗️ Project Upgrade — **AttentionScope II: Multi-Head Transformer Attention Visualizer with PyTorch & Matplotlib**

Add:

```text
layer selection
head selection
token selection
head comparison
attention heatmaps
```

### ✅ Exit Criteria

- [ ] Implement MHA.
- [ ] Explain head dimensions.
- [ ] Split and merge heads correctly.

</details>

<details>
<summary><b>Phase 14 — 📍 Positional Encoding & RoPE</b></summary>

### 🎯 Objective

Understand how Transformers represent sequence order.

### ❓ Questions to Answer

#### 1. Why doesn't self-attention inherently know token order?

Study:

`Permutation Properties`

#### 2. How can absolute position be represented?

Study:

`Learned Position Embeddings` · `Sinusoidal Encoding`

#### 3. How can position modify attention relationships?

Study:

`Relative Position` · `RoPE`

#### 4. Why is RoPE common in decoder-only LLMs?

Study:

`Rotary Embeddings` · `Q/K Rotation`

### 📘 Documentation Plan

#### `absolute_and_sinusoidal_position_encoding.pdf`

Cover:

`Absolute Position` · `Learned Embeddings` · `Sinusoidal Encoding`

#### `relative_position_and_rope.pdf`

Cover:

`Relative Position` · `Rotary Embeddings` · `Q/K Rotation`

Do not include long-context scaling yet.

### 💻 Implementation — **PositionLab: Sinusoidal & Rotary Positional Encoding Explorer with Python, PyTorch & Matplotlib**

Implement:

```text
sinusoidal position encoding
simplified RoPE
```

Visualize positional patterns.

### 📦 Artifact

```text
Code/Transformers/positionlab/
```

### ✅ Exit Criteria

- [ ] Explain why position is necessary.
- [ ] Implement sinusoidal encoding.
- [ ] Explain RoPE.

</details>

---

# PART V — TRANSFORMER ARCHITECTURE

<details>
<summary><b>Phase 15 — 🏗️ Transformer Block Architecture</b></summary>

### 🎯 Objective

Assemble the components of a Transformer block.

### ❓ Questions to Answer

#### 1. Why isn't attention alone enough?

Study:

`Feed-Forward Networks`

#### 2. Why are residual connections used?

Study:

`Residual Path` · `Gradient Flow`

#### 3. Why does normalization matter?

Study:

`LayerNorm` · `RMSNorm` · `Pre-Norm` · `Post-Norm`

#### 4. Why are gated MLPs common?

Study:

`GELU` · `GLU` · `SwiGLU`

### 📘 Documentation Plan

#### `transformer_block_architecture.pdf`

Cover:

`Attention Sublayer` · `MLP Sublayer` · `Residual Paths` · `Block Data Flow`

#### `normalization_and_residual_connections.pdf`

Cover:

`LayerNorm` · `RMSNorm` · `Residuals` · `Pre-Norm` · `Post-Norm`

#### `transformer_feed_forward_networks.pdf`

Cover:

`FFN` · `Expansion` · `GELU` · `Gated MLP` · `SwiGLU`

### 💻 Implementation — **BlockForge: Decoder Transformer Block From Scratch with Python & PyTorch**

Implement:

```python
class TransformerBlock(nn.Module):
    ...
```

Verify:

```text
input shape == output shape
all trainable components receive gradients
causal attention remains intact
```

### 📦 Artifact

```text
Code/Transformers/blockforge/
```

### ✅ Exit Criteria

- [ ] Implement a Transformer block.
- [ ] Explain residuals.
- [ ] Explain normalization.
- [ ] Explain FFNs.

</details>

<details>
<summary><b>Phase 16 — 🔄 Transformer Architecture Families</b></summary>

### 🎯 Objective

Understand encoder-only, decoder-only, and encoder-decoder Transformers.

### ❓ Questions to Answer

#### 1. What changes when attention becomes bidirectional?

Study:

`Encoder` · `Bidirectional Attention`

#### 2. Why are decoder-only models suited to generation?

Study:

`Causal Attention` · `Autoregression`

#### 3. How can one sequence attend to another?

Study:

`Cross-Attention`

#### 4. Why do BERT, GPT-style models, and T5 differ?

Study:

`Encoder-Only` · `Decoder-Only` · `Encoder-Decoder`

### 📘 Documentation Plan

#### `transformer_architecture_families.pdf`

Cover all three architectures together because their differences are best understood comparatively.

#### `cross_attention.pdf`

Cover:

`Decoder Queries` · `Encoder Keys/Values` · `Cross-Sequence Attention`

### 🧪 Investigation — **TransformerFamilyTree: Architecture Comparison with Python & Hugging Face Transformers**

Inspect one small model from each family.

Record:

```text
model type
training objective
layers
hidden size
heads
attention visibility
cross-attention
typical use
```

### 📦 Artifact

```text
Labs/Architectures/transformer-family-tree/
```

### ✅ Exit Criteria

- [ ] Distinguish architecture families.
- [ ] Explain cross-attention.
- [ ] Explain decoder-only generation.

</details>

<details>
<summary><b>Phase 17 — 🤖 Decoder-Only LLM Architecture</b></summary>

### 🎯 Objective

Understand the complete structure of a causal LLM.

### ❓ Questions to Answer

#### 1. What is the full token-ID-to-logit path?

Study:

`Embeddings → Blocks → Final Norm → LM Head`

#### 2. Where do billions of parameters come from?

Study:

`Embeddings` · `Attention` · `MLP` · `Output Head`

#### 3. What can configuration files reveal?

Study:

`Hidden Size` · `Layers` · `Heads` · `KV Heads` · `FFN Size` · `Context`

### 📘 Documentation Plan

#### `decoder_only_llm_architecture.pdf`

Cover the complete decoder-only data path.

#### `llm_parameter_anatomy.pdf`

Cover parameter sources and parameter-count formulas.

#### `llm_configuration_anatomy.pdf`

Cover configuration fields and architectural consequences.

### 🏗️ Project — **ModelXRay: Decoder-Only LLM Architecture Inspector with Python, PyTorch & Hugging Face Transformers**

Build:

```bash
python inspect_model.py <model>
```

Output:

```text
architecture
vocabulary size
hidden size
layers
heads
KV heads
head dimension
FFN size
context
dtype
total parameters
embedding parameters
attention parameters
MLP parameters
```

### 📦 Artifact

```text
Projects/modelxray/
```

### ✅ Exit Criteria

- [ ] Trace IDs to logits.
- [ ] Read configurations.
- [ ] Estimate parameter counts.
- [ ] Identify parameter groups.

</details>

---

# PART VI — GENERATION & MODEL IMPLEMENTATION

<details>
<summary><b>Phase 18 — 🎲 Autoregressive Generation & Decoding</b></summary>

### 🎯 Objective

Understand how model logits become generated language.

### ❓ Questions to Answer

#### 1. Why isn't greedy selection always desirable?

Study:

`Greedy Decoding` · `Sampling`

#### 2. What does temperature change?

Study:

`Logit Scaling` · `Entropy`

#### 3. How do top-k and top-p constrain candidates?

Study:

`Top-k` · `Nucleus Sampling`

#### 4. Why can identical prompts generate different outputs?

Study:

`Random Sampling` · `Seeds`

### 📘 Documentation Plan

#### `autoregressive_generation_loop.pdf`

Cover:

`Forward → Final Logits → Selection → Append → Repeat`

#### `decoding_and_sampling.pdf`

Cover:

`Greedy` · `Temperature` · `Top-k` · `Top-p` · `Repetition Control` · `Stopping`

### 💻 Implementation — **DecodeZero: Autoregressive Decoding From Scratch with Python, PyTorch & Hugging Face Transformers**

Without `model.generate()`, implement:

```python
greedy_decode()
temperature_sample()
top_k_sample()
top_p_sample()
generate()
```

### 🏗️ Project — **DecodeLab: LLM Sampling & Token-Probability Explorer with Python, PyTorch, Hugging Face Transformers, Pandas & Matplotlib**

For every generated token record:

```text
position
selected token
probability
top alternatives
temperature
top-k
top-p
seed
```

Compare generation configurations visually.

### 📦 Artifact

```text
Projects/decodelab/
```

### ✅ Exit Criteria

- [ ] Implement generation.
- [ ] Implement temperature/top-k/top-p.
- [ ] Explain deterministic vs stochastic decoding.

</details>

<details>
<summary><b>Phase 19 — 🏗️ Language Model From Scratch</b></summary>

### 🎯 Objective

Integrate the previous phases into a complete decoder-only Transformer.

### 🏗️ Project — **MiniForgeLM: Decoder-Only Transformer Language Model From Scratch with Python & PyTorch**

Build:

```text
Projects/miniforgelm/
├── README.md
├── config.py
├── tokenizer.py
├── dataset.py
├── embeddings.py
├── attention.py
├── block.py
├── model.py
├── train.py
├── generate.py
├── evaluate.py
├── checkpoint.py
└── tests/
```

### ❓ Questions to Answer

#### 1. Can every component be traced from text to logits?

#### 2. Can the model train without high-level Transformer abstractions?

#### 3. Can checkpoints reproduce generation?

#### 4. Which components dominate parameter count?

### Build Order

```text
TOKENIZER
→ DATASET
→ EMBEDDINGS
→ POSITION
→ CAUSAL MULTI-HEAD ATTENTION
→ TRANSFORMER BLOCK
→ N BLOCKS
→ FINAL NORM
→ LM HEAD
→ LOGITS
```

### Required Tests

```text
tokenizer round trip
tensor shapes
causal masking
attention
Transformer block
forward pass
loss
backward pass
checkpoint save/load
generation
```

### 📘 Documentation Plan

#### `miniforgelm_architecture.pdf`

Document only your implementation architecture and design decisions.

#### `miniforgelm_engineering_report.pdf`

Cover:

`Dataset` · `Configuration` · `Training` · `Loss Curves` · `Generation Samples` · `Failures` · `Limitations`

### 📦 Artifact

```text
Projects/miniforgelm/
```

### ✅ Exit Criteria

- [ ] Build a decoder-only Transformer.
- [ ] Train it.
- [ ] Save/reload it.
- [ ] Generate text.
- [ ] Explain every major component.

</details>

---

# PART VII — PRETRAINING & DATA ENGINEERING

<details>
<summary><b>Phase 20 — 📚 LLM Pretraining</b></summary>

### 🎯 Objective

Understand the complete causal-LM pretraining process.

### ❓ Questions to Answer

#### 1. How are documents transformed into training sequences?

Study:

`Token Streams` · `Context Windows` · `Sequences`

#### 2. What constitutes one training step?

Study:

`Batch` · `Forward` · `Loss` · `Backward` · `Optimizer`

#### 3. How do we distinguish learning from memorization?

Study:

`Training Loss` · `Validation Loss`

#### 4. Why measure training in tokens?

Study:

`Tokens Seen` · `Batch Tokens` · `Training Budget`

### 📘 Documentation Plan

#### `llm_pretraining_pipeline.pdf`

Cover the complete training loop.

#### `pretraining_scale_and_compute.pdf`

Cover:

`Parameters` · `Training Tokens` · `Batch Tokens` · `Steps` · `Compute` · `Scaling Concepts`

### 📊 Benchmark — **ScaleDown: Small Language Model Scaling Experiment with Python, PyTorch, Pandas & Matplotlib**

Train:

```text
2 layers / 128 hidden
4 layers / 128 hidden
4 layers / 256 hidden
```

under controlled data/training budgets.

Measure:

```text
parameters
tokens seen
training time
training loss
validation loss
memory
```

### 📦 Artifact

```text
Benchmarks/Training/scaledown/
```

### ✅ Exit Criteria

- [ ] Explain pretraining.
- [ ] Track tokens seen.
- [ ] Interpret train/validation loss.
- [ ] Explain scale trade-offs.

</details>

<details>
<summary><b>Phase 21 — 🗃️ LLM Data Engineering</b></summary>

### 🎯 Objective

Understand the transformation of raw documents into training-ready data.

### ❓ Questions to Answer

#### 1. Why isn't more text automatically better data?

Study:

`Quality` · `Noise` · `Provenance` · `Licensing`

#### 2. How does repeated content affect training?

Study:

`Exact Deduplication` · `Near Deduplication`

#### 3. How can benchmark data leak into training?

Study:

`Contamination`

#### 4. Why is sequence packing useful?

Study:

`Padding Waste` · `Packing`

#### 5. Why are large datasets sharded?

Study:

`Streaming` · `Sharding` · `Distributed Loading`

### 📘 Documentation Plan

#### `llm_data_provenance_and_collection.pdf`

Cover:

`Sources` · `Licensing` · `Metadata` · `Traceability`

#### `llm_data_cleaning_and_quality.pdf`

Cover:

`Parsing` · `Normalization` · `Language Filtering` · `Quality Filtering`

#### `deduplication_and_contamination.pdf`

Cover:

`Exact Duplicates` · `Near Duplicates` · `Benchmark Leakage`

#### `packing_sharding_and_dataset_mixtures.pdf`

Cover:

`Tokenization` · `Packing` · `Sharding` · `Mixtures`

### 🏗️ Project — **DataForge: Reproducible LLM Pretraining Data Pipeline with Python, Hugging Face Datasets, Tokenizers & Pandas**

Build:

```text
RAW DOCUMENTS
→ INGEST
→ NORMALIZE
→ FILTER
→ DEDUPLICATE
→ TOKENIZE
→ PACK
→ SHARD
→ REPORT
```

Track after every stage:

```text
documents
bytes
characters
tokens
removed documents
duplicates
average length
```

### 🧪 Investigation — **PackingWaste: Sequence Packing Efficiency Experiment with Python, Hugging Face Datasets & Pandas**

Compare:

```text
one-document-per-sequence
packed sequences
```

Measure:

```text
padding tokens
useful tokens
utilization %
number of sequences
```

### 📦 Artifact

```text
Projects/dataforge/
```

### ✅ Exit Criteria

- [ ] Build a reproducible data pipeline.
- [ ] Track provenance.
- [ ] Explain contamination.
- [ ] Deduplicate and pack data.

</details>

---

# PART VIII — TRAINING ENGINEERING

<details>
<summary><b>Phase 22 — 📉 Training Optimization & Stability</b></summary>

### 🎯 Objective

Understand why training converges, diverges, or becomes unstable.

### ❓ Questions to Answer

#### 1. What happens when learning rate is too high or low?

Study:

`Learning Rate` · `Convergence` · `Divergence`

#### 2. Why is AdamW widely used?

Study:

`Momentum` · `Adaptive Moments` · `Weight Decay`

#### 3. Why use warmup?

Study:

`Warmup` · `Schedulers`

#### 4. What do exploding gradients look like?

Study:

`Gradient Norm` · `Clipping` · `NaN/Inf`

### 📘 Documentation Plan

#### `adam_and_adamw.pdf`

Cover:

`SGD` · `Momentum` · `Adam` · `AdamW` · `Weight Decay`

#### `learning_rate_and_scheduling.pdf`

Cover:

`Learning Rate` · `Warmup` · `Decay` · `Cosine Scheduling`

#### `gradient_stability.pdf`

Cover:

`Gradient Norms` · `Explosion` · `Clipping` · `NaN/Inf`

### 🧪 Investigation — **TrainingCrashLab: Learning-Rate & Gradient-Stability Failure Experiment with MiniForgeLM, Python & PyTorch**

Train with:

```text
very low LR
reasonable LR
excessive LR
```

Record:

```text
loss
gradient norm
learning rate
NaN/Inf events
```

Plot all runs.

Explain why each failed or succeeded.

### 📦 Artifact

```text
Labs/Training/training-crash-lab/
```

### ✅ Exit Criteria

- [ ] Explain AdamW.
- [ ] Explain warmup.
- [ ] Detect instability.
- [ ] Measure gradient norms.

</details>

<details>
<summary><b>Phase 23 — ⚡ Training Precision & GPU Memory</b></summary>

### 🎯 Objective

Understand training memory quantitatively.

### ❓ Questions to Answer

#### 1. What occupies GPU memory during training?

Study:

`Weights` · `Gradients` · `Optimizer States` · `Activations`

#### 2. How do FP16 and BF16 differ?

Study:

`FP32` · `FP16` · `BF16` · `Dynamic Range`

#### 3. How can larger effective batches fit?

Study:

`Gradient Accumulation`

#### 4. Why can recomputation reduce memory?

Study:

`Activation Checkpointing`

### 📘 Documentation Plan

#### `training_numerical_precision.pdf`

Cover:

`FP32` · `FP16` · `BF16` · `Mixed Precision` · `Loss Scaling`

#### `llm_training_memory_anatomy.pdf`

Cover:

`Weights` · `Gradients` · `Optimizer States` · `Activations`

#### `memory_efficient_training.pdf`

Cover:

`Gradient Accumulation` · `Activation Checkpointing` · `Offloading Concepts`

### 📊 Benchmark — **VRAMLedger: LLM Training Memory & Precision Benchmark with PyTorch CUDA APIs, Pandas & Matplotlib**

Where hardware supports them, compare:

```text
FP32
FP16
BF16
activation checkpointing on/off
multiple batch sizes
```

Measure:

```text
peak VRAM
step time
tokens/sec
loss
```

### 📦 Artifact

```text
Benchmarks/Training/vramledger/
```

### ✅ Exit Criteria

- [ ] Account for training memory.
- [ ] Explain FP16/BF16.
- [ ] Use gradient accumulation.
- [ ] Explain activation checkpointing.

</details>

<details>
<summary><b>Phase 24 — 🌐 Distributed LLM Training</b></summary>

### 🎯 Objective

Understand how training scales beyond one accelerator.

### ❓ Questions to Answer

#### 1. How do multiple GPUs synchronize training?

Study:

`Data Parallelism` · `Gradient Synchronization` · `All-Reduce`

#### 2. What if the model doesn't fit on one GPU?

Study:

`FSDP` · `ZeRO`

#### 3. How can individual operations be distributed?

Study:

`Tensor Parallelism`

#### 4. How can layers be distributed?

Study:

`Pipeline Parallelism`

#### 5. When does communication become the bottleneck?

Study:

`All-Reduce` · `All-Gather` · `Reduce-Scatter`

### 📖 Sources to Study

- PyTorch Distributed
- PyTorch FSDP
- DeepSpeed
- Megatron-LM
- NVIDIA NCCL

### 📘 Documentation Plan

#### `distributed_training_fundamentals.pdf`

Cover:

`Ranks` · `World Size` · `Process Groups` · `DDP` · `All-Reduce`

#### `fsdp_and_zero.pdf`

Cover:

`Parameter` · `Gradient` · `Optimizer-State Sharding` · `FSDP` · `ZeRO`

#### `llm_model_parallelism.pdf`

Cover:

`Tensor Parallelism` · `Pipeline Parallelism` · `Sequence/Context Parallel Concepts`

#### `distributed_training_communication.pdf`

Cover:

`All-Reduce` · `All-Gather` · `Reduce-Scatter` · `Communication/Compute`

### 📊 Benchmark — **ScaleOut: Single-GPU vs Multi-GPU LLM Training Benchmark with PyTorch Distributed / DDP**

Where multi-GPU hardware is available, compare:

```text
1 GPU
2 GPUs
```

Measure:

```text
tokens/sec
step time
memory/GPU
scaling efficiency
```

### 📦 Artifact

```text
Benchmarks/Distributed-Training/scaleout/
```

### ✅ Exit Criteria

- [ ] Explain DDP.
- [ ] Explain FSDP/ZeRO.
- [ ] Distinguish parallelism strategies.
- [ ] Explain communication overhead.

</details>

<details>
<summary><b>Phase 25 — 💾 Checkpointing & Training Recovery</b></summary>

### 🎯 Objective

Understand complete training-state persistence and recovery.

### ❓ Questions to Answer

#### 1. Why aren't model weights sufficient to resume exactly?

Study:

`Optimizer` · `Scheduler` · `RNG` · `Step`

#### 2. How often should checkpoints be written?

Study:

`Checkpoint Cost` · `Recovery Point`

#### 3. How does distributed training complicate checkpoints?

Study:

`Sharded State`

### 📘 Documentation Plan

#### `training_checkpoint_anatomy.pdf`

Cover:

`Model` · `Optimizer` · `Scheduler` · `Scaler` · `RNG` · `Metadata`

#### `distributed_checkpointing_and_recovery.pdf`

Cover:

`Sharded State` · `Distributed Save/Load` · `Recovery`

### 🔬 Failure Study — **CrashResume: Training Checkpoint Recovery Failure Study with MiniForgeLM & PyTorch**

1. Start training.
2. Save complete checkpoints.
3. Terminate training intentionally.
4. Resume from checkpoint.
5. Verify step, optimizer, scheduler, and RNG state.
6. Compare with uninterrupted training.
7. Repeat using weights-only recovery.
8. Explain the difference.

### 📦 Artifact

```text
Labs/Training/crashresume/
```

### ✅ Exit Criteria

- [ ] Save complete state.
- [ ] Resume correctly.
- [ ] Explain distributed checkpointing concerns.

</details>

---

# PART IX — POST-TRAINING

<details>
<summary><b>Phase 26 — 💬 Instruction Tuning & Chat Models</b></summary>

### 🎯 Objective

Understand how pretrained models become instruction-following assistants.

### ❓ Questions to Answer

#### 1. Why doesn't a base model automatically behave like an assistant?

Study:

`Base Model` · `SFT`

#### 2. How are conversations represented?

Study:

`System` · `User` · `Assistant` · `Chat Templates`

#### 3. Should every conversation token contribute to loss?

Study:

`Label Masking` · `Assistant-Only Loss`

### 📖 Sources to Study

- Hugging Face TRL
- Hugging Face chat templates

### 📘 Documentation Plan

#### `instruction_tuning_fundamentals.pdf`

Cover:

`Base Model` · `Instruction Data` · `SFT` · `Behavior Adaptation`

#### `chat_templates.pdf`

Cover:

`Roles` · `Control Tokens` · `Formatting` · `Generation Prompt`

#### `instruction_tuning_data_and_loss.pdf`

Cover:

`Conversation Dataset` · `Tokenization` · `Labels` · `Loss Masking`

### 🧪 Investigation — **TemplateTrap: Chat-Template Formatting Behavior Experiment with Python & Hugging Face Transformers**

Compare:

```text
correct chat template
plain-text prompt
incorrect role formatting
missing generation prompt
```

Use the same model and semantic request.

Record the resulting prompts/tokens and outputs.

### 🏗️ Project — **MiniForgeChat: Small Instruction-Tuned Chat Model with Python, Hugging Face Transformers, Datasets & TRL**

Fine-tune a suitably small model on an appropriately licensed instruction dataset.

Compare base vs tuned model using held-out prompts.

### 📦 Artifact

```text
Projects/miniforgechat/
```

### ✅ Exit Criteria

- [ ] Explain SFT.
- [ ] Inspect chat templates.
- [ ] Prepare conversation data.
- [ ] Explain loss masking.

</details>

<details>
<summary><b>Phase 27 — 🔧 Fine-Tuning, LoRA & PEFT</b></summary>

### 🎯 Objective

Understand parameter-efficient model adaptation.

### ❓ Questions to Answer

#### 1. Why is full fine-tuning expensive?

Study:

`Trainable Parameters` · `Gradient Memory` · `Optimizer Memory`

#### 2. How does a low-rank update modify a frozen matrix?

Study:

`LoRA` · `Rank` · `A/B Matrices` · `Alpha`

#### 3. Which modules should receive adapters?

Study:

`Target Modules` · `Attention` · `MLP`

#### 4. How can LoRA work with a quantized model?

Study:

`QLoRA`

### 📖 Sources to Study

- Hugging Face PEFT
- LoRA paper
- QLoRA paper

### 📘 Documentation Plan

#### `full_fine_tuning_vs_peft.pdf`

Cover:

`Full Fine-Tuning` · `Frozen Parameters` · `Adapters` · `Training Cost`

#### `lora_architecture.pdf`

Cover:

`Low-Rank Update` · `Rank` · `Alpha` · `Target Modules` · `Merge`

#### `qlora.pdf`

Cover:

`Quantized Base Model` · `LoRA` · `Memory Advantages`

### 🏗️ Project — **LoRALab: Parameter-Efficient Fine-Tuning Benchmark with Python, Hugging Face Transformers, PEFT, TRL & PyTorch**

Compare:

```text
rank = 4
rank = 8
rank = 16
```

Record:

```text
rank
alpha
target modules
trainable parameters
trainable %
peak VRAM
training time
adapter size
evaluation score
```

### 📦 Artifact

```text
Projects/loralab/
```

### ✅ Exit Criteria

- [ ] Explain LoRA mathematically.
- [ ] Configure adapters.
- [ ] Measure trainable-parameter reduction.
- [ ] Explain QLoRA.

</details>

<details>
<summary><b>Phase 28 — 🎯 Preference Alignment & DPO</b></summary>

### 🎯 Objective

Understand preference-based post-training.

### ❓ Questions to Answer

#### 1. How does preference data represent desired behavior?

Study:

`Prompt` · `Chosen` · `Rejected`

#### 2. How does traditional RLHF use preferences?

Study:

`Reward Model` · `Policy` · `PPO Concepts`

#### 3. How does DPO differ?

Study:

`Policy` · `Reference Model` · `Preference Objective`

#### 4. What biases can preference datasets contain?

Study:

`Length Bias` · `Style Bias` · `Annotator Bias`

### 📖 Sources to Study

- InstructGPT
- DPO paper
- Hugging Face TRL

### 📘 Documentation Plan

#### `preference_data_and_reward_modeling.pdf`

Cover:

`Chosen/Rejected` · `Ranking` · `Reward Models` · `Preference Bias`

#### `rlhf_pipeline.pdf`

Cover:

`SFT → Preference Collection → Reward Model → Policy Optimization`

#### `direct_preference_optimization.pdf`

Cover:

`Reference Model` · `Policy` · `DPO Objective` · `RLHF Comparison`

### 🧪 Investigation — **PreferenceLens: Human-Preference Dataset Bias Analysis with Python, Hugging Face Datasets, Pandas & Matplotlib**

Analyze:

```text
prompt length
chosen length
rejected length
length differences
```

Manually inspect samples for:

```text
quality
length bias
style bias
ambiguous preference
```

### 📦 Artifact

```text
Labs/Post-Training/preferencelens/
```

### ✅ Exit Criteria

- [ ] Explain preference datasets.
- [ ] Explain RLHF.
- [ ] Explain DPO.
- [ ] Identify dataset biases.

</details>

---

# PART X — EVALUATION

<details>
<summary><b>Phase 29 — 📊 LLM Evaluation</b></summary>

### 🎯 Objective

Evaluate models reproducibly rather than relying on anecdotal prompts.

### ❓ Questions to Answer

#### 1. Does lower validation loss guarantee better behavior?

Study:

`Loss` · `Perplexity` · `Task Metrics`

#### 2. How are open-ended generations evaluated?

Study:

`Human Evaluation` · `Pairwise Preference` · `Rubrics`

#### 3. Can an LLM judge another LLM reliably?

Study:

`LLM-as-Judge` · `Position Bias` · `Judge Bias`

#### 4. What happens when benchmark data leaks into training?

Study:

`Contamination`

#### 5. Why should quality and performance be evaluated separately?

Study:

`Quality` · `Latency` · `Memory` · `Throughput`

### 📘 Documentation Plan

#### `language_model_quality_evaluation.pdf`

Cover:

`Loss` · `Perplexity` · `Accuracy` · `F1` · `Exact Match`

#### `generative_and_human_evaluation.pdf`

Cover:

`Rubrics` · `Human Preference` · `Pairwise Evaluation` · `LLM Judges`

#### `evaluation_contamination_and_reproducibility.pdf`

Cover:

`Leakage` · `Seeds` · `Prompt Versions` · `Model Versions`

#### `llm_system_evaluation.pdf`

Cover:

`Quality` · `Latency` · `Throughput` · `Memory` · `Cost`

### 🏗️ Project — **EvalForge: Reproducible LLM Evaluation Harness with Python, Hugging Face Transformers, Datasets & Evaluate**

Build:

```text
Projects/evalforge/
├── datasets/
├── prompts/
├── evaluators/
├── metrics/
├── configs/
├── results/
└── run_eval.py
```

Preserve:

```text
model
model revision
prompt
generation configuration
seed
raw output
metric
timestamp
```

### 📦 Artifact

```text
Projects/evalforge/
```

### ✅ Exit Criteria

- [ ] Run reproducible evaluations.
- [ ] Explain metric limitations.
- [ ] Separate quality and system performance.
- [ ] Preserve raw evidence.

</details>

---

# PART XI — INFERENCE ENGINEERING

<details>
<summary><b>Phase 30 — 🚀 LLM Inference Fundamentals</b></summary>

### 🎯 Objective

Understand inference as a measurable execution pipeline.

### ❓ Questions to Answer

#### 1. Why is prompt processing different from subsequent generation?

Study:

`Prefill` · `Decode`

#### 2. What determines time to first token?

Study:

`TTFT` · `Prompt Length` · `Queue Time`

#### 3. Why is tokens/sec different from requests/sec?

Study:

`Token Throughput` · `Request Throughput`

#### 4. Why can equal output lengths have different latency?

Study:

`Prompt Length` · `Prefill Cost`

### 📘 Documentation Plan

#### `llm_inference_execution.pdf`

Cover:

`Load → Tokenize → Prefill → First Token → Decode → Detokenize`

#### `llm_inference_metrics.pdf`

Cover:

`TTFT` · `Inter-Token Latency` · `End-to-End Latency` · `Tokens/sec` · `Requests/sec`

### 🏗️ Project — **InferenceBench: LLM Latency, Throughput & GPU-Memory Benchmark with Python, PyTorch, Hugging Face Transformers & Pandas**

Inputs:

```text
model
precision
prompt length
output length
batch size
concurrency
```

Outputs:

```text
TTFT
total latency
tokens/sec
peak VRAM
```

### 🧪 Investigation — **PromptLengthCurve: LLM Prefill Scaling Experiment with InferenceBench, PyTorch CUDA Metrics & Matplotlib**

Test:

```text
128
512
1024
2048
```

input tokens while keeping output length fixed.

Plot:

```text
TTFT vs prompt length
VRAM vs prompt length
```

### 📦 Artifact

```text
Projects/inferencebench/
```

### ✅ Exit Criteria

- [ ] Explain prefill/decode.
- [ ] Measure TTFT.
- [ ] Measure throughput.
- [ ] Explain prompt-length effects.

</details>

<details>
<summary><b>Phase 31 — 💾 KV Cache & Generation Memory</b></summary>

### 🎯 Objective

Understand autoregressive generation state and memory scaling.

### ❓ Questions to Answer

#### 1. What would naive decoding repeatedly calculate?

Study:

`Previous Tokens` · `K/V Projection`

#### 2. What exactly is cached?

Study:

`Keys` · `Values` · `Layers` · `KV Heads` · `Head Dimension`

#### 3. Why does caching trade memory for speed?

Study:

`Compute Reuse` · `Memory Growth`

#### 4. How can KV memory be estimated?

Study:

`Layers × KV Heads × Head Dimension × Tokens × Bytes`

#### 5. Why do GQA/MQA matter?

Study:

`KV Head Reduction`

### 📘 Documentation Plan

#### `kv_cache_fundamentals.pdf`

Cover:

`Prefill` · `K/V Creation` · `Cache Reuse` · `Decode`

#### `kv_cache_memory_accounting.pdf`

Cover the complete cache-size calculation.

#### `kv_cache_management.pdf`

Cover:

`Static/Dynamic Cache Concepts` · `Paging` · `Offloading` · `Quantized Cache Concepts`

### 📊 Benchmark — **KVScale: KV-Cache Memory & Decode Performance Benchmark with Python, PyTorch, Hugging Face Transformers & CUDA Memory Metrics**

For increasing contexts record:

```text
estimated KV memory
measured GPU memory
TTFT
decode tokens/sec
```

Where supported, compare cache enabled and disabled.

### 📦 Artifact

```text
Benchmarks/Inference/kvscale/
```

### ✅ Exit Criteria

- [ ] Explain what is cached.
- [ ] Estimate KV memory.
- [ ] Explain GQA/MQA implications.

</details>

<details>
<summary><b>Phase 32 — 📦 Quantization & Model Compression</b></summary>

### 🎯 Objective

Understand reduced-precision model deployment.

### ❓ Questions to Answer

#### 1. Why do fewer bits reduce memory?

Study:

`FP32` · `FP16/BF16` · `INT8` · `INT4`

#### 2. How can floating-point values be mapped to integers?

Study:

`Scale` · `Zero Point`

#### 3. Why are some layers more sensitive?

Study:

`Outliers` · `Per-Channel Quantization`

#### 4. How should quantization be evaluated?

Study:

`Memory` · `Latency` · `Throughput` · `Quality`

### 📘 Documentation Plan

#### `llm_numerical_formats.pdf`

Cover common numeric formats.

#### `quantization_fundamentals.pdf`

Cover:

`Scale` · `Zero Point` · `Per-Tensor` · `Per-Channel` · `Weight/Activation Quantization`

#### `llm_quantization_methods.pdf`

Cover:

`8-bit` · `4-bit` · `GPTQ` · `AWQ` · `bitsandbytes` · `PTQ/QAT Concepts`

### 📊 Benchmark — **QuantBench: LLM Precision, Quantization, Memory & Quality Benchmark with Transformers, bitsandbytes, PyTorch & EvalForge**

Compare supported representations of the same model.

Measure:

```text
model size
VRAM
load time
TTFT
tokens/sec
EvalForge quality score
```

### 📦 Artifact

```text
Benchmarks/Inference/quantbench/
```

### ✅ Exit Criteria

- [ ] Explain quantization.
- [ ] Explain scale/zero point.
- [ ] Measure performance and quality.
- [ ] Explain quantization trade-offs.

</details>

---

# PART XII — MODERN LLM ARCHITECTURE

<details>
<summary><b>Phase 33 — ⚡ Efficient Attention</b></summary>

### 🎯 Objective

Understand modern approaches to reducing attention memory and execution cost.

### ❓ Questions to Answer

#### 1. Why does standard MHA create large KV caches?

Study:

`Query Heads` · `KV Heads`

#### 2. How do MQA and GQA reduce memory?

Study:

`Shared K/V` · `Grouped Query Attention`

#### 3. How can FlashAttention accelerate exact attention?

Study:

`Memory IO` · `Tiling` · `Kernel Fusion Concepts`

#### 4. Why restrict attention to local windows?

Study:

`Sliding Window` · `Local Attention`

### 📖 Sources to Study

- FlashAttention
- FlashAttention-2
- PyTorch SDPA documentation

### 📘 Documentation Plan

#### `mha_mqa_gqa.pdf`

Cover architecture and KV-memory differences.

#### `flash_attention.pdf`

Cover:

`Memory Movement` · `Tiling` · `IO Awareness` · `Exact Attention`

#### `sliding_window_attention.pdf`

Cover:

`Local Windows` · `Receptive Field` · `Compute Trade-offs`

### 🧪 Investigation — **AttentionArchitectureAtlas: Modern Attention Configuration Study with Python, Hugging Face Transformers & ModelXRay**

Compare open model configurations.

Record:

```text
query heads
KV heads
head dimension
attention implementation
sliding-window configuration
context length
```

### 📦 Artifact

```text
Labs/Architectures/attention-architecture-atlas/
```

### ✅ Exit Criteria

- [ ] Explain MHA/MQA/GQA.
- [ ] Explain FlashAttention conceptually.
- [ ] Explain local attention.

</details>

<details>
<summary><b>Phase 34 — 🧬 Modern LLM Architecture Patterns</b></summary>

### 🎯 Objective

Understand common components in contemporary decoder-only architectures.

### ❓ Questions to Answer

#### 1. Why is RMSNorm commonly used?

Study:

`LayerNorm` · `RMSNorm`

#### 2. Why are gated MLPs common?

Study:

`SwiGLU`

#### 3. Why is RoPE common?

Study:

`Rotary Position`

#### 4. Which architectural choices affect memory and inference?

Study:

`GQA` · `Hidden Size` · `FFN Size` · `Context` · `Weight Tying`

### 📘 Documentation Plan

#### `modern_transformer_components.pdf`

Cover:

`RMSNorm` · `SwiGLU` · `RoPE` · `GQA` · `Bias Choices`

#### `modern_llm_architecture_comparison.pdf`

Use exclusively for comparative architecture analysis.

### 🏗️ Project Upgrade — **ModelXRay Architecture Archaeology: Open LLM Architecture Comparison with Transformers & Python**

Generate:

```text
model
parameters
layers
hidden size
query heads
KV heads
head dimension
FFN
normalization
activation
position method
context
weight tying
```

Verify against official model documentation.

### ✅ Exit Criteria

- [ ] Read unfamiliar configurations.
- [ ] Identify modern components.
- [ ] Compare architectures systematically.

</details>

<details>
<summary><b>Phase 35 — 🧩 Mixture of Experts</b></summary>

### 🎯 Objective

Understand sparse expert architectures.

### ❓ Questions to Answer

#### 1. What changes when one dense FFN becomes multiple experts?

Study:

`Experts` · `Sparse Activation`

#### 2. How are tokens routed?

Study:

`Router` · `Top-k`

#### 3. What happens when routing becomes imbalanced?

Study:

`Capacity` · `Load Balancing`

#### 4. Why can total and active parameter counts differ dramatically?

Study:

`Total Parameters` · `Active Parameters`

#### 5. Why is MoE difficult to distribute?

Study:

`Expert Parallelism` · `Communication`

### 📘 Documentation Plan

#### `mixture_of_experts_architecture.pdf`

Cover:

`Experts` · `Router` · `Top-k Routing` · `Sparse Activation`

#### `moe_routing_and_load_balancing.pdf`

Cover:

`Capacity` · `Imbalance` · `Load-Balancing Objectives`

#### `moe_systems_engineering.pdf`

Cover:

`Active Parameters` · `Expert Placement` · `Expert Parallelism`

### 💻 Implementation — **TinyMoE: Sparse Mixture-of-Experts Layer From Scratch with Python & PyTorch**

Implement:

```python
Router
Expert
MoELayer
```

Start with:

```text
4 experts
top-2 routing
```

### 🧪 Investigation — **RouterWatch: Mixture-of-Experts Routing & Load-Balance Experiment with PyTorch, Pandas & Matplotlib**

Record the number of tokens assigned to each expert.

Generate deliberately skewed inputs.

Plot expert utilization and routing imbalance.

### 📦 Artifacts

```text
Code/Architectures/tiny-moe/
Labs/Architectures/routerwatch/
```

### ✅ Exit Criteria

- [ ] Implement sparse routing.
- [ ] Explain active vs total parameters.
- [ ] Explain imbalance.
- [ ] Explain expert parallelism.

</details>

<details>
<summary><b>Phase 36 — 📏 Long-Context Language Models</b></summary>

### 🎯 Objective

Understand long-context architecture, behavior, and systems cost.

### ❓ Questions to Answer

#### 1. Why does longer context increase inference cost?

Study:

`Prefill` · `Attention` · `KV Cache`

#### 2. Why can't positional methods extrapolate indefinitely?

Study:

`RoPE` · `Position Extrapolation` · `Scaling`

#### 3. Does information location matter?

Study:

`Lost in the Middle` · `Position Sensitivity`

#### 4. Is maximum context equal to useful context?

Study:

`Context Utilization`

### 📘 Documentation Plan

#### `long_context_architecture.pdf`

Cover:

`Context Window` · `Attention Cost` · `Local/Sliding Strategies`

#### `long_context_positional_methods.pdf`

Cover:

`RoPE Scaling` · `Interpolation/Extrapolation Concepts`

#### `long_context_systems_cost.pdf`

Cover:

`Prefill` · `KV Memory` · `TTFT`

#### `long_context_evaluation.pdf`

Cover:

`Position Sensitivity` · `Retrieval Tests` · `Effective Context`

### 🏗️ Project — **ContextLab: Long-Context Retrieval, Position-Sensitivity & Performance Analyzer with Python, Transformers, PyTorch, Pandas & Matplotlib**

Place a required fact at:

```text
START
25%
50%
75%
END
```

Repeat with increasing context lengths.

Measure:

```text
answer accuracy
TTFT
VRAM
decode speed
```

Plot accuracy and systems cost against context length and fact position.

### 📦 Artifact

```text
Projects/contextlab/
```

### ✅ Exit Criteria

- [ ] Explain long-context cost.
- [ ] Evaluate context utilization.
- [ ] Distinguish maximum and effective context.

</details>

---

# PART XIII — RETRIEVAL & TOOL-AUGMENTED LLMS

<details>
<summary><b>Phase 37 — 🔎 Retrieval-Augmented Generation</b></summary>

### 🎯 Objective

Build and evaluate retrieval-augmented generation from its constituent components.

### ❓ Questions to Answer

#### 1. How can documents be searched semantically?

Study:

`Embedding Models` · `Dense Retrieval` · `Similarity`

#### 2. Why must documents be chunked?

Study:

`Chunking` · `Overlap` · `Metadata`

#### 3. Why might top similarity not mean best evidence?

Study:

`Top-k` · `Reranking`

#### 4. How do we separate retrieval failure from generation failure?

Study:

`Retrieval Evaluation` · `Grounded Generation`

#### 5. Why can hallucination occur despite retrieving the correct document?

Study:

`Context Usage` · `Faithfulness`

### 📖 Sources to Study

- RAG paper
- Sentence Transformers
- FAISS

### 📘 Documentation Plan

#### `embedding_based_retrieval.pdf`

Cover:

`Query Embeddings` · `Document Embeddings` · `Similarity` · `ANN`

#### `document_chunking_and_indexing.pdf`

Cover:

`Parsing` · `Chunk Size` · `Overlap` · `Metadata` · `Index`

#### `rag_architecture.pdf`

Cover:

`Query → Retrieve → Rerank → Context → Generate`

#### `rag_evaluation.pdf`

Cover:

`Retrieval Recall` · `Relevance` · `Grounding` · `Answer Correctness`

### 🏗️ Project — **RAGScope: Retrieval-Augmented Generation Failure Analyzer with Python, Sentence Transformers, FAISS, Hugging Face Transformers & Pandas**

Build:

```text
Projects/ragscope/
├── ingest.py
├── chunk.py
├── embed.py
├── index.py
├── retrieve.py
├── rerank.py
├── generate.py
├── evaluate.py
└── README.md
```

Preserve for every query:

```text
query
expected evidence
retrieved chunks
retrieval scores
reranker scores
generated answer
failure classification
```

### 🧪 Investigation — **ChunkSizeStudy: RAG Chunk-Size Quality Experiment with RAGScope**

Compare:

```text
256
512
1024
```

token chunks.

### 🧪 Investigation — **RetrievalDepthStudy: Top-k Retrieval Recall Experiment with RAGScope**

Compare:

```text
k = 1
k = 3
k = 5
k = 10
```

### 🧪 Investigation — **RerankerImpactStudy: Dense Retrieval vs Reranked Retrieval Experiment with RAGScope**

Compare retrieval metrics and final answer quality with and without reranking.

### 📦 Artifact

```text
Projects/ragscope/
```

### ✅ Exit Criteria

- [ ] Build dense retrieval.
- [ ] Evaluate retrieval independently.
- [ ] Explain chunking.
- [ ] Diagnose retrieval vs generation failure.

</details>

<details>
<summary><b>Phase 38 — 🛠️ Tool Use & Agent Fundamentals</b></summary>

### 🎯 Objective

Understand structured generation and controlled tool execution.

### ❓ Questions to Answer

#### 1. How can probabilistic generation produce structured software arguments?

Study:

`JSON` · `Schemas` · `Structured Outputs`

#### 2. Who validates generated arguments?

Study:

`Application Validation` · `Pydantic` · `JSON Schema`

#### 3. What if a model requests an unauthorized tool?

Study:

`Allowlist` · `Permissions` · `Authorization`

#### 4. How should tool failure be handled?

Study:

`Timeouts` · `Retries` · `Exceptions` · `Idempotency`

#### 5. What turns tool calling into an agent loop?

Study:

`Action` · `Observation` · `State` · `Termination`

### 📘 Documentation Plan

#### `structured_llm_outputs.pdf`

Cover:

`JSON` · `Schemas` · `Parsing` · `Validation`

#### `llm_tool_use_architecture.pdf`

Cover:

`Tool Definition → Selection → Arguments → Execution → Result`

#### `tool_permissions_and_failure_handling.pdf`

Cover:

`Authorization` · `Validation` · `Timeouts` · `Retries` · `Errors`

#### `agent_loop_fundamentals.pdf`

Cover:

`Model → Action → Observation → Model`

### 🏗️ Project — **ToolForge: Schema-Validated LLM Tool-Calling Runtime with Python, Pydantic & Hugging Face/OpenAI-Compatible Tool Schemas**

Provide deterministic tools:

```text
calculator
SQLite query
local document search
mock external service
```

Implement:

```text
schema registry
tool selection
argument parsing
Pydantic validation
permission checking
execution
result injection
failure handling
```

### 🔬 Failure Study — **ToolFailureMatrix: Structured Tool-Calling Failure Study with ToolForge & Pytest**

Test:

```text
malformed JSON
wrong argument type
unknown tool
unauthorized tool
timeout
exception
duplicate request
empty result
```

Create automated tests for every failure mode.

### 📦 Artifact

```text
Projects/toolforge/
```

### ✅ Exit Criteria

- [ ] Validate structured output.
- [ ] Enforce permissions.
- [ ] Handle tool failures.
- [ ] Explain agent loops.

</details>

---

# PART XIV — SERVING

<details>
<summary><b>Phase 39 — 🌐 LLM Serving</b></summary>

### 🎯 Objective

Understand how a model becomes a network-accessible inference service.

### ❓ Questions to Answer

#### 1. What exists between a client and GPU inference?

Study:

`HTTP API` · `Validation` · `Queue` · `Worker` · `Inference Engine`

#### 2. Why stream generated tokens?

Study:

`Streaming` · `Perceived Latency`

#### 3. How do replicas differ from tensor-parallel workers?

Study:

`Replication` · `Tensor Parallelism`

#### 4. How is readiness determined?

Study:

`Health` · `Readiness` · `Startup`

### 📖 Sources to Study

- vLLM
- Hugging Face TGI
- NVIDIA Triton
- TensorRT-LLM
- FastAPI

### 📘 Documentation Plan

#### `llm_serving_request_architecture.pdf`

Cover:

`Client → API → Queue → Tokenizer → Inference Engine → GPU → Response`

#### `llm_serving_topologies.pdf`

Cover:

`Single Worker` · `Replicas` · `Load Balancing` · `Tensor Parallel Serving`

#### `llm_server_lifecycle.pdf`

Cover:

`Startup` · `Model Load` · `Health` · `Readiness` · `Streaming` · `Shutdown`

### 🏗️ Project — **ForgeServe: Streaming LLM Inference API with Python, FastAPI & vLLM**

Build:

```text
Projects/forgeserve/
├── server/
├── client/
├── configs/
├── tests/
└── README.md
```

Implement:

```text
health endpoint
readiness endpoint
generation endpoint
streaming responses
input validation
error handling
metrics endpoint
```

Record baseline:

```text
startup time
model load time
TTFT
tokens/sec
GPU memory
```

### 📦 Artifact

```text
Projects/forgeserve/
```

### ✅ Exit Criteria

- [ ] Serve an LLM through an API.
- [ ] Explain request flow.
- [ ] Implement streaming.
- [ ] Explain serving topologies.

</details>

<details>
<summary><b>Phase 40 — 📦 Batching, Scheduling & Serving Performance</b></summary>

### 🎯 Objective

Understand how inference engines serve concurrent users efficiently.

### ❓ Questions to Answer

#### 1. Why is static batching awkward for generation?

Study:

`Variable Sequence Length` · `Different Completion Times`

#### 2. How does continuous batching work?

Study:

`Iteration-Level Scheduling` · `Admission`

#### 3. Why can concurrency improve throughput while worsening latency?

Study:

`Queueing` · `Saturation`

#### 4. Why does KV memory limit concurrency?

Study:

`Paged KV` · `Capacity`

#### 5. How is saturation detected?

Study:

`Queue Depth` · `Tail Latency` · `Throughput Plateau`

### 📘 Documentation Plan

#### `llm_batching_fundamentals.pdf`

Cover:

`No Batching` · `Static` · `Dynamic` · `Continuous Batching`

#### `llm_request_scheduling.pdf`

Cover:

`Queue` · `Prefill Scheduling` · `Decode Scheduling` · `Fairness` · `Backpressure`

#### `paged_kv_cache.pdf`

Cover:

`Fragmentation` · `Paged Allocation` · `Logical/Physical Blocks`

### 📊 Benchmark — **ConcurrencyCurve: vLLM Continuous-Batching & Saturation Benchmark with Python, AsyncIO, Pandas, Matplotlib & NVIDIA GPU Metrics**

Test:

```text
1
2
4
8
16
```

concurrent requests.

Measure:

```text
queue time
TTFT
p50 latency
p95 latency
p99 latency
requests/sec
tokens/sec
GPU utilization
VRAM
```

Determine the concurrency at which throughput plateaus while latency continues increasing.

### 📦 Artifact

```text
Benchmarks/Serving/concurrency-curve/
```

### ✅ Exit Criteria

- [ ] Explain continuous batching.
- [ ] Explain paged KV.
- [ ] Measure tail latency.
- [ ] Identify saturation.

</details>

---

# PART XV — OBSERVABILITY, SECURITY & RELIABILITY

<details>
<summary><b>Phase 41 — 📊 LLM Observability</b></summary>

### 🎯 Objective

Observe the complete path from application request to GPU execution.

### ❓ Questions to Answer

#### 1. Which metrics represent user experience?

Study:

`TTFT` · `Latency` · `Error Rate`

#### 2. Which metrics describe inference-engine health?

Study:

`Queue Depth` · `Tokens/sec` · `Batching`

#### 3. Which metrics describe GPU health?

Study:

`Utilization` · `VRAM` · `Power` · `Temperature`

#### 4. Why aren't averages sufficient?

Study:

`p50` · `p95` · `p99`

#### 5. How do metrics, logs, and traces work together?

Study:

`Correlation IDs` · `Tracing`

### 📖 Sources to Study

- Prometheus
- Grafana
- OpenTelemetry
- NVIDIA DCGM

### 📘 Documentation Plan

#### `llm_observability_architecture.pdf`

Cover:

`Metrics` · `Logs` · `Traces` · `Correlation`

#### `llm_serving_metrics.pdf`

Cover:

`Request Rate` · `Queue` · `TTFT` · `Latency` · `Tokens/sec`

#### `gpu_telemetry_for_llms.pdf`

Cover:

`GPU Utilization` · `Memory` · `Power` · `Temperature` · `DCGM`

#### `llm_slos_and_alerting.pdf`

Cover:

`SLIs` · `SLOs` · `Tail Latency` · `Availability` · `Alerts`

### 🏗️ Project — **LLMWatch: LLM & GPU Observability Stack with Prometheus, Grafana, OpenTelemetry & NVIDIA DCGM Exporter**

Connect:

```text
FORGESERVE
    ↓
PROMETHEUS
    ↓
GRAFANA

GPU
 ↓
DCGM EXPORTER
 ↓
PROMETHEUS
```

Dashboards:

```text
request rate
errors
queue depth
TTFT
p50/p95/p99
tokens/sec
GPU utilization
VRAM
```

### 🧪 Investigation — **LoadToTelemetry: LLM Load-to-Metrics Correlation Experiment with vLLM, Prometheus, Grafana & DCGM**

Run the ConcurrencyCurve workload.

Capture dashboard changes as concurrency increases.

Explain:

```text
when queue depth begins increasing
when TTFT degrades
when GPU utilization saturates
when throughput plateaus
```

### 📦 Artifact

```text
Projects/llmwatch/
```

### ✅ Exit Criteria

- [ ] Build dashboards.
- [ ] Correlate application/GPU metrics.
- [ ] Explain SLIs/SLOs.
- [ ] Distinguish symptoms and causes.

</details>

<details>
<summary><b>Phase 42 — 🔐 LLM Application Security</b></summary>

### 🎯 Objective

Understand trust boundaries introduced by LLM applications.

### ❓ Questions to Answer

#### 1. Why is retrieved text untrusted?

Study:

`Indirect Prompt Injection`

#### 2. Why can't generated tool calls be trusted automatically?

Study:

`Authorization` · `Validation` · `Least Privilege`

#### 3. Where can sensitive data leak?

Study:

`Prompts` · `Logs` · `Retrieval` · `Tool Results`

#### 4. What supply-chain risks exist?

Study:

`Model Provenance` · `Datasets` · `Dependencies`

#### 5. How should security boundaries be modeled?

Study:

`Threat Modeling` · `Assets` · `Actors` · `Trust Boundaries`

### 📖 Sources to Study

- OWASP guidance for LLM applications
- NIST AI Risk Management Framework

### 📘 Documentation Plan

#### `llm_application_threat_model.pdf`

Cover:

`Assets` · `Actors` · `Trust Boundaries` · `Attack Surfaces`

#### `prompt_injection_and_untrusted_context.pdf`

Cover:

`Direct Injection` · `Indirect Injection` · `Retrieved Instructions`

#### `llm_tool_security.pdf`

Cover:

`Permissions` · `Validation` · `Authorization` · `Side Effects`

#### `llm_supply_chain_and_data_security.pdf`

Cover:

`Model Provenance` · `Data Provenance` · `Dependencies` · `Secrets` · `Logs`

### 🧪 Investigation — **TrustBoundaryLab: RAG & Tool-Calling Threat-Model Experiment with Python, RAGScope, ToolForge & OWASP LLM Guidance**

For every system boundary record:

```text
input
output
trusted?
permissions
sensitive data
possible failure
mitigation
```

Safely test within your own environment:

```text
malicious retrieved instruction
unauthorized tool request
malformed arguments
synthetic secret in context
unsafe logging
```

### 📦 Artifact

```text
Labs/Security/trust-boundary-lab/
```

### ✅ Exit Criteria

- [ ] Threat-model an LLM application.
- [ ] Explain prompt injection.
- [ ] Enforce tool authorization.
- [ ] Identify data/supply-chain risks.

</details>

<details>
<summary><b>Phase 43 — 🩺 LLM Reliability & Troubleshooting</b></summary>

### 🎯 Objective

Develop an evidence-driven LLM failure-diagnosis methodology.

### ❓ Questions to Answer

#### 1. How do memory pressure and compute saturation differ?

Study:

`VRAM` · `GPU Utilization` · `OOM` · `Queue`

#### 2. Why can TTFT increase suddenly?

Study:

`Queueing` · `Prompt Length` · `Concurrency`

#### 3. How can chat formatting look like model failure?

Study:

`Templates` · `Special Tokens`

#### 4. How is a RAG failure localized?

Study:

`Retrieval` · `Reranking` · `Generation`

#### 5. What happens after an incident?

Study:

`Runbooks` · `Postmortems` · `Corrective Actions`

### 📘 Documentation Plan

#### `llm_troubleshooting_methodology.pdf`

Cover:

`Symptom → Scope → Hypothesis → Evidence → Test → Root Cause → Mitigation`

#### `llm_model_and_memory_failures.pdf`

Cover:

`OOM` · `Context Limits` · `KV Pressure` · `Model Loading`

#### `llm_serving_failure_modes.pdf`

Cover:

`Queue Saturation` · `High TTFT` · `Worker Failure` · `Timeout`

#### `rag_and_tool_failure_modes.pdf`

Cover retrieval, reranking, generation, and tool failures together.

#### `llm_incident_response.pdf`

Cover:

`Triage` · `Mitigation` · `Recovery` · `Runbooks` · `Postmortems`

### 🏗️ Project — **FailureForge: LLM Failure-Injection & Troubleshooting Laboratory with ForgeServe, vLLM, RAGScope, ToolForge, Prometheus & Grafana**

Create controlled failures:

```text
GPU memory pressure
context overflow
queue saturation
incorrect chat template
retrieval miss
bad reranking
tool timeout
malformed JSON
model-worker termination
```

For every incident capture:

```text
symptom
metrics
logs
hypothesis
test
root cause
mitigation
recovery
prevention
```

### 📋 Runbooks

Create:

```text
Runbooks/
├── gpu-oom.md
├── high-ttft.md
├── queue-saturation.md
├── model-worker-failure.md
├── retrieval-failure.md
└── tool-failure.md
```

Each runbook:

```text
SYMPTOM
IMPACT
FIRST CHECKS
EVIDENCE
LIKELY CAUSES
MITIGATION
RECOVERY
ESCALATION
PREVENTION
```

### 📦 Artifacts

```text
Projects/failureforge/
Runbooks/
```

### ✅ Exit Criteria

- [ ] Diagnose failures using evidence.
- [ ] Distinguish resource/application failures.
- [ ] Write runbooks.
- [ ] Produce an incident postmortem.

</details>

---

# PART XVI — PRODUCTION

<details>
<summary><b>Phase 44 — 🏭 Production LLM Systems</b></summary>

### 🎯 Objective

Integrate model engineering, retrieval, serving, evaluation, observability, security, and reliability into one production-oriented system.

### ❓ Questions to Answer

#### 1. How should a model be selected for a real workload?

Study:

`Quality` · `License` · `Memory` · `Latency` · `Cost`

#### 2. When should retrieval or tools be added?

Study:

`Knowledge Freshness` · `Private Data` · `Deterministic Actions`

#### 3. How much traffic can the deployment safely sustain?

Study:

`Concurrency` · `Throughput` · `Tail Latency` · `Headroom`

#### 4. How is system health defined?

Study:

`SLIs` · `SLOs` · `Metrics` · `Alerts`

#### 5. What happens when a dependency fails?

Study:

`Failure Isolation` · `Degradation` · `Recovery`

#### 6. How should quality, performance, security, reliability, and cost be considered together?

Study:

`Production Readiness`

### 🏗️ Final Project — **ForgePlatform: Production LLM Platform with Python, FastAPI, vLLM, FAISS, Prometheus, Grafana, OpenTelemetry & NVIDIA DCGM**

Build:

```text
Projects/forgeplatform/
├── README.md
├── app/
├── inference/
├── retrieval/
├── tools/
├── evaluation/
├── benchmarks/
├── observability/
├── security/
├── tests/
├── configs/
└── deployment/
```

### Architecture

```text
                         ┌──────────────┐
                         │    CLIENT    │
                         └──────┬───────┘
                                │
                                ▼
                         ┌──────────────┐
                         │     API      │
                         └──────┬───────┘
                                │
                  ┌─────────────┴─────────────┐
                  │                           │
                  ▼                           ▼
             ┌─────────┐                ┌─────────┐
             │   RAG   │                │  TOOLS  │
             └────┬────┘                └────┬────┘
                  │                           │
                  └─────────────┬─────────────┘
                                │
                                ▼
                       ┌────────────────┐
                       │ MODEL SERVER   │
                       └───────┬────────┘
                               │
                               ▼
                            ┌─────┐
                            │ GPU │
                            └─────┘
                               │
                               ▼
                    METRICS / LOGS / TRACES
                               │
                               ▼
                     PROMETHEUS / GRAFANA
```

### Milestone 1 — Workload Definition

Define:

```text
use case
expected users
request rate
prompt length
output length
quality requirements
latency requirements
availability requirements
privacy requirements
cost constraints
```

### Milestone 2 — Model Selection

Use:

```text
ModelXRay
EvalForge
InferenceBench
```

Record:

```text
license
parameters
architecture
context
quality
VRAM
TTFT
tokens/sec
```

### Milestone 3 — Quality Baseline

Freeze:

```text
evaluation dataset
prompts
model revision
generation configuration
```

Run EvalForge and preserve raw outputs.

### Milestone 4 — Inference Optimization

Evaluate supported:

```text
precision
quantization
context configuration
generation configuration
```

Rerun quality evaluation after every meaningful optimization.

### Milestone 5 — Retrieval

If external/private knowledge is required:

```text
INGEST
→ CHUNK
→ EMBED
→ INDEX
→ RETRIEVE
→ RERANK
→ CONTEXT
→ GENERATE
```

Reuse RAGScope.

### Milestone 6 — Tool Use

If deterministic external actions are required:

```text
MODEL
→ TOOL REQUEST
→ SCHEMA VALIDATION
→ AUTHORIZATION
→ EXECUTION
→ RESULT
→ MODEL
```

Reuse ToolForge.

### Milestone 7 — Serving

Reuse ForgeServe.

Provide:

```text
health
readiness
generation
streaming
metrics
```

### Milestone 8 — Load Testing

Reuse InferenceBench.

Measure:

```text
request rate
queue time
TTFT
p50
p95
p99
tokens/sec
requests/sec
GPU utilization
VRAM
error rate
```

### Milestone 9 — Capacity Study

Determine:

```text
maximum sustainable throughput
acceptable concurrency
latency saturation point
memory headroom
failure point
```

### Milestone 10 — Observability

Reuse LLMWatch.

Monitor:

```text
requests/sec
errors/sec
queue depth
TTFT
p50/p95/p99
input tokens
output tokens
tokens/sec
GPU utilization
GPU memory
```

### Milestone 11 — SLOs

Define workload-specific:

```text
availability
TTFT
end-to-end latency
error rate
quality
```

### Milestone 12 — Security Review

Review:

```text
authentication
authorization
rate limiting
prompt injection
retrieval trust boundaries
tool permissions
secrets
logging
model provenance
dataset provenance
dependencies
licenses
```

### Milestone 13 — Failure Injection

Reuse FailureForge.

Test:

```text
model worker failure
GPU memory pressure
high concurrency
retrieval unavailable
tool unavailable
malformed structured output
```

### Milestone 14 — Recovery Measurement

Record:

```text
detection time
mitigation time
recovery time
user impact
```

### Milestone 15 — Operational Runbooks

Create:

```text
Runbooks/
├── gpu-oom.md
├── high-latency.md
├── queue-saturation.md
├── model-server-failure.md
├── retrieval-failure.md
├── tool-failure.md
└── degraded-generation-quality.md
```

### Milestone 16 — Incident Exercise

Write one complete incident report:

```text
SUMMARY
IMPACT
TIMELINE
DETECTION
ROOT CAUSE
MITIGATION
RECOVERY
WHAT WORKED
WHAT FAILED
CORRECTIVE ACTIONS
```

### 📘 Final Documentation Plan

#### `production_llm_architecture.pdf`

**Question:** How does the complete platform process a request?

Cover:

`API` · `Retrieval` · `Tools` · `Inference Server` · `GPU` · `Observability` · `Dependencies`

#### `llm_capacity_and_performance_engineering.pdf`

**Question:** How much traffic can the platform safely support?

Cover:

`Concurrency` · `Throughput` · `TTFT` · `Tail Latency` · `VRAM` · `Saturation` · `Headroom`

#### `production_llm_security_architecture.pdf`

**Question:** Where are the platform's trust boundaries?

Cover:

`Authentication` · `Authorization` · `Retrieval` · `Tools` · `Secrets` · `Logging` · `Provenance`

#### `production_llm_reliability.pdf`

**Question:** How does the platform detect, survive, and recover from failures?

Cover:

`Health Checks` · `Alerts` · `Incidents` · `Degradation` · `Recovery` · `Runbooks` · `Postmortems`

#### `production_llm_system_report.pdf`

Final engineering report:

```text
1. Problem Definition
2. Requirements
3. Workload Assumptions
4. Architecture
5. Model Selection
6. Evaluation Methodology
7. Quality Results
8. Retrieval Design
9. Tool Architecture
10. Inference Configuration
11. Performance Results
12. Capacity Analysis
13. Observability
14. Security Model
15. Failure Testing
16. Reliability
17. Limitations
18. Future Improvements
```

### 📦 Final Artifacts

```text
Projects/forgeplatform/
Docs/Production/
Benchmarks/Production/
Runbooks/
```

### ✅ Exit Criteria

- [ ] Select a model using evidence.
- [ ] Establish reproducible evaluation.
- [ ] Optimize inference while measuring quality.
- [ ] Integrate retrieval where justified.
- [ ] Integrate validated tools where justified.
- [ ] Serve the model.
- [ ] Benchmark realistic concurrency.
- [ ] Determine sustainable capacity.
- [ ] Build observability.
- [ ] Define SLOs.
- [ ] Threat-model the platform.
- [ ] Inject controlled failures.
- [ ] Recover from failures.
- [ ] Maintain operational runbooks.
- [ ] Produce a complete engineering report.

</details>

---

# 📚 Primary Source Map

Prefer **original papers, official documentation, and authoritative technical references** over summaries.

## 🐍 Python, NumPy & PyTorch

- Python — https://docs.python.org/3/
- NumPy — https://numpy.org/doc/
- PyTorch — https://docs.pytorch.org/docs/stable/
- PyTorch Tutorials — https://docs.pytorch.org/tutorials/

## 🤗 Hugging Face Ecosystem

- Transformers — https://huggingface.co/docs/transformers/
- Tokenizers — https://huggingface.co/docs/tokenizers/
- Datasets — https://huggingface.co/docs/datasets/
- PEFT — https://huggingface.co/docs/peft/
- TRL — https://huggingface.co/docs/trl/
- Evaluate — https://huggingface.co/docs/evaluate/
- LLM Course — https://huggingface.co/learn/llm-course/

## 📚 Foundations

- Speech and Language Processing — https://web.stanford.edu/~jurafsky/slp3/
- Dive into Deep Learning — https://d2l.ai/
- 3Blue1Brown — https://www.3blue1brown.com/

## 🏗️ Transformer Foundations

### Attention Is All You Need

https://arxiv.org/abs/1706.03762

### BERT

https://arxiv.org/abs/1810.04805

### T5

https://arxiv.org/abs/1910.10683

### RoFormer / RoPE

https://arxiv.org/abs/2104.09864

## 🔧 Post-Training

### LoRA

https://arxiv.org/abs/2106.09685

### QLoRA

https://arxiv.org/abs/2305.14314

### InstructGPT

https://arxiv.org/abs/2203.02155

### Direct Preference Optimization

https://arxiv.org/abs/2305.18290

## ⚡ Efficient Attention

### FlashAttention

https://arxiv.org/abs/2205.14135

### FlashAttention-2

https://arxiv.org/abs/2307.08691

## 🧩 Mixture of Experts

### Switch Transformer

https://arxiv.org/abs/2101.03961

## 🔎 Retrieval

- Retrieval-Augmented Generation — https://arxiv.org/abs/2005.11401
- Sentence Transformers — https://www.sbert.net/
- FAISS — https://github.com/facebookresearch/faiss

## 🌐 Distributed Training

- PyTorch Distributed — https://docs.pytorch.org/docs/stable/distributed.html
- PyTorch FSDP — https://docs.pytorch.org/docs/stable/fsdp.html
- DeepSpeed — https://www.deepspeed.ai/
- Megatron-LM — https://github.com/NVIDIA/Megatron-LM
- NVIDIA NCCL — https://docs.nvidia.com/deeplearning/nccl/

## 🚀 Inference & Serving

- vLLM — https://docs.vllm.ai/
- Hugging Face Text Generation Inference — https://huggingface.co/docs/text-generation-inference/
- NVIDIA TensorRT-LLM — https://nvidia.github.io/TensorRT-LLM/
- NVIDIA Triton — https://docs.nvidia.com/deeplearning/triton-inference-server/
- FastAPI — https://fastapi.tiangolo.com/

## 📊 Evaluation

- EleutherAI LM Evaluation Harness — https://github.com/EleutherAI/lm-evaluation-harness
- Hugging Face Evaluate — https://huggingface.co/docs/evaluate/

## 📈 Observability

- Prometheus — https://prometheus.io/docs/
- Grafana — https://grafana.com/docs/
- OpenTelemetry — https://opentelemetry.io/docs/
- NVIDIA DCGM — https://docs.nvidia.com/datacenter/dcgm/

## 🔐 Security

- OWASP — https://owasp.org/
- NIST AI Risk Management Framework — https://www.nist.gov/itl/ai-risk-management-framework

---

# 🗂️ Long-Term Repository Structure

Do **not** create empty directories simply to make the repository look complete.

Create a directory when its first real artifact exists.

```text
LanguageForge/
│
├── README.md
├── ROADMAP.md
│
├── Docs/
│   ├── Foundations/
│   ├── Text/
│   ├── Tokenization/
│   ├── Embeddings/
│   ├── Language-Modeling/
│   ├── Attention/
│   ├── Transformers/
│   ├── Training/
│   ├── Distributed-Training/
│   ├── Post-Training/
│   ├── Evaluation/
│   ├── Inference/
│   ├── Architectures/
│   ├── RAG/
│   ├── Tool-Use/
│   ├── Serving/
│   ├── Observability/
│   ├── Security/
│   ├── Reliability/
│   └── Production/
│
├── Code/
│   ├── Foundations/
│   ├── Tokenization/
│   ├── Attention/
│   ├── Transformers/
│   └── Architectures/
│
├── Labs/
│   ├── Foundations/
│   ├── PyTorch/
│   ├── Text/
│   ├── Transformers/
│   ├── Embeddings/
│   ├── Architectures/
│   ├── Training/
│   ├── Post-Training/
│   └── Security/
│
├── Benchmarks/
│   ├── Tokenization/
│   ├── Training/
│   ├── Distributed-Training/
│   ├── Inference/
│   ├── Serving/
│   └── Production/
│
├── Projects/
│   ├── tokenlens/
│   ├── charforge/
│   ├── bigramforge/
│   ├── attentionscope/
│   ├── modelxray/
│   ├── decodelab/
│   ├── miniforgelm/
│   ├── dataforge/
│   ├── miniforgechat/
│   ├── loralab/
│   ├── evalforge/
│   ├── contextlab/
│   ├── inferencebench/
│   ├── ragscope/
│   ├── toolforge/
│   ├── forgeserve/
│   ├── llmwatch/
│   ├── failureforge/
│   └── forgeplatform/
│
└── Runbooks/
```

---

<div align="center">

### 🧠 LanguageForge

`QUESTION → UNDERSTAND → IMPLEMENT → INVESTIGATE → MEASURE → BUILD`

**Engineering language models from fundamentals to production systems.**

</div>
