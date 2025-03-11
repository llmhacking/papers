# LLM for Vulnerability Detection Releated Papers
## 0. study
- 1. https://arxiv.org/pdf/2404.02525
## 1. prompt engineering(pe)
- pe1. Fu, M., Tantithamthavorn, C., Nguyen, V., and Le, T. Chatgpt for vulnerability detection, classification, and repair: How far are we? APSEC (2023)
- pe2. Khare, A., Dutta, S., Li, Z., Solko-Breslin, A., Alur, R., and Naik, M. Understanding the effectiveness of large language models in detecting security vulnerabilities. arXiv preprint arXiv: 2311.16169 (2023).
- pe3. Ni, C., Shen, L., Xu, X., Yin, X., and Wang, S. Learning-based models for vulnerability detection: An extensive study. arXiv preprint arXiv:2408.07526 (2024).
- pe4. Purba, M. D., Ghosh, A., Radford, B. J., and Chu, B. Software vulnerability detection using large language models.
In 34th IEEE International Symposium on Software Reliability Engineering, ISSRE 2023 - Workshops, Florence, Italy, October 9-12, 2023 (2023), IEEE, pp. 112–119.
- pe5. Yin, X. Pros and cons! evaluating chatgpt on software vulnerability. CoRR abs/2404.03994 (2024).
- pe6. Zhang, C., Liu, H., Zeng, J., Yang, K., Li, Y., and Li, H. Prompt-enhanced software vulnerability detection using chatgpt. arXiv preprint arXiv: 2308.12697 (2023)
- pe7. Zhou, X., Tran, D.-M., Le-Cong, T., Zhang, T., Irsan, I. C., Sumarlin, J., Le, B., and Lo, D. Comparison of static application security testing tools and large language models for repo-level vulnerability detection. arXiv preprint arXiv:2407.16235 (2024).
- pe8. Zhou, X., Zhang, T., and Lo, D. Large language model for vulnerability detection: Emerging results and future directions. ICSE NIER track (2024).

## 2. fine-tuning(ft)
### Data-centric Innovations
- ft1. Wen, X., Wang, X., Gao, C., Wang, S., Liu, Y., and Gu, Z. When less is enough: Positive and unlabeled learning model for vulnerability detection. In 38th IEEE/ACM International Conference on Automated Software Engineering,
ASE 2023, Luxembourg, September 11-15, 2023 (2023), IEEE, pp. 345–357
- ft2. Kuang, H., Yang, F., Zhang, L., Tang, G., and Yang, L. Leveraging user-defined identifiers for counterfactual data generation in source code vulnerability detection. In 23rd IEEE International Working Conference on Source Code Analysis and Manipulation, SCAM 2023, Bogotá, Colombia, October 2-3, 2023 (2023), L. Moonen, C. D. Newman, and A. Gorla, Eds., IEEE, pp. 143–150.
- ft3.  Ding, Y., Fu, Y., Ibrahim, O., Sitawarin, C., Chen, X., Alomair, B., Wagner, D. A., Ray, B., and Chen, Y. Vulnerability detection with code language models: How far are we? arXiv preprint arXiv: 2403.18624 (2024).
- ft4. Yang, X., Wang, S., Li, Y., and Wang, S. Does data sampling improve deep learning-based vulnerability detection? yeas! and nays! In 45th IEEE/ACM International Conference on Software Engineering, ICSE 2023, Melbourne, Australia, May 14-20, 2023 (2023), IEEE, pp. 2287–2298.

### Combining with Program Analysis
- ft5. Peng, T., Chen, S., Zhu, F., Tang, J., Liu, J., and Hu, X. Ptlvd:program slicing and transformer-based line-level vulnerability detection system. In 23rd IEEE International Working Conference on Source Code Analysis and Manipulation, SCAM 2023, Bogotá, Colombia, October 2-3, 2023 (2023), L. Moonen, C. D. Newman, and A. Gorla, Eds., IEEE, pp. 162–173.
- ft6. Zhang, J., Liu, Z., Hu, X., Xia, X., and Li, S. Vulnerability detection by learning from syntax-based execution paths of code. IEEE Trans. Software Eng. 49, 8 (2023), 4196–4212.
- ft7. Wang, H., Tang, Z., Tan, S. H., Wang, J., Liu, Y., Fang, H., Xia, C., and Wang, Z. Combining structured static code information and dynamic symbolic traces for software vulnerability prediction. In Proceedings of the 46th International Conference on Software Engineering (2024), ACM.
- ft8. Liu, Z., Tang, Z., Zhang, J., Xia, X., and Yang, X. Pre-training by predicting program dependencies for vulnerability analysis tasks. ICSE (2024).
- ft9. Tran, H.-C., Tran, A.-D., and Le, K.-H. Detectvul: A statement-level code vulnerability detection for python. Future Generation Computer Systems (2024), 107504.
- ft10. Weng, C., Qin, Y., Lin, B., Liu, P., and Chen, L. Matsvd: Boosting statement-level vulnerability detection via
dependency-based attention. In Proceedings of the 15th Asia-Pacific Symposium on Internetware, Internetware 2024,Macau, SAR, China, July 24-26, 2024 (2024), H. Mei, J. Lv, A. Helal, X. Ma, S. Cheung, J. Zhang, and T. Zhang, Eds., ACM.

