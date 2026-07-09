# LLM for Vulnerability Detection

A curated collection of academic papers on using Large Language Models for software vulnerability detection, analysis, and remediation.

## 📖 Categories

| # | Category | Count | Key Focus |
|---|----------|-------|-----------|
| [1](#1-prompt-engineering--knowledge-augmented-pe) | Prompt Engineering & Knowledge-Augmented | 27 | Prompting, CoT, RAG, CPG-guided reasoning |
| [2](#2-agent-based-systems-agent) | Agent-based Systems | 29 | Autonomous agents, multi-agent, self-improving agents |
| [3](#3-fine-tuning-ft) | Fine-Tuning | 33 | Supervised fine-tuning on vulnerable code |
| [4](#4-evaluation--benchmarks-ev) | Evaluation & Benchmarks | 10 | Benchmarking & evaluation frameworks |
| [5](#5-code-generation-gen) | Code Generation | 2 | Secure code generation |
| [6](#6-code-understanding-understand) | Code Understanding | 3 | Code comprehension with LLMs |
| [7](#7-surveys--overviews-study) | Surveys & Overviews | 5 | Survey & overview |
| [8](#8-others) | Others | 1 | Misc approaches |

---

> **Sections 1–4** focus on vulnerability detection. **Sections 5–6** cover adjacent areas (code generation, code understanding) that are relevant but not directly about vulnerability detection.

---

## 1. Prompt Engineering & Knowledge-Augmented (pe)

Prompt设计、CoT推理、RAG检索增强、CPG/图结构引导的大模型漏洞检测。

| # | Paper | Venue | Year | 说明 |
|---|-------|-------|------|------|
| pe1 | Fu, M. et al. — ChatGPT for Vulnerability Detection, Classification, and Repair: How Far Are We? | APSEC | 2023 | 🧪 零样本评估ChatGPT在漏洞检测/分类/修复上的能力边界 |
| pe2 | Khare, A. et al. — [Understanding the Effectiveness of LLMs in Detecting Security Vulnerabilities](https://arxiv.org/abs/2311.16169) | arXiv | 2023 | 🧪 系统评估LLM检测安全漏洞的有效性及局限性 |
| pe3 | Ni, C. et al. — [Learning-based Models for Vulnerability Detection: An Extensive Study](https://arxiv.org/abs/2408.07526) | arXiv | 2024 | 📊 大规模对比学习式漏洞检测模型，覆盖多种架构 |
| pe4 | Purba, M. D. et al. — [Software Vulnerability Detection Using Large Language Models](https://ieeexplore.ieee.org/document/10301302) | ISSRE Workshops | 2023 | 🧪 LLM用于软件漏洞检测的可行性验证 |
| pe5 | Yin, X. — [Pros and Cons! Evaluating ChatGPT on Software Vulnerability](https://arxiv.org/abs/2404.03994) | CoRR | 2024 | 🧪 ChatGPT在漏洞检测上的优缺点分析 |
| pe6 | Zhang, C. et al. — [Prompt-Enhanced Software Vulnerability Detection Using ChatGPT](https://arxiv.org/abs/2308.12697) | arXiv | 2023 | 💡 用prompt增强ChatGPT的漏洞检测能力 |
| pe7 | Zhou, X. et al. — [Comparison of SAST Tools and LLMs for Repo-Level Vulnerability Detection](https://arxiv.org/abs/2407.16235) | arXiv | 2024 | 📊 SAST工具 vs LLM在仓库级漏洞检测上的对比 |
| pe8 | Zhou, X., Zhang, T., Lo, D. — Large Language Model for Vulnerability Detection: Emerging Results and Future Directions | ICSE NIER | 2024 | 🔄 LLM漏洞检测的初步成果和未来方向 |
| pe9 | Wang, C. et al. — [LLMDFA: Analyzing Dataflow in Code with Large Language Models](https://papers.nips.cc/paper_files/paper/2024/hash/...) | NeurIPS | 2024 | ⚙️🔗 LLM做数据流分析，NeurIPS顶会。🔥 关键论文 |
| pe10 | — [VulnLLM-R: Specialized Reasoning LLM with Agent Scaffold for Vulnerability Detection](https://arxiv.org/abs/2512.07533) | arXiv | 2025 | 🤖🧠 专用推理LLM + Agent框架 |
| pe11 | — [PromptAudit: Auditing Prompt Sensitivity in LLM-Based Vulnerability Detection](https://arxiv.org/abs/2605.24171) | arXiv | 2025 | 💡 Prompt敏感性审计 |
| pe12 | — [Antaeus: Hunting Repository-Level Logic Vulns via Context-Grounded LLM Reasoning](https://arxiv.org/abs/2607.01138) | arXiv | 2026 | 🧠 上下文锚定推理，仓库级逻辑漏洞挖掘 |
| pe13 | — [Three Heads Are Better Than One: Multi-perspective Reasoning for Enhanced Vuln Detection](https://arxiv.org/abs/2605.18153) | arXiv | 2025 | 🧠 多视角协同推理 |
| pe14 | — [R2Vul: Learning to Reason about Vulns with RL and Structured Reasoning Distillation](https://arxiv.org/abs/2504.04699) | arXiv | 2025 | 🧠🤖 RL + 结构化推理蒸馏 |
| pe15 | — [Chain-of-Thought Prompting of LLMs for Discovering and Fixing Software Vulns](https://arxiv.org/abs/2402.17230) | arXiv | 2024 | 💡 CoT推理用于漏洞发现和修复 |
| pe16 | — [Multi-role Consensus through LLMs Discussions for Vulnerability Detection](https://arxiv.org/abs/2403.14274) | arXiv | 2024 | 🤖 多角色LLM讨论达成共识检测漏洞 |
| pe17 | — [VULPO: Context-Aware Vulnerability Detection via on-Policy LLM Optimization](https://arxiv.org/abs/2511.11896) | arXiv | 2025 | 🧠 on-policy优化LLM做上下文感知漏洞检测 |
| pe18 | — [Specification-Guided Vulnerability Detection with Large Language Models](https://arxiv.org/abs/2511.04014) | arXiv | 2025 | 📋 用规约/规范引导LLM检测漏洞 |
| pe19 | — [One-for-All Does Not Work! Enhancing Vuln Detection by Mixture-of-Experts](https://arxiv.org/abs/2501.16454) | arXiv | 2025 | 🧩 MoE专家混合模型增强漏洞检测 |
| pe20 | — [VulTriage: Triple-Path Context Augmentation for LLM-Based Vuln Detection](https://arxiv.org/abs/2605.09461) | arXiv | 2026 | 💡 三路径上下文增强 |
| pe21 | — [QRS: A Rule-Synthesizing Neuro-Symbolic Triad for Autonomous Vulnerability Discovery](https://arxiv.org/abs/2602.09774) | arXiv | 2026 | 🧠 神经符号系统自动合成规则发现漏洞 |
| pe22 | — [Everything you wanted to know about LLM-based vuln detection but were afraid to ask](https://arxiv.org/abs/2504.13474) | arXiv | 2025 | 🔄 LLM漏洞检测综述/问答式梳理 |
| pe23 | Liu, Z. et al. — [Software Vulnerability Detection with GPT and In-Context Learning](https://ieeexplore.ieee.org/document/10381286) | DSC | 2023 | 💡🧪 GPT + ICL少样本漏洞检测 |
| pe24 | Zhou, X., Zhang, T., Lo, D. — Large Language Model for Vulnerability Detection: Emerging Results and Future Directions | ICSE NIER | 2024 | ⚠️ 与pe8重复 |
| pe25 | Du, X. et al. — [Vul-RAG: Enhancing LLM-Based Vulnerability Detection via Knowledge-Level RAG](https://arxiv.org/abs/2406.11147) | CoRR | 2024 | 🔗 RAG知识检索增强漏洞检测。🔥 关键论文 |
| pe26 | Wen, X. et al. — [VulEval: Towards Repository-Level Evaluation of Software Vulnerability Detection](https://arxiv.org/abs/2404.15596) | CoRR | 2024 | 📊 仓库级漏洞检测评估框架 |
| pe27 | Lekssays, A. et al. — [LLMxCPG: Context-Aware Vulnerability Detection Through Code Property Graph-Guided LLMs](https://www.usenix.org/conference/usenixsecurity25/presentation/lekssays) | USENIX Security | 2025 | ⚙️🔗 CPG引导LLM，USENIX Security顶会。🔥 关键论文 |

---

## 2. Agent-based Systems (agent)

基于智能体/多智能体架构的自动化漏洞检测与修复系统。

| # | Paper | Venue | Year | 说明 |
|---|-------|-------|------|------|
| ag1 | Li, Z. et al. — [IRIS: LLM-Assisted Static Analysis for Detecting Security Vulnerabilities](https://arxiv.org/abs/2405.17238) | ICLR | 2025 | 🤖 ICLR顶会。LLM辅助静态分析，agent + SAST协同。🔥 关键论文 |
| ag2 | Guo, J. et al. — [RepoAudit: An Autonomous LLM-Agent for Repository-Level Code Auditing](https://arxiv.org/abs/2501.18160) | ICML | 2025 | 🤖 ICML顶会。仓库级自主审计agent。🔥 关键论文 |
| ag3 | Liu, P. et al. — [LATTE: LLM-Powered Static Binary Taint Analysis](https://arxiv.org/abs/2310.08275) | TOSEM | 2025 | ⚙️ LLM增强二进制污点分析。🔥 关键论文 |
| ag4 | Li, Y. et al. — [AutoBug: Large Language Model Powered Symbolic Execution](https://arxiv.org/abs/2505.13452) | OOPSLA | 2025 | ⚙️ LLM驱动的符号执行，OOPSLA顶会。🔥 关键论文 |
| ag5 | Li, H. et al. — [LLIFT: Enhancing Static Analysis for Practical Bug Detection: An LLM-Integrated Approach](https://dl.acm.org/doi/10.1145/3649828) | OOPSLA | 2024 | ⚙️ OOPSLA顶会。LLM增强静态分析的实用bug检测。🔥 关键论文 |
| ag6 | Lin, H. et al. — [ACTaint: Agent-Based Taint Analysis for Access Control Vulns in Smart Contracts](https://doi.org/10.1109/ase63991.2025.00210) | ASE | 2025 | 🤖📝 智能合约访问控制污点分析agent |
| ag7 | — **Hyperion** (ICSE 2025) | ICSE | 2025 | ❌ 未找到PDF |
| ag8 | — **GPTAid** (NDSS 2025) | NDSS | 2025 | ❌ 未找到PDF |
| ag9 | Wang, Z. et al. — [Revelio: Cost-Efficient Agentic Memory Safety Vuln Detection for Repo-Scale Codebases](https://arxiv.org/abs/2606.22263) | arXiv | 2026 | 🤖 仓库级内存安全漏洞检测agent，注重成本效率 |
| ag10 | — [Code-Augur: Agentic Vulnerability Detection via Specification Inference](https://arxiv.org/abs/2606.18619) | arXiv | 2026 | 🤖 规约推断的agent漏洞检测 |
| ag11 | — [Security in a Workflow: Exploring Role-Based Agentic Architectures for Vuln Handling](https://arxiv.org/abs/2606.14261) | arXiv | 2026 | 🤖 基于角色的多agent架构 |
| ag12 | — [FuzzingBrain V2: A Multi-Agent LLM System for Automated Vuln Discovery and Reproduction](https://arxiv.org/abs/2605.21779) | arXiv | 2025 | 🤖 多agent自动化漏洞发现与复现 |
| ag13 | — [MulVul: Retrieval-augmented Multi-Agent Code Vuln Detection via Cross-Model Prompt Evolution](https://arxiv.org/abs/2601.18847) | arXiv | 2026 | 🤖🔗 RAG增强的多agent跨模型prompt进化 |
| ag14 | — [AgenticSCR: An Autonomous Agentic Secure Code Review for Immature Vulns Detection](https://arxiv.org/abs/2601.19138) | arXiv | 2026 | 🤖 自主代码审查agent |
| ag15 | — [Synthesizing Multi-Agent Harnesses for Vulnerability Discovery](https://arxiv.org/abs/2604.20801) | arXiv | 2026 | 🤖 多agent编排框架 |
| ag16 | — [Veritas: A Semantically Grounded Agentic Framework for Memory Corruption Vuln Detection in Binaries](https://arxiv.org/abs/2605.15097) | arXiv | 2025 | 🤖⚙️ 二进制内存损坏漏洞agent框架 |
| ag17 | — [Sifting the Noise: LLM Agents in Vulnerability False Positive Filtering](https://arxiv.org/abs/2601.22952) | arXiv | 2026 | 🤖🎯 LLM agent做漏洞误报过滤 |
| ag18 | — [Combining Fine-Tuning and LLM-based Agents for Smart Contract Auditing](https://arxiv.org/abs/2403.16073) | ICSE | 2025 | 🤖🎯 微调 + agent结合的智能合约审计 |
| ag19 | — [SAEL: Adaptive Mixture-of-Experts for Smart Contract Vulnerability Detection](https://arxiv.org/abs/2507.22371) | arXiv | 2025 | 🧩📝 自适应MoE智能合约漏洞检测 |
| ag20 | — [MOS: MoE Tuning of LLMs for Smart Contract Vulnerability Detection](https://arxiv.org/abs/2504.12234) | arXiv | 2025 | 🧩📝 MoE微调智能合约漏洞检测 |
| ag21 | 🎯 — [QLPro: Automated Code Vulnerability Discovery via LLM and Static Code Analysis](https://arxiv.org/abs/2506.23644) | arXiv | 2025 | 🎯 TODO · LLM + CodeQL结合，CodeQL自动化漏洞挖掘 |
| ag22 | 🎯 — [CVE-Factory: Scaling Expert-Level Agentic Tasks for Code Security Vulnerability](https://arxiv.org/abs/2602.03012) | arXiv | 2026 | 🎯 TODO · 专家级agent任务规模化 |
| ag23 | 🎯 — [CQLLM: LLM-Driven CodeQL Security Vuln Detection Code Auto-Generation](https://preprints.org) | Preprints | 2025 | 🎯 TODO · LLM自动生成CodeQL查询 |
| ag24 | 🎯 — [Vulnhalla: CodeQL + LLM Post-Processing for Vuln Detection](https://www.cyberark.com) | CyberArk | 2025 | 🎯 TODO · CodeQL + LLM后处理 |
| ag25 | 🎯 — [OpenAI Aardvark: Agentic Security Researcher](https://openai.com/index/aardvark/) | OpenAI | 2025 | 🎯 TODO · OpenAI出的安全研究agent |
| ag26 | 🎯 — [D-CIPHER: Dynamic Collaborative Multi-Agent System for Offensive Security](https://arxiv.org/abs/2502.10931) | arXiv | 2025 | 🎯 TODO · 多agent攻防协同 |
| ag27 | 🎯 — [Decoupling Recon and Exploitation: LLM-Based Web Penetration Testing](https://arxiv.org/abs/2606.25332) | arXiv | 2026 | 🎯 TODO · Web渗透测试agent |
| ag28 | 🎯 — [SIVA: Self-Improving Vulnerability Agent — Research Direction](https://openreview.net) | OpenReview | 2025 | 🎯 TODO 🔄 自进化漏洞检测agent |
| ag29 | — [Ensembling Large Language Models for Code Vulnerability Detection](https://arxiv.org/abs/2509.12629) | arXiv | 2025 | 🧩 LLM集成/模型融合检测漏洞 |

---

## 3. Fine-Tuning (ft)

通过微调预训练语言模型进行漏洞检测，包括数据增强、程序分析融合、因果学习等方法。

### 📊 Data-Centric Innovations

数据为中心的创新：样本选择、反事实生成、数据采样策略。

| # | Paper | Venue | Year | 说明 |
|---|-------|-------|------|------|
| ft1 | Wen, X. et al. — When Less Is Enough: Positive and Unlabeled Learning Model for Vulnerability Detection | ASE | 2023 | 🧩 PU学习（正样本+无标签）做漏洞检测 |
| ft2 | Kuang, H. et al. — [Leveraging User-Defined Identifiers for Counterfactual Data Generation in Source Code Vulnerability Detection](https://ieeexplore.ieee.org/document/10356404) | SCAM | 2023 | 🧩 用标识符反事实数据增强漏洞检测 |
| ft3 | Ding, Y. et al. — [Vulnerability Detection with Code Language Models: How Far Are We?](https://arxiv.org/abs/2403.18624) | arXiv | 2024 | 📊 代码语言模型漏洞检测能力评估 |
| ft4 | Yang, X. et al. — Does Data Sampling Improve Deep Learning-Based Vulnerability Detection? Yeas! and Nays! | ICSE | 2023 | 🧩 数据采样策略对漏洞检测的影响分析 |

### 🔬 Combining with Program Analysis

静态分析+微调的混合方法：程序切片、执行路径、依赖预测。

| # | Paper | Venue | Year | 说明 |
|---|-------|-------|------|------|
| ft5 | Peng, T. et al. — PTLVD: Program Slicing and Transformer-Based Line-Level Vulnerability Detection System | SCAM | 2023 | ⚙️🔗 程序切片 + Transformer行级漏洞检测 |
| ft6 | Zhang, J. et al. — [Vulnerability Detection by Learning from Syntax-Based Execution Paths of Code](https://github.com/llmhacking/papers) | IEEE TSE | 2023 | ⚙️🔗 语法执行路径学习漏洞模式 |
| ft7 | Wang, H. et al. — Combining Structured Static Code Information and Dynamic Symbolic Traces for Software Vulnerability Prediction | ICSE | 2024 | ⚙️🔗 静态结构+动态符号轨迹联合预测 |
| ft8 | Liu, Z. et al. — Pre-Training by Predicting Program Dependencies for Vulnerability Analysis Tasks | ICSE | 2024 | 🎯 预训练预测程序依赖用于漏洞分析 |
| ft9 | Tran, H.-C. et al. — DetectVul: A Statement-Level Code Vulnerability Detection for Python | FGCS | 2024 | 🧪 Python语句级漏洞检测 |
| ft10 | Weng, C. et al. — [MATSVD: Boosting Statement-Level Vulnerability Detection via Dependency-Based Attention](https://dl.acm.org/doi/10.1145/3671016.3674807) | Internetware | 2024 | 🧩 依赖关系注意力增强语句级检测 |

### 🧩 LLM + Other DL Modules

LLM与其他深度学习模块融合。

| # | Paper | Venue | Year | 说明 |
|---|-------|-------|------|------|
| ft11 | Ziems, N., Wu, S. — Security Vulnerability Detection Using Deep Learning Natural Language Processing | INFOCOM Workshops | 2021 | 🧪 早期NLP+深度学习漏洞检测工作 |
| ft12 | Tang, W. et al. — CSGVD: A Deep Learning Approach Combining Sequence and Graph Embedding for Source Code Vulnerability Detection | J. Syst. Softw. | 2023 | 🧩 序列+图嵌入融合 |
| ft13 | Jiang, Z. et al. — DFEPT: Data Flow Embedding for Enhancing Pre-Trained Model Based Vulnerability Detection | Internetware | 2024 | ⚙️🔗 数据流嵌入增强预训练模型 |
| ft14 | Yang, A. Z. et al. — [Security Vulnerability Detection with Multitask Self-Instructed Fine-Tuning of Large Language Models](https://arxiv.org/abs/2406.05892) | arXiv | 2024 | 🎯 多任务自指令微调 |

### 🏗️ Domain-Specific Pre-Training

领域专用预训练：面向安全代码的预训练策略。

| # | Paper | Venue | Year | 说明 |
|---|-------|-------|------|------|
| ft15 | Hanif, H., Maffeis, S. — VulBERTa: Simplified Source Code Pre-Training for Vulnerability Detection | IJCNN | 2022 | 🎯 简化代码预训练，专注漏洞检测 |
| ft16 | Ni, C. et al. — Distinguishing Look-Alike Innocent and Vulnerable Code by Subtle Semantic Representation Learning and Explanation | ESEC/FSE | 2023 | 🧩 细粒度语义区分安全/漏洞代码 |
| ft17 | Wang, H. et al. — Combining Structured Static Code Information and Dynamic Symbolic Traces | ICSE | 2024 | ⚠️ 与ft7重复 |
| ft18 | Liu, Z. et al. — Pre-Training by Predicting Program Dependencies | ICSE | 2024 | ⚠️ 与ft8重复 |
| ft19 | Ding, Y. et al. — [Vulnerability Detection with Code Language Models: How Far Are We?](https://arxiv.org/abs/2403.18624) | arXiv | 2024 | ⚠️ 与ft3重复 |
| ft20 | Steenhoek, B. et al. — [Do Language Models Learn Semantics of Code? A Case Study in Vulnerability Detection](https://arxiv.org/abs/2311.04109) | arXiv | 2023 | 🧪 LLM真的学到代码语义了吗？漏洞检测案例研究 |

### 🔗 Causal Learning

因果学习视角的漏洞检测。

| # | Paper | Venue | Year | 说明 |
|---|-------|-------|------|------|
| ft21 | Mahbubur Rahman, M. et al. — Towards Causal Deep Learning for Vulnerability Detection | ICSE | 2024 | 🧠 因果深度学习用于漏洞检测 |

### ⚙️ Default Fine-Tuning

标准微调基线方法。

| # | Paper | Venue | Year | 说明 |
|---|-------|-------|------|------|
| ft22 | Fu, M., Tantithamthavorn, C. — LineVul: A Transformer-Based Line-Level Vulnerability Prediction | MSR | 2022 | 🎯 行级漏洞预测baseline。🔥 基线论文 |
| ft23 | Thapa, C. et al. — Transformer-Based Language Models for Software Vulnerability Detection | ACSAC | 2022 | 🎯 Transformer微调漏洞检测baseline |
| ft24 | Fu, M. et al. — AiBugHunter: A Practical Tool for Predicting, Classifying and Repairing Software Vulnerabilities | EMSE | 2024 | 🛠️ 一体化预测/分类/修复工具 |
| ft25 | Sejfia, A. et al. — Toward Improved Deep Learning-Based Vulnerability Detection | ICSE | 2024 | 🧪 改进深度学习漏洞检测的方法探索 |
| ft26 | Risse, N., Böhme, M. — Uncovering the Limits of Machine Learning for Automatic Vulnerability Detection | USENIX Security | 2024 | 📊 USENIX Security。揭露ML漏洞检测的边界和局限性。🔥 关键论文 |
| ft27 | Steenhoek, B. et al. — An Empirical Study of Deep Learning Models for Vulnerability Detection | ICSE | 2023 | 📊 深度学习漏洞检测大范围实证研究 |
| ft28 | Chen, Y. et al. — DiverseVul: A New Vulnerable Source Code Dataset for Deep Learning Based Vulnerability Detection | RAID | 2023 | 🧩 高质量漏洞数据集DiverseVul |
| ft29 | Li, Z. et al. — On the Effectiveness of Function-Level Vulnerability Detectors for Inter-Procedural Vulnerabilities | ICSE | 2024 | 📊 函数级检测器对过程间漏洞的效果评估 |
| ft30 | Croft, R. et al. — Data Quality for Software Vulnerability Datasets | ICSE | 2023 | 🧩 漏洞数据集数据质量问题 |
| ft31 | Le, T. H. M. et al. — Are Latent Vulnerabilities Hidden Gems for Software Vulnerability Prediction? | MSR | 2024 | 🧩 潜在/隐藏漏洞对预测的影响 |
| ft32 | Zhou, X. et al. — [Comparison of SAST Tools and LLMs for Repo-Level Vulnerability Detection](https://arxiv.org/abs/2407.16235) | arXiv | 2024 | ⚠️ 与pe7重复 |
| ft33 | Shestov, A. et al. — [Fine-Tuning Large Language Models for Vulnerability Detection](https://arxiv.org/abs/2401.17010) | CoRR | 2024 | 🎯 微调LLM做漏洞检测 |

---

## 4. Evaluation & Benchmarks (ev)

评测框架和基准数据集。

| # | Paper | Year | 说明 |
|---|-------|------|------|
| ev1 | [LLM4Vuln: A Unified Evaluation Framework for Decoupling and Enhancing LLMs' Vulnerability Reasoning](https://arxiv.org/pdf/2401.16185) | 2024 | 📊 统一评测框架，解耦和增强LLM漏洞推理能力 |
| ev2 | [LSAST: Enhancing Cybersecurity through LLM-Supported Static Application Security Testing](https://arxiv.org/html/2409.15735v2) | 2024 | ⚙️🔗 LLM增强SAST，混合方法 |
| ev3 | CyberGym et al. — [CyberGym: Evaluating AI Agents' Real-World Cybersecurity Capabilities at Scale](https://arxiv.org/abs/2506.02548) | 2025 | 📊 大规模AI agent网络安全能力评测 |
| ev4 | Zhun Wang et al. — [ExploitGym: Can AI Agents Turn Security Vulnerabilities into Real Attacks?](https://arxiv.org/abs/2605.11086) | 2025 | 📊 评估AI agent能否从漏洞到实战利用 |
| ev5 | Tianneng Shi et al. — [CyberGym-E2E: Scalable Real-World Benchmark for AI Agents' End-to-End Cybersecurity Capabilities](https://arxiv.org/abs/2606.04460) | 2025 | 📊 端到端网络安全能力评测 |
| ev6 | — [CyberChainBench: Can AI Agents Secure Smart Contracts Against Real-World On-Chain Vulnerabilities?](https://arxiv.org/abs/2606.26216) | 2026 | 📊📝 智能合约安全agent评测 |
| ev7 | — [VulnGym: A Real-World, Project-Level Vulnerability Benchmark for White-Box Vulnerability-Hunting Agents](https://github.com/Tencent/VulnGym) | 2026 | 📊 仓库级白盒漏洞挖掘benchmark |
| ev8 | — [SecLens: Benchmarking LLM Vuln Detection Through 5 Stakeholder Lenses on 406 Real-World CVEs](https://arxiv.org/abs/2604.01637) | 2026 | 📊 406个真实CVE，5个利益相关者视角评测 |
| ev9 | — [SV-TrustEval-C: Evaluating Structure and Semantic Reasoning for Source Code Vulnerability Analysis](https://arxiv.org/abs/2505.20630) | IEEE S&P | 2025 | 📊 结构和语义推理能力评估，IEEE S&P顶会 |
| ev10 | — [SecVulEval: Benchmarking LLMs for Real-World C/C++ Vulnerability Detection](https://arxiv.org/abs/2505.19828) | 2025 | 📊 C/C++真实漏洞检测benchmark |

---

## 5. Code Generation (gen)

安全代码生成。

| # | Paper | Year | 说明 |
|---|-------|------|------|
| g1 | [Improving LLM Code Generation with Grammar Augmentation](https://arxiv.org/html/2403.01632v1) | 2024 | 🧩 语法增强提升LLM代码生成质量 |
| g2 | [A Survey on Large Language Models for Code Generation](https://arxiv.org/pdf/2406.00515) | 2024 | 🔄 代码生成LLM综述 |

---

## 6. Code Understanding (understand)

代码理解。

| # | Paper | Year | 说明 |
|---|-------|------|------|
| u1 | [Testing the Effect of Code Documentation on Large Language Model Code Understanding](https://arxiv.org/pdf/2404.03114) | 2024 | 🧪 代码文档对LLM代码理解的影响 |
| u2 | [Using an LLM to Help With Code Understanding](https://arxiv.org/html/2307.08177v3) | 2023 | 🧪 LLM辅助代码理解 |
| u3 | [Automatic Semantic Augmentation of Language Model Prompts (for Code Summarization)](https://arxiv.org/pdf/2304.06815) | 2023 | 💡 自动语义增强prompt用于代码摘要 |

---

## 7. Surveys & Overviews (study)

综述与概览。

| # | Paper | Year | 说明 |
|---|-------|------|------|
| s1 | [Large Language Model for Vulnerability Detection and Repair: Literature Review and the Road Ahead](https://arxiv.org/pdf/2404.02525) | 2024 | 🔄 LLM漏洞检测与修复综述 |
| s2 | [LLMs in Software Security: A Survey of Vulnerability Detection Techniques and Insights](https://arxiv.org/abs/2502.07049) | 2025 | 🔄 LLM在软件安全领域的检测技术综述 |
| s3 | [A Systematic Literature Review on Detecting Software Vulnerabilities with Large Language Models](https://arxiv.org/abs/2507.22659) | 2025 | 🔄 系统性文献综述 |
| s4 | Chen, Y. et al. — [Software Defect Detection Using Large Language Models: A Literature Review](https://link.springer.com/article/10.1007/s11704-025-40672-2) | 2026 | 🔄 软件缺陷检测文献综述 |
| s5 | [When Labels Are Scarce: A Systematic Mapping of Label-Efficient Code Vulnerability Detection](https://arxiv.org/abs/2604.00079) | 2026 | 🔄 标签稀缺场景下的漏洞检测方法综述 |

---

## 8. Others

其他相关论文。

| # | Paper | Year | 说明 |
|---|-------|------|------|
| o1 | [How Well Do Large Language Models Serve as End-to-End Secure Code Producers?](https://arxiv.org/pdf/2408.10495) | 2024 | 🧪 LLM端到端生成安全代码的能力评估 |

---

## 📁 Repository Structure

```
papers/
├── README.md          # This file — full index with hyperlinks
├── .gitignore
├── pe/                # Prompt Engineering papers
├── ft/                # Fine-Tuning papers
├── rag/               # RAG papers (refs from PE section)
├── ev/                # Evaluation papers
├── study/             # Survey / overview
├── gen/               # Code generation
└── understand/        # Code understanding
```

Papers in `pe/`, `ft/`, and `rag/` are stored as either:
- **`.pdf`** — full paper downloaded (for offline access)
- **`.txt`** — link to official publication (DOI or IEEE/ACM)

### 标签说明

| 标签 | 含义 |
|------|------|
| 🔬 Research | 基础研究 |
| 🛠️ Tool/System | 工具/系统 |
| 📊 Benchmark/Evaluation | 评测框架 |
| 🔄 Survey | 综述 |
| 🧪 Experimental | 实验性工作 |
| 🤖 Agent | 智能体系统 |
| 💡 Prompt Engineering | Prompt设计 |
| 🔗 RAG | 检索增强生成 |
| 🎯 Fine-Tuning | 微调方法 |
| ⚙️ SAST+LLM | 静态分析结合LLM |
| 🧩 Data-centric | 数据为中心 |
| 🧠 Reasoning | 推理增强 |
| 📝 Smart Contracts | 智能合约相关 |
| ❌ Not Found | 未找到PDF |
| ⚠️ Duplicate | 与前面重复 |

---

> Maintained by [@llmhacking](https://github.com/llmhacking)
