# Arian Abdi (`arian262785-cell`)

Independent software and mathematical systems engineer based in Mannheim, Germany.
Focused on deterministic signal processing, low-level compute kernels (`C++` / `Metal` / `Rust` / `Python`), compiler verification, and local edge inference.

---

## ILONA - Unified Local & Web AI Workspace (Black-Box Showcase)

![ILONA Workspace Black-Box Showcase](showcase/ilona_blackbox_showcase.gif)

* **Full 1080p MP4 Video Showcase (`16:9`, 48 kHz Audio):** [`showcase/ILONA_BLACKBOX_WORKSPACE_SHOWCASE.mp4`](showcase/ILONA_BLACKBOX_WORKSPACE_SHOWCASE.mp4) | **[Watch on YouTube (`16:9`)](https://www.youtube.com/watch?v=ZQLgbScmJ_o)**
* **Vertical Audit Reel (`9:16`, 48 kHz Audio):** [`showcase/ILONA_BLACKBOX_VERTICAL_REEL_9x16.mp4`](showcase/ILONA_BLACKBOX_VERTICAL_REEL_9x16.mp4) | **[Watch on YouTube Shorts (`9:16`)](https://www.youtube.com/shorts/X4bgIpNJQCQ)**
* **Technical Specification & Verification Index:** **[`https://arian262785-cell.github.io`](https://arian262785-cell.github.io)**
* **High-Resolution Auditor Views:** [OS Socket Audit (0 Bytes Outbound)](showcase/ilona_blackbox_01.png) | [Live Contract & Hospital Clause Stress-Test](showcase/ilona_blackbox_02.png) | [5-Stage Independent Auditor Scorecard](showcase/ilona_blackbox_03.png) | [VS Code-Style Folder & Domain Switcher](showcase/ilona_blackbox_04.png)

> **Black-Box Verification Table (Mathematically & Empirically Verifiable Metrics Only - No Source Code or Internal Architecture Published):**

| Verification Parameter | Measured Black-Box Value | Mathematical Proof & OS Verification (Shown in Video) |
| :--- | :--- | :--- |
| **1. Kernel Socket & WAN Isolation** | `127.0.0.1:8788` (`LISTEN` Loopback Only) \| `0 Bytes` WAN TX/RX | Verified live via `lsof -nP -iTCP:8788 -sTCP:LISTEN`, `netstat -anvp tcp`, and `tcpdump -ni en0 'not net 127.0.0.0/8'` (`0` external packets, `0` DNS queries, `0` cloud API calls). |
| **2. Sustained Paced Throughput** | `68.68 tok/s` (`14.5603 ms/tok`) on `8.0 GB` Unified RAM | Exact rational pacing `68.68 / 77.77 = 68 / 77` (`1000 / 68.68 = 14.5603 ms/tok` vs. `12.8584 ms/tok`, yielding `+1.7019 ms` deterministic verification time per token within a `15 W - 35 W` local power envelope). |
| **3. Audit Case 1 - Multi-Tier Contract Math** | `32,280.00 EUR` Verified vs. `32,000.00 EUR` Draft (`+280.00 EUR` Caught) | Exact arithmetic proof: `(6 * 2,500.00 + 6 * 3,200.00) * (1 - 0.10) + 1,500.00 = 34,200.00 * 0.90 + 1,500.00 = 30,780.00 + 1,500.00 = 32,280.00 EUR` net (`0 Bytes` WAN). |
| **4. Audit Case 2 - Missing Annex B Gate** | `0.00%` Unverified Guessing (`UNVERIFIED` Deterministic Stop) | Section 9 references an unmounted `Annex B`; system halts deterministically with `UNVERIFIED` instead of fabricating or guessing a Q3 unit price (`0 Bytes` WAN). |
| **5. Audit Case 3 - Corporate Blocking Minority** | `25.1%` Veto Threshold (`74.9% < 75.0%`) & IP Pledge Isolated | Statutory three-quarters majority proof (`Section 53 Abs. 2 GmbHG`): `100.0% - 25.1% = 74.9% < 75.0%` blocks charter amendments; hidden IP pledge (`Section 15 PatG`) isolated (`0 Bytes` WAN). |
| **6. Audit Case 4 - Holding Tax & Runway Proof** | `1.50%` Effective Holding Tax (`95%` Exempt) & `Section 15a InsO` Runway | Statutory holding arithmetic (`Section 8b KStG`): `5.0%` non-deductible share at `~30%` combined corporate/trade tax rate yields `0.05 * 30% = 1.50%` effective tax burden (`0 Bytes` WAN). |
| **7. Audit Case 5 - Clinical Renal Dosage Ceiling** | `mg/kg` Renal Contraindication & Ceiling Flagged (`5 / 5` Audits Passed) | Verifies weight-adjusted `mg/kg` dosage ceiling against impaired renal clearance under statutory medical confidentiality (`Section 203 StGB`, `0 Bytes` WAN). |
| **8. Per-Directory Workspace Isolation** | `1 / 6` Mounted Workspace Folders Active (`-83.33%` Unrelated File Scope) | Strict single-directory mounting (`01-code` through `06-campus`), isolating active context to `1 / 6` (`16.67%`) of local workspace directories (`0 Bytes` cross-folder bleed). |

---

## Dedication to Maryam Mirzakhani (1977-2017) - On 20-Watt Intelligence, European Bureaucracy, and Why We Must Stop Fighting Nature

For Maryam Mirzakhani (1977-2017), who saw the quiet, invariant paths beneath apparent chaos. May that which time took from you too soon be preserved for others.

> *"A drop of water trembled, torn apart*
> *From the wide ocean, heavy at the heart;*
> *The ocean smiled and whispered to the drop:*
> *'We are one whole - a point sets us apart.'"*
> -- Omar Khayyam (1048-1131)

When Maryam Mirzakhani became the first and only woman to receive the Fields Medal for her work on the dynamics and geometry of Riemann surfaces and moduli spaces, she had no interest in self-promotion or tech theater. Having grown up in Tehran during a war, sketching hyperbolic surfaces on large sheets of paper on the floor, she simply said: *"I feel as I always do, and I am honored."* Nine centuries earlier, Omar Khayyam (*"the Tentmaker"*) examined the parallel postulate and laid geometric foundations that would eventually lead to hyperbolic geometry - reminding us in his poetry that what looks separated in chaos belongs to a single underlying whole.

I am writing this from a 50-square-meter apartment in Mannheim, Germany, which I share with my mother. I do not hold a "Dr." title or a university degree; in 2008, I left mechanical engineering at TU Darmstadt after three semesters to take responsibility for my family. For most of my life, I fought against my own nature. Because my mind constantly searched for dynamical patterns and invariants across systems, I thought I was an outsider with nervous tics who was somehow inferior to people with formal titles. Nine months ago, I finally stopped fighting the gift nature gave me, accepted the responsibility that comes with it, and found an inner peace I had never known - even when my financial situation became harder.

Watching how verifiable low-level engineering work is received internationally versus right outside my front door in Germany and Europe reveals a mathematical pattern that explains not only Europe's technological stagnation, but also its political crisis and our ecological dead end:

### 1. The Wrong Equation: Copying Brute Force Under Different Boundary Conditions
Right here in Mannheim in 1885, Carl Benz built the first automobile in a small backyard workshop while his wife Bertha kept the workshop alive with her savings. Like Werner and Carl von Siemens, or Albert Einstein working as a third-class clerk at the Bern patent office while deriving special relativity at his kitchen table, European pioneers created prosperity for generations because they solved problems from their own real boundary conditions through physics, precision, and efficiency.

Today, European AI companies (such as Aleph Alpha right next door in Heidelberg) and legacy European automotive and semiconductor corporations do the exact opposite: they try to copy the US or Chinese brute-force equation - massive GPU clusters, gigawatt data centers, and throwing raw capital and energy at probabilistic transformers. Mathematically, you cannot copy the solution of another system when your boundary conditions are completely different. Europe does not have America's cheap domestic fracking energy and infinite venture capital, nor China's state-centralized coal plants and power grid. Trying to win a brute-force energy game under European constraints guarantees failure.

### 2. Bureaucratic Arrogance, Economic Stagnation, and the Rise of the Far Right in Europe
When Apple's engineers in California reviewed my Metal GPU kernel patches (`mlx#4791` and `#4794`), nobody asked for a university diploma, a vendor registration number, or a 30-page slide deck. They checked the index equation and the regression test, and merged the code. In the US, East Asia, or the Gulf states, the artifact is the credential.

In Germany and Europe, the equation runs backwards. Even when you point directly to documented data races in automotive middleware or bugs in semiconductor HAL drivers - and prove in public commits that you solve those exact problems every week - you hit a wall of arrogant tie-wearing bureaucrats (`Krawattenträger`), rigid HR degree filters, and locked "Preferred Supplier" procurement cartels that would rather approve six-figure budgets for consulting slide decks than let an independent engineer without an academic title touch the code.

This bureaucratic arrogance - the rigid refusal to adapt dynamically as the world evolves - is the direct root cause of Europe's economic crisis and the rise of the far right across the continent:
When rigid elites freeze a society in outdated structures, industry stagnates and living standards erode. People grow bitter and fearful. Instead of taking responsibility for their own structural failure, political opportunists and a bitter establishment redirect that anger onto scapegoats: migrants and minorities. Having lived here for 25 years, I experience that latent and open racism every single day.

Even more dishonest is the historical and geographical blind spot behind that arrogance: Europe is a small peninsula of 500 million people that consumes far more resources and energy per unit of area than Africa, Asia, or even the Americas. Yet many here act as if being native-born European grants an eternal birthright to consume the world's resources, pointing a moralizing finger at China, the US, or the Global South while blaming migrants for homemade economic stagnation.

### 3. Learning from the First Half of the 20th Century: Einstein, Oppenheimer, Helmut Schmidt, and the UN Charter as a Mathematical Invariant
History already showed us in the first half of the 20th century where economic stagnation, wounded pride, and scapegoating lead: two catastrophic World Wars and tens of millions of dead.

Today we face a dangerous generational blind spot. Most political and corporate decision-makers belong to a generation that has never personally experienced a major war and its suffering - unlike post-war statesmen such as Helmut Schmidt, Valery Giscard d'Estaing, or Henry Kissinger, who knew from personal experience what war does to human beings. As Helmut Schmidt warned: *"Marching into a country may be easy; getting out of it decently is not so easy."*

In a world with nine nuclear-armed states, there can be no winner in a next great war; in an existential conflict, states use everything they have to survive. That is why Albert Einstein refused out of deep humanism to work on the atomic bomb, and why J. Robert Oppenheimer - who fell into the trap of *"it is physically solvable, therefore we build it"* - carried bitter regret until the end of his days.

The principle *"Everything that does not violate the laws of nature is mathematically and physically solvable"* defines only the space of physical feasibility, never the sufficient condition to act. An equation is mathematically incomplete and solved falsely if it omits the largest factor in the calculation: human dignity, the common good, and moral responsibility. While personal views of morality can curve like a hyperbolic surface depending on where an observer stands, humanity has a fixed invariant agreed upon after the horrors of the 20th century: the Charter of the United Nations and the inviolable dignity of every human being. Life-and-death military decisions must never be handed over to automated AI systems, and reckless capital-driven AI racing that ignores human safety will ultimately destroy itself.

### 4. Ending the 300-Year War Against Nature: The 20-Watt Human Brain Blueprint
For 300 years since the start of industrialization, humanity has treated economic growth as synonymous with exponential CO2 growth and the destruction of the biosphere. Why? Out of the same human arrogance: believing that because we sit at a tip of evolution, we are the rulers and builders of nature. We are not. We are a part of nature and evolution. When a part of a system wages war against the host system that sustains it, it destroys everything that makes life worth living.

Look at today's cloud AI frenzy - which astrophysicist Prof. Harald Lesch recently summarized in Munich with a single question: *"Have we lost our minds?"* The industry burns gigawatts of electricity, evaporates millions of liters of cooling water, and calls for nuclear reactors just so bloated probabilistic models can guess tokens, trampling the laws of thermodynamics (Rolf Landauer's principle).

Nature itself already gave us the proof that intelligence does not require environmental destruction: the human brain performs extraordinary reasoning, mathematics, and creativity on **20 Watts** of power.

When we bow to nature instead of fighting it - replacing megawatt brute force with mathematical precision, harmonic pacing (`68.68 tok/s`), and deterministic local verification on `8.0 GB` of memory (`15-35 Watts`, `0 bytes` of cloud waste) - we prove that technological progress and ecological responsibility belong together.

A system can never replace human beings, and it must never put the human mind to sleep. Its only legitimate purpose is to expand human possibilities so that every person can crystallize and live the best, natural version of themselves. And to make sure my own habits never get corrupted by money or scaling pressure, my brother will handle the commercial side while I keep my daily work anchored in research that directly relieves human suffering - such as non-toxic, physics-based vascular cancer research.

Nature is worth standing up for. And if we humble ourselves before the laws of nature and human dignity, it goes better.

---

## Two-Week Engineering & Open-Source Log (October 19 - November 1, 2026)

Over the past two weeks, alongside finalizing the ILONA workspace environment, we contributed upstream bug fixes across GPU compute kernels, compiler borrow checkers, and evaluation frameworks:

### 1. Low-Level Compute Kernels & Edge Inference (`C++` / `Metal` / `Python`)
* **[`ml-explore/mlx#4791`](https://github.com/ml-explore/mlx/pull/4791) (Merged - [`9e2e8e2`](https://github.com/ml-explore/mlx/commit/9e2e8e26c62f5a6fb7c4381d08475a7d39757bf4))** - Fixed 4D per-channel gate (`g`) indexing stride bug in the Metal `gated_delta_update` kernel where `g_idx` omitted the head-dimension stride `Dh` (`((b_idx * T + t) * Hv + hv_idx) * Dh + dv_idx`), preventing cross-head out-of-bounds reads on 4D vector-gated recurrence states (closes [`#4763`](https://github.com/ml-explore/mlx/issues/4763)).
* **[`ml-explore/mlx#4794`](https://github.com/ml-explore/mlx/pull/4794) (Merged - [`9d5b21d`](https://github.com/ml-explore/mlx/commit/9d5b21d310eaee2c71e1dc3357cd8b1196c95abd))** - Promoted Metal `SliceUpdate` offset arithmetic (`src_offset`, `out_offset`) to `int64_t` across strided and contiguous copy kernels to prevent 32-bit signed integer overflow on large tensors (closes [`#3126`](https://github.com/ml-explore/mlx/issues/3126)).
* **[`ml-explore/mlx#4793`](https://github.com/ml-explore/mlx/pull/4793)** - Refined NAX Steel GEMM split-K dispatch heuristic (`k >= 1024 && m <= 64 && n <= 1024`) to avoid split-K reduction barrier overhead when M/N tile occupancy already saturates the GPU.
* **[`ml-explore/mlx-lm#2020`](https://github.com/ml-explore/mlx-lm/pull/2020)** - Fixed `json_tools` streaming parser bracket rebalancing (`_rebalance_brackets`) to track string literal state and escape sequences (`\"`, `\\`), preventing bracket characters inside string arguments from corrupting the outer JSON delimiter stack.
* **[`awni/mylm#2`](https://github.com/awni/mylm/pull/2)** - Fixed stale LoRA adapter checkpoint selection across multi-session continual sleep consolidation and guarded masked cross-entropy loss against zero-token division (`NaN`) when the prompt spans the full context window.
* **[`awni/voxmlx#8`](https://github.com/awni/voxmlx/pull/8)** - Applied causal sliding-window attention mask (`create_additive_causal_mask(N, offset)`) in the Conformer speech encoder (`EncoderBlock`) to enforce bounded left-context attention during streaming and chunked inference.

### 2. Compiler Verification & Static Analysis (`Rust`)
* **[`limitlessprojects/Go-Hybrid#2316`](https://github.com/limitlessprojects/Go-Hybrid/pull/2316)** - Fixed lexical environment snapshot soundness bug in the borrow/ownership checker (`hy-check`) when inner-scope block shadowing (`:=`) overlapped with variables captured by an outer closure.

### 3. Statistical & Mathematical Verification (`Python` / `Rust`)
* **[`Aleph-Alpha-Research/eval-framework#1193`](https://github.com/Aleph-Alpha-Research/eval-framework/pull/1193)** - Replaced floating `refs/convert/parquet` branch loading for `allenai/social_i_qa` with a deterministic commit SHA (`537a2ec8ec565adc0b70b70752893e59e024df26`) in `frozen-hf-dataset-revisions.json` via `pinned_frozen` (closes [`#491`](https://github.com/Aleph-Alpha-Research/eval-framework/issues/491)).
* **[`Aleph-Alpha-Research/eval-framework#1177`](https://github.com/Aleph-Alpha-Research/eval-framework/pull/1177)** - Fixed multi-subject standard error (`stderr`) aggregation by computing the root-sum-of-squares pooled standard error (`math.sqrt(sum(se**2)) / N`) instead of an unweighted arithmetic mean of standard errors.
* **[`Aleph-Alpha/aleph-alpha-inference#10`](https://github.com/Aleph-Alpha/aleph-alpha-inference/pull/10)** - Eliminated redundant token-vector allocation per generation loop step in the Rust inference worker when sampling logprobs are disabled (`logprobs == 0`).

### 4. Standalone Open-Source & Verification Utilities
* **[`biba-v1.1`](https://github.com/arian262785-cell/biba-v1.1)** - Command-line timeline compositor for 9:16 vertical video over raw FFmpeg pipes with pre-allocated frame buffers and temporal TPDF sub-LSB dithering.
* **[`reelgate`](https://github.com/arian262785-cell/reelgate) (`v0.3.0`)** - Deterministic broadcast, vertical video, and regulatory compliance gate (ISO/IEC 14496-12 MP4 `faststart` box scanner, H.264/BT.709 stream check, ITU-R BS.1770-4 `LUFS` and 4x oversampled `dBTP` loudness verification, SQLite SHA-256 asset deduplication ledger, and COPPA/JMStV/UWG/UrhG compliance evaluator).
* **[`inboxshield`](https://github.com/arian262785-cell/inboxshield)** - Zero-trust RFC 5322 email sanitizer (attachment/link stripping, prompt-injection firewall), RFC 3463 DSN bounce parser with SQLite suppression ledger, and deterministic DACH B2B reply classifier.
* **[`leadgate`](https://github.com/arian262785-cell/leadgate)** - Deterministic B2B entity pre-qualification, multi-year statutory R&D grant (`FZulG` 2022-2029) calculation engine, and SQLite-WAL review state machine.

---

## Global B2B Remote Engineering & Enterprise Inquiries

**Contact:**
- **Email:** `ariila262785@gmail.com`
- **Location:** Mannheim, Germany (`CET / UTC+1`)