### LLM+Other DL Modules 
- ft11. Ziems, N., and Wu, S. Security vulnerability detection using deep learning natural language processing. In 2021 IEEE Conference on Computer Communications Workshops, INFOCOM Workshops 2021, Vancouver, BC, Canada, May 10-13, 2021 (2021), IEEE, pp. 1–6.
- ft12.  Tang, W., Tang, M., Ban, M., Zhao, Z., and Feng, M. CSGVD: A deep learning approach combining sequence and graph embedding for source code vulnerability detection. J. Syst. Softw. 199 (2023), 111623.
- ft13. Jiang, Z., Sun, W., Gu, X., Wu, J., Wen, T., Hu, H., and Yan, M. DFEPT: data flow embedding for enhancing pre-trained model based vulnerability detection. In Proceedings of the 15th Asia-Pacific Symposium on Internetware, Internetware 2024, Macau, SAR, China, July 24-26, 2024 (2024), H. Mei, J. Lv, A. Helal, X. Ma, S. Cheung, J. Zhang, and T. Zhang, Eds., ACM.
- ft14. Yang, A. Z., Tian, H., Ye, H., Martins, R., and Goues, C. L. Security vulnerability detection with multitask self-instructed fine-tuning of large language models. arXiv preprint arXiv:2406.05892 (2024).

### Domain-specific Pre-training
- ft15. Hanif, H., and Maffeis, S. Vulberta: Simplified source code pre-training for vulnerability detection. In International Joint Conference on Neural Networks, IJCNN 2022, Padua, Italy, July 18-23, 2022 (2022), IEEE, pp. 1–8.
- ft16. Ni, C., Yin, X., Yang, K., Zhao, D., Xing, Z., and Xia, X. Distinguishing look-alike innocent and vulnerable code by
subtle semantic representation learning and explanation. In Proceedings of the 31st ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering (2023), pp. 1611–1622.
- ft17. Wang, H., Tang, Z., Tan, S. H., Wang, J., Liu, Y., Fang, H., Xia, C., and Wang, Z. Combining structured static code information and dynamic symbolic traces for software vulnerability prediction. In Proceedings of the 46th International Conference on Software Engineering (2024), ACM.
- ft18. Liu, Z., Tang, Z., Zhang, J., Xia, X., and Yang, X. Pre-training by predicting program dependencies for vulnerability analysis tasks. ICSE (2024).
- ft19. Ding, Y., Fu, Y., Ibrahim, O., Sitawarin, C., Chen, X., Alomair, B., Wagner, D. A., Ray, B., and Chen, Y. Vulnerability detection with code language models: How far are we? arXiv preprint arXiv: 2403.18624 (2024).
- ft20. Steenhoek, B., Rahman, M. M., Sharmin, S., and Le, W. Do language models learn semantics of code? A case study in vulnerability detection. arXiv preprint arXiv: 2311.04109 (2023).

