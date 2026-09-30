# 🏆 Best AI Models: Benchmark Cheat Sheet

> Top LLMs across independent leaderboards. Snapshot: **2026-09-30**. 26+ models shipped in September alone.
> Every number is copied from a cited source with its date. Nothing is estimated or invented.

## Contents
- [TL;DR](#-tldr)
- [Intelligence Index (Artificial Analysis)](#-intelligence-index-artificial-analysis)
- [Overall score (BenchLM)](#-overall-score-benchlm)
- [Human preference (Arena)](#-human-preference-arena-text-elo)
- [Category leaders](#-category-leaders)
- [Pricing and context](#-pricing-and-context)
- [Open-weights models](#-open-weights-models)
- [September 2026 release log](#-september-2026-release-log)
- [Caveats](#-read-this-before-trusting-any-number)
- [Sources](#sources)

## ⚡ TL;DR

| Need | Pick |
|------|------|
| Highest overall score | **GPT-6 Astra** (BenchLM #1) |
| Highest Intelligence Index | **Claude Opus 5.5 (max)**, 58 |
| Best human-preference Elo | **Claude Opus 5.5 (high)**, 1509 (statistical tie with 4 others) |
| Best quality for the price | **Claude Opus 5.5** ($4/$20), or **GPT-6.1 Sol** (AA index 52 at $0.72 blended cost, the cheapest top-5 entry) |
| Cheapest usable | **GPT-6 Luna** ($0.10/$0.50) or **Muse Spark 1.3** (~$0.10 blended) |
| Best open weights | **Kimi K3** (GPQA 93.5%) or **MiMo-V2.6-Pro** (AA index 46) |

## 🧠 Intelligence Index (Artificial Analysis)

Composite of many evals. Best setting shown per model; reasoning effort in parentheses. Cost is the blended figure the site reports. Source: [artificialanalysis.ai](https://artificialanalysis.ai/leaderboards/models)

| # | Model | Creator | Index | Context | Cost | Speed | Weights |
|---|-------|---------|-------|---------|------|-------|---------|
| 1 | Claude Opus 5.5 (max) | Anthropic | 58 | 1M | $5.98 | 92 t/s | Closed |
| 2 | Claude Sonnet 5.5 (max) | Anthropic | 56 | 1M | $7.60 | 139 t/s | Closed |
| 3 | Claude Fable 5.1 (max) | Anthropic | 53 | 1M | $7.63 | 69 t/s | Closed |
| 3 | GPT-6 Astra (max) | OpenAI | 53 | 1M | $3.26 | 56 t/s | Closed |
| 5 | GPT-6.1 Sol (max) | OpenAI | 52 | 1M | $0.72 | 68 t/s | Closed |
| 6 | Muse Spark 1.3 (max) | Meta | 48 | 1M | $1.60 | 177 t/s | Closed |
| 7 | GPT-6 Sol (max) | OpenAI | 48 | 872K | $1.05 | 76 t/s | Closed |
| 8 | Grok 4.7 (xhigh) | SpaceXAI | 46 | 500K | $3.74 | 74 t/s | Closed |
| 8 | MiMo-V2.6-Pro | Xiaomi | 46 | 1M | $0.13 | 41 t/s | Closed* |

*The launch coverage lists MiMo V2.6 as open source, while the leaderboard lists it as closed. Verify before relying on the license.

Note: a September release-log source cites Fable 5.1 at 66 on "Index v4.1.1", which does not match the leaderboard above. The index version differs, so don't compare across sources.

## 🥇 Overall score (BenchLM)

Weighted score across 8 categories. Data date 2026-09-29. Source: [benchlm.ai](https://benchlm.ai/)

| # | Model | Provider | Score | Output $/1M |
|---|-------|----------|-------|-------------|
| 1 | GPT-6 Astra | OpenAI | 88.22 | $50.00 |
| 2 | Claude Opus 5.5 | Anthropic | 86.94 | $20.00 |
| 3 | Claude Fable 5.1 | Anthropic | 82.50 | $50.00 |
| 4 | Claude Sonnet 5.5 | Anthropic | 80.90 | $10.00 |
| 5 | Claude Opus 5 | Anthropic | 79.24 | $25.00 |
| 6 | Claude Fable 5 | Anthropic | 78.59 | $50.00 |
| 7 | GPT-6 Sol | OpenAI | 78.57 | $10.00 |
| 8 | GPT-5.6 Sol | OpenAI | 78.19 | $20.00 |
| 9 | MiMo-V2.6-Pro | Xiaomi | 74.18 | $0.87 |
| 10 | Gemini 3.8 Flash | Google | 73.31 | $3.75 |
| 11 | GPT-5.6 Terra | OpenAI | 72.40 | $12.00 |
| 12 | GPT-5.5 Pro | OpenAI | 72.18 | $180.00 |

GPT-6.1 Sol (released Sep 29) is not in this snapshot yet.

## 💬 Human preference (Arena text Elo)

Blind pairwise votes. Last updated 2026-09-25. Source: [arena.ai](https://arena.ai/leaderboard/text)

| # | Model | Org | Score | Votes |
|---|-------|-----|-------|-------|
| 1 | claude-opus-5.5-high | Anthropic | 1509 ±12 | 2,307 |
| 2 | claude-opus-4-6-high | Anthropic | 1505 ±3 | 76,518 |
| 3 | claude-fable-5-high | Anthropic | 1504 ±4 | 36,462 |
| 4 | claude-opus-4-7-high | Anthropic | 1502 ±4 | 64,007 |
| 5 | claude-fable-5.1-max | Anthropic | 1501 ±7 | 9,942 |
| 6 | claude-opus-4-6 | Anthropic | 1498 ±3 | 80,836 |
| 7 | muse-spark-1.2 (xHigh) | Meta | 1496 ±10 | 3,422 |
| 8 | claude-opus-4-7 | Anthropic | 1495 ±4 | 65,051 |
| 9 | muse-spark-1.3-max | Meta | 1494 ±7 | 10,036 |
| 10 | gemini-3.8-flash-high | Google | 1492 ±5 | 21,728 |

The top five overlap within error margins, so treat them as a tie. Sonnet 5.5, GPT-6.x and Grok 4.7 have too few votes to appear yet.

## 🎯 Category leaders

From [llm-stats.com](https://llm-stats.com/) and [morphllm.com](https://www.morphllm.com/swe-bench-pro).

| Category | Leader | Reported score |
|----------|--------|----------------|
| GPQA Diamond | GPT-6 Astra | 96.0% |
| GPQA Diamond, open weights | Kimi K3 | 93.5% |
| AIME 2025 | GPT-5.2 Pro | 100.0% |
| Coding (Arena) | Claude Opus 5 | 26.7 |
| SWE-bench Pro (public / commercial) | Muse Spark 1.1 | 61.5% / 51.5% |
| DeepSWE | MiMo-V2.6-Pro | 72.57 |
| Terminal-Bench 2.1 | Gemini 3.8 Flash | 90.8% |
| Terminal-Bench 4.0 | Claude Mythos 5.1 (gated) | 60.9% |
| Terminal-Bench 4.0 (public) | Claude Fable 5.1 | 55.8% |
| CyberGym | GLM-5.3 | 84.5% |
| Throughput | Mistral Medium 3.5 | 325 tok/s |
| Longest context | Grok-4.1 Fast Non-Reasoning | 2.0M |

**SWE-bench Verified: sources disagree.** Reported values for top models range from 80.0% to 95.0% depending on the listing ([llm-stats](https://llm-stats.com/benchmarks/swe-bench-verified)). Check the primary source before quoting.

## 💸 Pricing and context

USD per 1M tokens (input / output). Sources: [local-ai-zone](https://local-ai-zone.github.io/blog/September_2026_AI_Model_Updates.html), [TeamDay](https://www.teamday.ai/blog/best-ai-models-2026)

| Model | Price | Context |
|-------|-------|---------|
| GPT-6 Astra | $10 / $50 | 1.05M |
| Claude Fable 5.1 | $10 / $50 | 1M |
| Claude Opus 5.5 | $4 / $20 | 1M |
| Claude Sonnet 5 | $2 / $10 | 1M |
| GPT-6 Sol | $2 / $10 | not listed |
| Kimi K3 | $3 / $15 | 1M |
| Grok 4.7 | $3.20 / $9.60 (OpenRouter listing: $1.60 / $4.80) | 500K |
| Qwen3.8-Max (0902) | $2 / $6 | 1M |
| Gemini 3.8 Flash | $0.75 / $3.75 (doubles Jan 1, 2027) | 1M |
| DeepSeek V4.1-Flash | $0.30 / $1.20 peak, $0.15 / $0.60 off-peak | 1M |
| GLM-5.3-Flash | $0.15 / $0.50 | 1M |
| MiMo-V2.6-Pro | $0.435 / $0.87 | 1M |
| GPT-6 Luna | $0.10 / $0.50 | not listed |
| Muse Spark 1.3 | ~$0.10 blended | not listed |

Claude Sonnet 5.5 and GPT-6.1 Sol launch pricing was not confirmed in my sources.

## 🔓 Open-weights models

| Model | Org | Notes |
|-------|-----|-------|
| Kimi K3 | Moonshot | GPQA Diamond 93.5%, top open model on that benchmark |
| MiMo-V2.6-Pro / Flash | Xiaomi | AA Index 46, highest reported open-weight; 1M context |
| Qwen3.8-2.4T-A95B | Alibaba | 2.4T total / 95B active MoE |
| Qwen3.8-27B | Alibaba | Dense; reported to beat Claude Opus 4.6 on 15 of 19 benchmarks; runs in 24GB VRAM |
| Hy4 preview | Tencent | 770B/49B MoE; GPQA 92.3% |
| GLM-5.3 FlashX | Z.ai | Open weights, Sep 18 |
| DeepSeek V4-Pro-0813 / V4-Flash-0731 | DeepSeek | 1M context |
| MiniMax H3 | MiniMax | 465B/30B MoE, omni-modal |
| Cohere Command A+ | Cohere | Open weights, 192K context |
| Nemotron 3.5 Lightning-30B-A3B | NVIDIA | 30B/3B MoE |
| Bonsai 2 27B | Prism ML | 98.2% FP16 quality retained at 5.9GB |

## 🗓 September 2026 release log

Sources: [LLM Gateway](https://llmgateway.io/timeline), [LLM-Stats](https://llm-stats.com/llm-updates)

| Date | Model | Provider |
|------|-------|----------|
| Sep 29 | GPT-6.1 Sol | OpenAI |
| Sep 28 | Claude Sonnet 5.5 | Anthropic |
| Sep 24 | Perplexity Search Fast | Perplexity |
| Sep 23 | GLM 5.3 Prime, Qwen3.8 Max Prime, Gemini 3.8 Flash TTS | Z.ai, Alibaba, Google |
| Sep 22 | Claude Opus 5.5, GPT-6 Sol, GPT-6 Luna, MiMo-V2.6 Pro/Flash, Cohere Command A+, Nex N2.5 Mini/Pro | multiple |
| Sep 21 | Grok 4.7, Qwen3.8 Omni Flash | SpaceXAI, Alibaba |
| Sep 18 | GLM-5.3 FlashX | Z.ai |
| Sep 17 | Bonsai 2 27B | Prism ML |
| Sep 15 | Gemini 3.8 Live | Google |
| Sep 10 | DeepSeek V4.1-Flash | DeepSeek |
| Sep 3 | GPT-6 Astra, Qwen3.8-Max (0902) | OpenAI, Alibaba |
| Sep 2 | Gemini 3.8 Flash, Gemini 3.8 Flash Cyber, Muse Spark 1.3 | Google, Meta |
| Sep 1 | Claude Fable 5.1, Claude Mythos 5.1 (gated) | Anthropic |

Release dates differ by a day between sources in a few cases.

## ⚠️ Read this before trusting any number

1. **Vendor-reported is not independent.** Labs often use their own harness and settings.
2. **Aggregators disagree.** The same model can differ by 10+ points (see SWE-bench Verified, and the two Artificial Analysis index versions).
3. **Newest models lag the leaderboards.** GPT-6.1 Sol and Sonnet 5.5 are 1–2 days old and missing from Arena and BenchLM.
4. **Saturated benchmarks.** AIME at 100% and GPQA at 96% no longer separate the frontier.
5. **Arena Elo measures preference, not correctness.**
6. **Prices and ranks change weekly.** Check the date on this sheet.
7. **Not covered:** Humanity's Last Exam and MMLU-Pro. I couldn't find consistent verifiable numbers, so they are left out rather than guessed. Gemini Pro-tier and Llama/Mistral flagship results are also missing from my sources.

## Sources

- [Artificial Analysis leaderboard](https://artificialanalysis.ai/leaderboards/models)
- [BenchLM.ai](https://benchlm.ai/), 2026-09-29
- [Arena text leaderboard](https://arena.ai/leaderboard/text), 2026-09-25
- [LLM-Stats](https://llm-stats.com/) and [SWE-bench Verified](https://llm-stats.com/benchmarks/swe-bench-verified)
- [SWE-bench Pro (Morph)](https://www.morphllm.com/swe-bench-pro)
- [September 2026 model updates (local-ai-zone)](https://local-ai-zone.github.io/blog/September_2026_AI_Model_Updates.html)
- [LLM Gateway timeline](https://llmgateway.io/timeline)
- [TeamDay model comparison](https://www.teamday.ai/blog/best-ai-models-2026)

## Contributing

PRs welcome. Every number needs a source link and date. Mark vendor-reported figures as such. No estimates or numbers from memory.

## License

MIT
