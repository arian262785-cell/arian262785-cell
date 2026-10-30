# Arian Abdi (`arian262785-cell`)

Independent software and mathematical systems engineer based in Mannheim, Germany.
Focused on deterministic signal processing, low-level kernel optimization (C++ / Metal / Rust / Python), compiler verification, and local edge inference.

---

## Selected Open-Source Contributions & Engineering Work

### 1. Low-Level Compute Kernels & Edge Inference (`C++` / `Metal` / `Python`)
* **[`ml-explore/mlx#4791`](https://github.com/ml-explore/mlx/pull/4791) (Merged - [`9e2e8e2`](https://github.com/ml-explore/mlx/commit/9e2e8e26c62f5a6fb7c4381d08475a7d39757bf4))** - Fixed 4D per-channel gate (`g`) indexing stride bug in the Metal `gated_delta_update` kernel where `g_idx` omitted the head-dimension stride `Dh` (`((b_idx * T + t) * Hv + hv_idx) * Dh + dv_idx`), preventing cross-head out-of-bounds reads on 4D vector-gated recurrence states (closes [`#4763`](https://github.com/ml-explore/mlx/issues/4763)).
* **[`ml-explore/mlx#4793`](https://github.com/ml-explore/mlx/pull/4793)** - Refined NAX Steel GEMM split-K dispatch heuristic (`k >= 1024 && m <= 64 && n <= 1024`) to avoid split-K reduction barrier overhead when M/N tile occupancy already saturates the GPU.
* **[`ml-explore/mlx#4794`](https://github.com/ml-explore/mlx/pull/4794)** - Promoted Metal `SliceUpdate` offset arithmetic (`src_offset`, `out_offset`) to `int64_t` across strided and contiguous copy kernels to prevent 32-bit signed integer overflow on large tensors (closes [`#3126`](https://github.com/ml-explore/mlx/issues/3126)).
* **[`ml-explore/mlx-lm#2020`](https://github.com/ml-explore/mlx-lm/pull/2020)** - Fixed `json_tools` streaming parser bracket rebalancing (`_rebalance_brackets`) to track string literal state and escape sequences (`\"`, `\\`), preventing bracket characters inside string arguments from corrupting the outer JSON delimiter stack.
* **[`awni/mylm#2`](https://github.com/awni/mylm/pull/2)** - Fixed stale LoRA adapter checkpoint selection across multi-session continual sleep consolidation and guarded masked cross-entropy loss against zero-token division (`NaN`) when the prompt spans the full context window.
* **[`awni/voxmlx#8`](https://github.com/awni/voxmlx/pull/8)** - Applied causal sliding-window attention mask (`create_additive_causal_mask(N, offset)`) in the Conformer speech encoder (`EncoderBlock`) to enforce bounded left-context attention during streaming and chunked inference.

### 2. Compiler Verification & Static Analysis (`Rust`)
* **[`limitlessprojects/Go-Hybrid#2316`](https://github.com/limitlessprojects/Go-Hybrid/pull/2316)** - Fixed lexical environment snapshot soundness bug in the borrow/ownership checker (`hy-check`) when inner-scope block shadowing (`:=`) overlapped with variables captured by an outer closure.

### 3. Statistical & Mathematical Verification (`Python`)
* **[`Aleph-Alpha-Research/eval-framework#1177`](https://github.com/Aleph-Alpha-Research/eval-framework/pull/1177)** - Fixed multi-subject standard error (`stderr`) aggregation by computing the root-sum-of-squares pooled standard error (`math.sqrt(sum(se**2)) / N`) instead of an unweighted arithmetic mean of standard errors.

### 4. Standalone Open-Source Packages (MIT)
* **[`reelgate`](https://github.com/arian262785-cell/reelgate)** - Deterministic broadcast and vertical video quality gate (H.264 bitstream inspection, `yuv420p` chroma check, `faststart` atom layout, ITU-R BS.1770-4 loudness verification, SHA-256 deduplication ledger).
* **[`inboxshield`](https://github.com/arian262785-cell/inboxshield)** - Zero-trust RFC 5322 email sanitizer (attachment/link stripping, prompt-injection firewall), RFC 3463 DSN bounce parser with SQLite suppression ledger, and deterministic DACH B2B reply classifier.
* **[`biba-v1.1`](https://github.com/arian262785-cell/biba-v1.1)** - Command-line timeline compositor for 9:16 vertical video over raw FFmpeg pipes with pre-allocated frame buffers and temporal TPDF sub-LSB dithering.

---

## B2B Remote Engineering & Contracting (DACH / Europe)

Available for remote B2B engineering mandates and work packages (`80% - 100% Remote`) across European semiconductor, embedded systems, and automotive software teams:
- Edge-AI quantization (`Float32` / `FP16` / `Int8` / `FP8`), NPU/DSP operator lowering, and numerical accuracy verification
- Memory-safe system components, IPC ring buffers, and static analysis / compiler passes in `C++` and `Rust`
- Deterministic Software-in-the-Loop (SIL) test oracles and audio/video/sensor signal pipelines in `Python` and `C++`

**Contact:**
- **Email:** `ariila262785@gmail.com`
- **Phone (Office):** `+49 621 43786527`
- **Location:** Mannheim, Germany