### Causal Learning
- ft21. Mahbubur Rahman, M., Ceka, I., Mao, C., Chakraborty, S., Ray, B., and Le, W. Towards causal deep learning for vulnerability detection. ICSE (2024).
### Default Fine-tunning
- ft22. Fu, M., and Tantithamthavorn, C. Linevul: A transformer-based line-level vulnerability prediction. In 19th IEEE/ACM International Conference on Mining Software Repositories, MSR 2022, Pittsburgh, PA, USA, May 23-24, 2022 (2022), ACM, pp. 608–620.
- ft23. Thapa, C., Jang, S. I., Ahmed, M. E., Camtepe, S., Pieprzyk, J., and Nepal, S. Transformer-based language models for software vulnerability detection. In Annual Computer Security Applications Conference, ACSAC 2022, Austin, TX, USA, December 5-9, 2022 (2022), ACM, pp. 481–496.
- ft24. Fu, M., Tantithamthavorn, C., Le, T., Kume, Y., Nguyen, V., Phung, D. Q., and Grundy, J. C. Aibughunter: A practical tool for predicting, classifying and repairing software vulnerabilities. Empir. Softw. Eng. 29, 1 (2024), 4.
- ft25. Sejfia, A., Das, S., Shafiq, S., and Medvidovic, N. Toward improved deep learning-based vulnerability detection. In Proceedings of the 46th IEEE/ACM International Conference on Software Engineering, ICSE 2024, Lisbon, Portugal, April 14-20, 2024 (2024), ACM, pp. 62:1–62:12.
- ft26. Risse, N., and Böhme, M. Uncovering the limits of machine learning for automatic vulnerability detection. In 33rd USENIX Security Symposium, USENIX Security 2024, Philadelphia, PA, USA, August 14-16, 2024 (2024), D. Balzarotti and W. Xu, Eds., USENIX Association.
- ft27. Steenhoek, B., Rahman, M. M., Jiles, R., and Le, W. An empirical study of deep learning models for vulnerability detection. In 45th IEEE/ACM International Conference on Software Engineering, ICSE 2023, Melbourne, Australia, May 14-20, 2023 (2023), IEEE, pp. 2237–2248.
- ft28. Chen, Y., Ding, Z., Alowain, L., Chen, X., and Wagner, D. A. Diversevul: A new vulnerable source code dataset for deep learning based vulnerability detection. In Proceedings of the 26th International Symposium on Research in Attacks, Intrusions and Defenses, RAID 2023, Hong Kong, China, October 16-18, 2023 (2023), ACM, pp. 654–668.
- ft29. Li, Z., Wang, N., Zou, D., Li, Y., Zhang, R., Xu, S., Zhang, C., and Jin, H. On the effectiveness of functionlevel vulnerability detectors for inter-procedural vulnerabilities. In Proceedings of the 46th IEEE/ACM International Conference on Software Engineering, ICSE 2024, Lisbon, Portugal, April 14-20, 2024 (2024), ACM, pp. 157:1–157:12.
- ft30. Croft, R., Babar, M. A., and Kholoosi, M. M. Data quality for software vulnerability datasets. In 45th IEEE/ACM International Conference on Software Engineering, ICSE 2023, Melbourne, Australia, May 14-20, 2023 (2023), IEEE, pp. 121–133.
- ft31. Le, T. H. M., Du, X., and Babar, M. A. Are latent vulnerabilities hidden gems for software vulnerability prediction? an empirical study. In 21st IEEE/ACM International Conference on Mining Software Repositories, MSR 2024, Lisbon, Portugal, April 15-16, 2024 (2024), D. Spinellis, A. Bacchelli, and E. Constantinou, Eds., ACM, pp. 716–727.
- ft32. Zhou, X., Tran, D.-M., Le-Cong, T., Zhang, T., Irsan, I. C., Sumarlin, J., Le, B., and Lo, D. Comparison of static application security testing tools and large language models for repo-level vulnerability detection. arXiv preprint arXiv:2407.16235 (2024).
- ft33. Shestov, A., Cheshkov, A., Levichev, R., Mussabayev, R., Zadorozhny, P., Maslov, E., Vadim, C., and Bulychev, E. Finetuning large language models for vulnerability detection. CoRR abs/2401.17010 (2024).

## 3. retrieval-augmented generation(rag)
- rag1. Liu, Z., Liao, Q., Gu, W., and Gao, C. Software vulnerability detection with GPT and in-context learning. In 8th International Conference on Data Science in Cyberspace, DSC 2023, Hefei, China, August 18-20, 2023 (2023), IEEE, pp. 229–236.
- rag2. Zhou, X., Zhang, T., and Lo, D. Large language model for vulnerability detection: Emerging results and future directions. ICSE NIER track (2024).
- rag3. Du, X., Zheng, G., Wang, K., Feng, J., Deng, W., Liu, M., Chen, B., Peng, X., Ma, T., and Lou, Y. Vul-rag: Enhancing llm-based vulnerability detection via knowledge-level RAG. CoRR abs/2406.11147 (2024).
- rag4. Wen, X., Wang, X., Chen, Y., Hu, R., Lo, D., and Gao, C. Vuleval: Towards repository-level evaluation of software vulnerability detection. CoRR abs/2404.15596 (2024).

## 4. Evaluation
- ev1. [LLM4Vuln: A Unified Evaluation Framework for Decoupling and
Enhancing LLMs’ Vulnerability Reasoning](https://arxiv.org/pdf/2401.16185)
- ev2. [LSAST: Enhancing Cybersecurity through LLM-supported Static Application Security Testing
](https://arxiv.org/html/2409.15735v2)

## 5. others
- o1. LLM-Assisted Static Analysis for Detecting Security Vulnerabilities
- o2. [How Well Do Large Language Models Serve as End-to-End Secure
Code Producers?](https://arxiv.org/pdf/2408.10495) 