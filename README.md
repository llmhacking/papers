# LLM for Vulnerability Detection

A curated collection of academic papers on using Large Language Models for software vulnerability detection, analysis, and remediation.

## 📖 Categories

| # | Category | Count | Key Focus |
|---|----------|-------|-----------|
| [1](#1-prompt-engineering--agent-based-pe) | Prompt Engineering | Prompt Engineering & Agent-based | 17 | Agent-based | 31 | Prompting and LLM agents for vuln detection |
| [2](#2-fine-tuning-ft) | Fine-Tuning | 33 | Supervised fine-tuning on vulnerable code |
| [3](#3-rag--knowledge-augmented-rag) | RAG & Knowledge-Augmented | 5 | Retrieval-augmented & CPG-guided vuln detection |
| [4](#4-evaluation--benchmarks-ev) | Evaluation & Benchmarks | 5 | Benchmarking & evaluation frameworks |
| [5](#5-code-generation-gen) | Code Generation | 2 | Secure code generation |
| [6](#6-code-understanding-understand) | Code Understanding | 3 | Code comprehension with LLMs |
| [7](#7-surveys--overviews-study) | Surveys | Surveys & Overviews | 1 | Overviews | 5 | Survey & overview |
| [8](#8-others) | Others | 1 | Misc approaches |

---


## 1. Prompt Engineering & Agent-based (pe)

| # | Paper | Venue | Year | File |
|---|-------|-------|------|------|
| pe1 | Fu, M. et al. — ChatGPT for Vulnerability Detection, Classification, and Repair: How Far Are We? | APSEC | 2023 | [`pe/1.pdf`](pe/1.pdf) |
| pe2 | Khare, A. et al. — [Understanding the Effectiveness of Large Language Models in Detecting Security Vulnerabilities](https://arxiv.org/abs/2311.16169) | arXiv | 2023 | [`pe/2.pdf`](pe/2.pdf) |
| pe3 | Ni, C. et al. — [Learning-based Models for Vulnerability Detection: An Extensive Study](https://arxiv.org/abs/2408.07526) | arXiv | 2024 | [`pe/3.pdf`](pe/3.pdf) |
| pe4 | Purba, M. D. et al. — [Software Vulnerability Detection Using Large Language Models](https://ieeexplore.ieee.org/document/10301302) | ISSRE Workshops | 2023 | [`pe/4.txt`](pe/4.txt) |
| pe5 | Yin, X. — [Pros and Cons! Evaluating ChatGPT on Software Vulnerability](https://arxiv.org/abs/2404.03994) | CoRR | 2024 | [`pe/5.pdf`](pe/5.pdf) |
| pe6 | Zhang, C. et al. — [Prompt-Enhanced Software Vulnerability Detection Using ChatGPT](https://arxiv.org/abs/2308.12697) | arXiv | 2023 | [`pe/6.pdf`](pe/6.pdf) |
| pe7 | Zhou, X. et al. — [Comparison of Static Application Security Testing Tools and Large Language Models for Repo-Level Vulnerability Detection](https://arxiv.org/abs/2407.16235) | arXiv | 2024 | [`pe/7.pdf`](pe/7.pdf) |
| pe8 | Zhou, X., Zhang, T., Lo, D. — Large Language Model for Vulnerability Detection: Emerging Results and Future Directions | ICSE NIER | 2024 | [`pe/8.pdf`](pe/8.pdf) |
| pe9 | Wang, C. et al. — [LLMDFA: Analyzing Dataflow in Code with Large Language Models](https://papers.nips.cc/paper_files/paper/2024/hash/...) | NeurIPS | 2024 | — |
| pe10 | Li, Z. et al. — [IRIS: LLM-Assisted Static Analysis for Detecting Security Vulnerabilities](https://arxiv.org/abs/2405.17238) | ICLR | 2025 | [`pe/iris.pdf`](pe/iris.pdf) |
| pe11 | Guo, J. et al. — [RepoAudit: An Autonomous LLM-Agent for Repository-Level Code Auditing](https://arxiv.org/abs/2501.18160) | ICML | 2025 | [`pe/repoaudit.pdf`](pe/repoaudit.pdf) |
| pe12 | Liu, P. et al. — [LATTE: LLM-Powered Static Binary Taint Analysis](https://arxiv.org/abs/2310.08275) | TOSEM | 2025 | [`pe/latte.pdf`](pe/latte.pdf) |
| pe13 | Li, Y. et al. — [AutoBug: Large Language Model Powered Symbolic Execution](https://arxiv.org/abs/2505.13452) | OOPSLA | 2025 | [`pe/autobug.pdf`](pe/autobug.pdf) |
| pe14 | Li, H. et al. — [LLIFT: Enhancing Static Analysis for Practical Bug Detection: An LLM-Integrated Approach](https://dl.acm.org/doi/10.1145/3649828) | OOPSLA | 2024 | [`pe/llift.pdf`](pe/llift.pdf) |
| pe15 | Lin, H. et al. — [ACTaint: Agent-Based Taint Analysis for Access Control Vulnerabilities in Smart Contracts](https://doi.org/10.1109/ase63991.2025.00210) | ASE | 2025 | [`pe/actaint.txt`](pe/actaint.txt) |
| pe16 | — **Hyperion** (ICSE 2025) | ICSE | 2025 | — ❌ |
| pe17 | — **GPTAid** (NDSS 2025) | NDSS | 2025 | — ❌ |
| pe18 | Wang, Z. et al. — [Revelio: Cost-Efficient Agentic Memory Safety Vulnerability Detection For Repository-Scale Codebases](https://arxiv.org/abs/2606.22263) | arXiv | 2026 | — |
| pe19 | — [Code-Augur: Agentic Vulnerability Detection via Specification Inference](https://arxiv.org/abs/2606.18619) | arXiv | 2026 | — |
| pe20 | — [Security in a Workflow: Exploring Role-Based Agentic Architectures for Vulnerability Handling](https://arxiv.org/abs/2606.14261) | arXiv | 2026 | — |
| pe21 | — [FuzzingBrain V2: A Multi-Agent LLM System for Automated Vulnerability Discovery and Reproduction](https://arxiv.org/abs/2605.21779) | arXiv | 2025 | — |
| pe22 | — [MulVul: Retrieval-augmented Multi-Agent Code Vulnerability Detection via Cross-Model Prompt Evolution](https://arxiv.org/abs/2601.18847) | arXiv | 2026 | — |
| pe23 | — [AgenticSCR: An Autonomous Agentic Secure Code Review for Immature Vulnerabilities Detection](https://arxiv.org/abs/2601.19138) | arXiv | 2026 | — |
| pe24 | — [Synthesizing Multi-Agent Harnesses for Vulnerability Discovery](https://arxiv.org/abs/2604.20801) | arXiv | 2026 | — |
| pe25 | — [VulnLLM-R: Specialized Reasoning LLM with Agent Scaffold for Vulnerability Detection](https://arxiv.org/abs/2512.07533) | arXiv | 2025 | — |
| pe26 | — [PromptAudit: Auditing Prompt Sensitivity in LLM-Based Vulnerability Detection](https://arxiv.org/abs/2605.24171) | arXiv | 2025 | — |
| pe27 | — [Antaeus: Hunting Repository-Level Logic Vulnerabilities via Context-Grounded LLM Reasoning](https://arxiv.org/abs/2607.01138) | arXiv | 2026 | — |
| pe28 | — [Three Heads Are Better Than One: A Multi-perspective Reasoning Framework for Enhanced Vulnerability Detection](https://arxiv.org/abs/2605.18153) | arXiv | 2025 | — |
| pe29 | — [Veritas: A Semantically Grounded Agentic Framework for Memory Corruption Vulnerability Detection in Binaries](https://arxiv.org/abs/2605.15097) | arXiv | 2025 | — |
| pe30 | — [Sifting the Noise: A Comparative Study of LLM Agents in Vulnerability False Positive Filtering](https://arxiv.org/abs/2601.22952) | arXiv | 2026 | — |
| pe31 | — [Combining Fine-Tuning and LLM-based Agents for Intuitive Smart Contract Auditing with Justifications](https://arxiv.org/abs/2403.16073) | ICSE | 2025 | — |
| pe32 | — [SAEL: Leveraging Large Language Models with Adaptive Mixture-of-Experts for Smart Contract Vulnerability Detection](https://arxiv.org/abs/2507.22371) | arXiv | 2025 | — |
| pe33 | — [MOS: Towards Effective Smart Contract Vulnerability Detection through Mixture-of-Experts Tuning of Large Language Models](https://arxiv.org/abs/2504.12234) | arXiv | 2025 | — |
| pe35 | 🎯 — [QLPro: Automated Code Vulnerability Discovery via LLM and Static Code Analysis Integration](https://arxiv.org/abs/2506.23644) | arXiv | 2025 | 📌 TODO |
| pe36 | 🎯 — [CVE-Factory: Scaling Expert-Level Agentic Tasks for Code Security Vulnerability](https://arxiv.org/abs/2602.03012) | arXiv | 2026 | 📌 TODO |
| pe37 | 🎯 — [CQLLM: LLM-Driven CodeQL Security Vulnerability Detection Code Auto-Generation](https://preprints.org) | Preprints | 2025 | 📌 TODO |
| pe38 | 🎯 — [Vulnhalla: CodeQL + LLM Post-Processing for Vuln Detection](https://www.cyberark.com) | CyberArk | 2025 | 📌 TODO |
| pe39 | 🎯 — [OpenAI Aardvark: Agentic Security Researcher](https://openai.com/index/aardvark/) | OpenAI | 2025 | 📌 TODO |
| pe40 | 🎯 — [D-CIPHER: Dynamic Collaborative Multi-Agent System for Offensive Security](https://arxiv.org/abs/2502.10931) | arXiv | 2025 | 📌 TODO 🔴 Multi-Agent Pentesting |
| pe41 | 🎯 — [Decoupling Reconnaissance and Exploitation: LLM-Based Web Penetration Testing](https://arxiv.org/abs/2606.25332) | arXiv | 2026 | 📌 TODO 🔴 Multi-Agent Pentesting |
| pe42 | 🎯 — [SIVA: Self-Improving Vulnerability Agent — Research Direction](https://openreview.net) | OpenReview | 2025 | 📌 TODO 🔵 Self-Improving Agent |
| pe43 | — [R2Vul: Learning to Reason about Software Vulnerabilities with RL and Structured Reasoning Distillation](https://arxiv.org/abs/2504.04699) | arXiv | 2025 | — |
| pe44 | — [Multi-role Consensus through LLMs Discussions for Vulnerability Detection](https://arxiv.org/abs/2403.14274) | arXiv | 2024 | — |
| pe45 | — [Chain-of-Thought Prompting of LLMs for Discovering and Fixing Software Vulnerabilities](https://arxiv.org/abs/2402.17230) | arXiv | 2024 | — |
| pe46 | — [VULPO: Context-Aware Vulnerability Detection via on-Policy LLM Optimization](https://arxiv.org/abs/2511.11896) | arXiv | 2025 | — |
| pe47 | — [Specification-Guided Vulnerability Detection with Large Language Models](https://arxiv.org/abs/2511.04014) | arXiv | 2025 | — |
| pe48 | — [One-for-All Does Not Work! Enhancing Vulnerability Detection by Mixture-of-Experts (MoE)](https://arxiv.org/abs/2501.16454) | arXiv | 2025 | — |
| pe49 | — [VulTriage: Triple-Path Context Augmentation for LLM-Based Vulnerability Detection](https://arxiv.org/abs/2605.09461) | arXiv | 2026 | — |
| pe50 | — [QRS: A Rule-Synthesizing Neuro-Symbolic Triad for Autonomous Vulnerability Discovery](https://arxiv.org/abs/2602.09774) | arXiv | 2026 | — |
| pe51 | — [From Large to Mammoth: A Comparative Evaluation of LLMs in Vulnerability Detection](https://www.ndss-symposium.org/ndss-paper/from-large-to-mammoth-a-comparative-evaluation-of-large-language-models-in-vulnerability-detection/) | NDSS | 2025 | — |
| pe52 | — [VulnGym: A Real-World, Project-Level Vulnerability Benchmark for White-Box Vulnerability-Hunting Agents](https://github.com/Tencent/VulnGym) | — | 2026 | — |
| pe53 | — [CVE-Bench: Benchmarking LLM-based SE Agent's Ability to Repair Real-World CVEs](https://aclanthology.org/2025.naacl-long.212/) | NAACL | 2025 | — |
| pe54 | — [Everything you wanted to know about LLM-based vulnerability detection but were afraid to ask](https://arxiv.org/abs/2504.13474) | arXiv | 2025 | — |

### 📊 Data-Centric Innovations

| # | Paper | Venue | Year | File |
|---|-------|-------|------|------|
| ft1 | Wen, X. et al. — When Less Is Enough: Positive and Unlabeled Learning Model for Vulnerability Detection | ASE | 2023 | [`ft/1.pdf`](ft/1.pdf) |
| ft2 | Kuang, H. et al. — [Leveraging User-Defined Identifiers for Counterfactual Data Generation in Source Code Vulnerability Detection](https://ieeexplore.ieee.org/document/10356404) | SCAM | 2023 | [`ft/2.txt`](ft/2.txt) |
| ft3 | Ding, Y. et al. — [Vulnerability Detection with Code Language Models: How Far Are We?](https://arxiv.org/abs/2403.18624) | arXiv | 2024 | [`ft/3.pdf`](ft/3.pdf) |
| ft4 | Yang, X. et al. — Does Data Sampling Improve Deep Learning-Based Vulnerability Detection? Yeas! and Nays! | ICSE | 2023 | [`ft/4.pdf`](ft/4.pdf) |

### 🔬 Combining with Program Analysis

| # | Paper | Venue | Year | File |
|---|-------|-------|------|------|
| ft5 | Peng, T. et al. — PTLVD: Program Slicing and Transformer-Based Line-Level Vulnerability Detection System | SCAM | 2023 | — |
| ft6 | Zhang, J. et al. — [Vulnerability Detection by Learning from Syntax-Based Execution Paths of Code](https://github.com/llmhacking/papers) | IEEE TSE | 2023 | [`ft/6.pdf`](ft/6.pdf) |
| ft7 | Wang, H. et al. — Combining Structured Static Code Information and Dynamic Symbolic Traces for Software Vulnerability Prediction | ICSE | 2024 | [`ft/7.pdf`](ft/7.pdf) |
| ft8 | Liu, Z. et al. — Pre-Training by Predicting Program Dependencies for Vulnerability Analysis Tasks | ICSE | 2024 | [`ft/8.pdf`](ft/8.pdf) |
| ft9 | Tran, H.-C. et al. — DetectVul: A Statement-Level Code Vulnerability Detection for Python | FGCS | 2024 | — |
| ft10 | Weng, C. et al. — [MATSVD: Boosting Statement-Level Vulnerability Detection via Dependency-Based Attention](https://dl.acm.org/doi/10.1145/3671016.3674807) | Internetware | 2024 | [`ft/10.txt`](ft/10.txt) |

### 🧩 LLM + Other DL Modules

| # | Paper | Venue | Year | File |
|---|-------|-------|------|------|
| ft11 | Ziems, N., Wu, S. — Security Vulnerability Detection Using Deep Learning Natural Language Processing | INFOCOM Workshops | 2021 | — |
| ft12 | Tang, W. et al. — CSGVD: A Deep Learning Approach Combining Sequence and Graph Embedding for Source Code Vulnerability Detection | J. Syst. Softw. | 2023 | — |
| ft13 | Jiang, Z. et al. — DFEPT: Data Flow Embedding for Enhancing Pre-Trained Model Based Vulnerability Detection | Internetware | 2024 | — |
| ft14 | Yang, A. Z. et al. — [Security Vulnerability Detection with Multitask Self-Instructed Fine-Tuning of Large Language Models](https://arxiv.org/abs/2406.05892) | arXiv | 2024 | — |

### 🏗️ Domain-Specific Pre-Training

| # | Paper | Venue | Year | File |
|---|-------|-------|------|------|
| ft15 | Hanif, H., Maffeis, S. — VulBERTa: Simplified Source Code Pre-Training for Vulnerability Detection | IJCNN | 2022 | — |
| ft16 | Ni, C. et al. — Distinguishing Look-Alike Innocent and Vulnerable Code by Subtle Semantic Representation Learning and Explanation | ESEC/FSE | 2023 | — |
| ft17 | Wang, H. et al. — Combining Structured Static Code Information and Dynamic Symbolic Traces | ICSE | 2024 | — |
| ft18 | Liu, Z. et al. — Pre-Training by Predicting Program Dependencies | ICSE | 2024 | — |
| ft19 | Ding, Y. et al. — [Vulnerability Detection with Code Language Models: How Far Are We?](https://arxiv.org/abs/2403.18624) | arXiv | 2024 | — |
| ft20 | Steenhoek, B. et al. — [Do Language Models Learn Semantics of Code? A Case Study in Vulnerability Detection](https://arxiv.org/abs/2311.04109) | arXiv | 2023 | — |

### 🔗 Causal Learning

| # | Paper | Venue | Year | File |
|---|-------|-------|------|------|
| ft21 | Mahbubur Rahman, M. et al. — Towards Causal Deep Learning for Vulnerability Detection | ICSE | 2024 | — |

### ⚙️ Default Fine-Tuning

| # | Paper | Venue | Year | File |
|---|-------|-------|------|------|
| ft22 | Fu, M., Tantithamthavorn, C. — LineVul: A Transformer-Based Line-Level Vulnerability Prediction | MSR | 2022 | — |
| ft23 | Thapa, C. et al. — Transformer-Based Language Models for Software Vulnerability Detection | ACSAC | 2022 | — |
| ft24 | Fu, M. et al. — AiBugHunter: A Practical Tool for Predicting, Classifying and Repairing Software Vulnerabilities | EMSE | 2024 | — |
| ft25 | Sejfia, A. et al. — Toward Improved Deep Learning-Based Vulnerability Detection | ICSE | 2024 | — |
| ft26 | Risse, N., Böhme, M. — Uncovering the Limits of Machine Learning for Automatic Vulnerability Detection | USENIX Security | 2024 | — |
| ft27 | Steenhoek, B. et al. — An Empirical Study of Deep Learning Models for Vulnerability Detection | ICSE | 2023 | — |
| ft28 | Chen, Y. et al. — DiverseVul: A New Vulnerable Source Code Dataset for Deep Learning Based Vulnerability Detection | RAID | 2023 | — |
| ft29 | Li, Z. et al. — On the Effectiveness of Function-Level Vulnerability Detectors for Inter-Procedural Vulnerabilities | ICSE | 2024 | — |
| ft30 | Croft, R. et al. — Data Quality for Software Vulnerability Datasets | ICSE | 2023 | — |
| ft31 | Le, T. H. M. et al. — Are Latent Vulnerabilities Hidden Gems for Software Vulnerability Prediction? | MSR | 2024 | — |
| ft32 | Zhou, X. et al. — [Comparison of SAST Tools and LLMs for Repo-Level Vulnerability Detection](https://arxiv.org/abs/2407.16235) | arXiv | 2024 | — |
| ft33 | Shestov, A. et al. — [Fine-Tuning Large Language Models for Vulnerability Detection](https://arxiv.org/abs/2401.17010) | CoRR | 2024 | — |

---

## 3. RAG & Knowledge-Augmented (rag)

| # | Paper | Venue | Year | File |
|---|-------|-------|------|------|
| rag1 | Liu, Z. et al. — [Software Vulnerability Detection with GPT and In-Context Learning](https://ieeexplore.ieee.org/document/10381286) | DSC | 2023 | [`rag/1.txt`](rag/1.txt) |
| rag2 | Zhou, X., Zhang, T., Lo, D. — Large Language Model for Vulnerability Detection: Emerging Results and Future Directions | ICSE NIER | 2024 | [`rag/2.pdf`](rag/2.pdf) |
| rag3 | Du, X. et al. — [Vul-RAG: Enhancing LLM-Based Vulnerability Detection via Knowledge-Level RAG](https://arxiv.org/abs/2406.11147) | CoRR | 2024 | [`rag/3.pdf`](rag/3.pdf) |
| rag4 | Wen, X. et al. — [VulEval: Towards Repository-Level Evaluation of Software Vulnerability Detection](https://arxiv.org/abs/2404.15596) | CoRR | 2024 | [`rag/4.pdf`](rag/4.pdf) |
| rag5 | Lekssays, A. et al. — [LLMxCPG: Context-Aware Vulnerability Detection Through Code Property Graph-Guided Large Language Models](https://www.usenix.org/conference/usenixsecurity25/presentation/lekssays) | USENIX Security | 2025 | [`pe/llmxcpg.pdf`](pe/llmxcpg.pdf) |

---

## 4. Evaluation & Benchmarks (ev)

| # | Paper | Year | File |
|---|-------|------|------|
| ev1 | [LLM4Vuln: A Unified Evaluation Framework for Decoupling and Enhancing LLMs' Vulnerability Reasoning](https://arxiv.org/pdf/2401.16185) | 2024 | — |
| ev2 | [LSAST: Enhancing Cybersecurity through LLM-Supported Static Application Security Testing](https://arxiv.org/html/2409.15735v2) | 2024 | — |
| ev3 | CyberGym et al. — [CyberGym: Evaluating AI Agents' Real-World Cybersecurity Capabilities at Scale](https://arxiv.org/abs/2506.02548) | 2025 | — |
| ev4 | Zhun Wang et al. — [ExploitGym: Can AI Agents Turn Security Vulnerabilities into Real Attacks?](https://arxiv.org/abs/2605.11086) | 2025 | — |
| ev5 | Tianneng Shi et al. — [CyberGym-E2E: Scalable Real-World Benchmark for AI Agents' End-to-End Cybersecurity Capabilities](https://arxiv.org/abs/2606.04460) | 2025 | — |

---

## 5. Code Generation (gen)

| # | Paper | Year |
|---|-------|------|
| g1 | [Improving LLM Code Generation with Grammar Augmentation](https://arxiv.org/html/2403.01632v1) | 2024 |
| g2 | [A Survey on Large Language Models for Code Generation](https://arxiv.org/pdf/2406.00515) | 2024 |

---

## 6. Code Understanding (understand)

| # | Paper | Year |
|---|-------|------|
| u1 | [Testing the Effect of Code Documentation on Large Language Model Code Understanding](https://arxiv.org/pdf/2404.03114) | 2024 |
| u2 | [Using an LLM to Help With Code Understanding](https://arxiv.org/html/2307.08177v3) | 2023 |
| u3 | [Automatic Semantic Augmentation of Language Model Prompts (for Code Summarization)](https://arxiv.org/pdf/2304.06815) | 2023 |

---

## 7. Surveys & Overviews (study)

| # | Paper | Year | File |
|---|-------|------|------|
| s1 | [Large Language Model for Vulnerability Detection and Repair: Literature Review and the Road Ahead](https://arxiv.org/pdf/2404.02525) | 2024 | — |
| s2 | [LLMs in Software Security: A Survey of Vulnerability Detection Techniques and Insights](https://arxiv.org/abs/2502.07049) | 2025 | — |
| s3 | [A Systematic Literature Review on Detecting Software Vulnerabilities with Large Language Models](https://arxiv.org/abs/2507.22659) | 2025 | — |
| s4 | Chen, Y. et al. — [Software Defect Detection Using Large Language Models: A Literature Review](https://link.springer.com/article/10.1007/s11704-025-40672-2) | 2026 | — |
| s5 | [When Labels Are Scarce: A Systematic Mapping of Label-Efficient Code Vulnerability Detection](https://arxiv.org/abs/2604.00079) | 2026 | — |

---

## 8. Others

| # | Paper | Year |
|---|-------|------|
| o1 | [How Well Do Large Language Models Serve as End-to-End Secure Code Producers?](https://arxiv.org/pdf/2408.10495) | 2024 |

---

## 📁 Repository Structure

```
papers/
├── README.md          # This file — full index with hyperlinks
├── .gitignore
├── pe/                # Prompt Engineering papers
├── ft/                # Fine-Tuning papers
├── rag/               # RAG papers
├── ev/                # Evaluation papers
├── study/             # Survey / overview
├── gen/               # Code generation
└── understand/        # Code understanding
```

Papers in `pe/`, `ft/`, and `rag/` are stored as either:
- **`.pdf`** — full paper downloaded (for offline access)
- **`.txt`** — link to official publication (DOI or IEEE/ACM)

---

> Maintained by [@llmhacking](https://github.com/llmhacking)
