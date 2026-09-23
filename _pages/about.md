---

permalink: /
title: "Brief Introduction"
author_profile: true
redirect_from: 
/about 
/about.html


---

I am currently a Master's student in **Computer Technology at Tsinghua University**, with research interests in **Multimodal Large Language Models (MLLMs)** and **LLM Agents**. Before joining Tsinghua, I received my B.Eng. degree in **Software Engineering from Harbin Institute of Technology (HIT)**, where I ranked **1st in my major** and was recommended for graduate study at Tsinghua University.

My current research focuses on improving the **reliability, safety, and post-training of large language and multimodal models**, particularly in **hallucination mitigation, agentic tool use, preference learning, and reinforcement learning**. I am also interested in building trustworthy models that can reliably perceive multimodal information, reason over complex contexts, and interact with external tools.

I have published research at **ECCV, ICLR, and EMNLP**, covering multimodal hallucination mitigation, vision-language continual learning, LLM safety, and backdoor attacks. My recent work further explores **reinforcement learning for reliable agentic tool use**.

## 🔥 News

* **Sep. 2026** — Our work **ToolHallu**, which studies fine-grained hallucination mitigation for agentic tool calls through reinforcement learning, is under review at **ICLR 2027**.
* **2026** — Our paper on **multi-image hallucination mitigation** was accepted by **ECCV 2026**.
* **2026** — Our work **Revisiting LLM Backdoor Attacks: A Stealthy Poisoning Framework via Harmless Inputs** was accepted by **EMNLP 2026 Main Conference**.
* **2026** — Our work **CHILLGuard: Chinese LLM Guardrail with Data-Model-aware Preference Alignment** was accepted by **EMNLP 2026 Findings**.
* **2026** — Our work **Naming to Learn: Class Incremental Learning for Vision-Language Model with Unlabeled Data** was accepted by **ICLR 2026**.
* **Sep. 2026** — I started my Master's study at **Tsinghua University**.

## 🔬 Research Interests

My research interests broadly lie in **Trustworthy Multimodal Intelligence and LLM Agents**, with a particular focus on:

* **Multimodal Large Language Models:** multimodal reasoning, multi-image understanding, and visual hallucination mitigation.
* **LLM Agents:** reliable tool use, tool-call hallucination, and agentic reasoning.
* **LLM Post-training:** reinforcement learning, preference optimization, and model alignment.
* **AI Safety:** LLM guardrails, jailbreaks, backdoor attacks, and trustworthy model behavior.

## 📝 Publications

### Looking Back and Forth: Cross-Image Attention Preference Learning for Multi-Image Hallucination

**Xiaochen Yang**, et al.
**ECCV 2026**

We study hallucination in multi-image vision-language models from the perspectives of **cross-image information interaction** and **visual evidence preference**. We propose a framework combining **selective cross-image attention calibration** with **preference learning** to improve cross-image entity association and visual evidence utilization.

[Code](https://github.com/yyyxcleo/CAPL)

---

### Revisiting LLM Backdoor Attacks: A Stealthy Poisoning Framework via Harmless Inputs

**EMNLP 2026 Main Conference**

We investigate stealthy LLM backdoor attacks that rely only on **harmless training samples**, avoiding conventional poisoned examples that can be detected during data filtering. The framework combines clean-data backdoor construction with **gradient-guided universal trigger optimization** to achieve robust and transferable backdoor activation.

---

### CHILLGuard: Chinese LLM Guardrail with Data-Model-aware Preference Alignment

**EMNLP 2026 Findings**

We develop a fine-grained **Chinese LLM safety guardrail** covering **5 high-level and 31 fine-grained risk categories**. CHILLGuard combines a large-scale safety dataset with **model-aware preference alignment** to improve recognition of implicit, adversarial, and boundary safety risks.

---

### Naming to Learn: Class Incremental Learning for Vision-Language Model with Unlabeled Data

**ICLR 2026**

We study **class-incremental learning for vision-language models under unlabeled data**, exploring how semantic knowledge from vision-language models can facilitate continual adaptation without explicit class annotations.

---

### ToolHallu: Mitigating Hallucination in Agentic Tool Calls via Reinforcement Learning

**Xiaochen Yang**, et al.
**ICLR 2027, Under Review**

We study hallucinations in LLM agent tool use, including **tool selection errors, parameter hallucinations, and repeated tool calls**. We propose a fine-grained reinforcement learning framework with **structured hallucination rewards** and **curriculum-based reward scheduling** to progressively optimize tool selection and parameter generation.

## 🚀 Selected Research Projects

### Multi-Image Hallucination Mitigation via Cross-Image Attention and Preference Learning

**ECCV 2026 · First Author**
*Oct. 2025 – Mar. 2026*

Multi-image MLLMs often suffer from hallucinations because of insufficient information interaction across images and inadequate preference for cross-image visual evidence. We address these issues from both the **model architecture** and **post-training** perspectives.

* **Cross-Image Attention Calibration.** We design a selective cross-image attention mechanism that identifies informative visual tokens according to **embedding energy**, relaxes causal attention constraints across different images, and employs an **alternating attention mask** to improve cross-image interaction and entity alignment.
* **Cross-Image Preference Learning.** We construct preference pairs according to the degree of cross-image interaction and employ **DPO** to encourage stronger reliance on cross-image visual evidence, together with an **NLL objective** for stable generation.
* **Results.** Experiments on **Qwen2.5-VL, InternVL2.5, and GLM4.1VBase** demonstrate improvements of up to **4.49, 3.58, and 2.73 percentage points**, respectively, while largely preserving single-image and general multimodal capabilities.

### ToolHallu: Mitigating Hallucination in Agentic Tool Calls via Reinforcement Learning

**ICLR 2027 Under Review · First Co-author**
*Apr. 2026 – Sep. 2026*

LLM agents can hallucinate throughout the tool-use process, ranging from selecting nonexistent or incorrect tools to generating invalid parameters and repeatedly invoking tools. We develop **ToolHallu**, a reinforcement learning framework that explicitly models these fine-grained failure modes.

* **Fine-grained Hallucination Rewards.** We decompose tool-use hallucinations into **tool-name, parameter, and repeated-call errors**, with parameter errors further categorized into missing/redundant parameters, type errors, and value errors. Structured rule-based rewards provide interpretable supervision for each failure mode.
* **Curriculum Reward Scheduling.** We introduce a **cosine-based reward scheduling strategy** that first emphasizes tool selection and progressively increases parameter-level supervision, enabling optimization from coarse-grained tool selection to fine-grained argument generation.
* **Results.** Across multiple models and tool-use benchmarks, ToolHallu consistently reduces hallucinations. On **API-Bank** and **StableToolBench**, hallucination metrics decrease by an average relative **8.00% and 20.25%**, respectively, while task success rates continue to improve.

### Stealthy LLM Backdoor Attacks via Harmless Inputs

**EMNLP 2026 Main · First Co-author**
*May 2025 – Sep. 2025*

Conventional LLM backdoor attacks typically rely on poisoned or anomalous training samples, making them vulnerable to safety filtering before fine-tuning. We investigate whether a backdoor can instead be established using only apparently **harmless training data**.

* We construct implicit associations between trigger conditions and target behaviors through **affirmative prefixes and structured content**, without introducing explicitly malicious training samples.
* We further develop a **gradient-guided universal trigger optimization** strategy to improve trigger robustness and generalization across different inputs.
* After safety filtering, the method achieves an average **98.13% attack success rate (ASR)** under a rule-based judge, with several evaluated models reaching **100% ASR**.

### CHILLGuard: Fine-Grained Safety Guardrails for Chinese LLMs

**EMNLP 2026 Findings · Co-author**
*Nov. 2025 – Mar. 2026*

Existing LLM guardrails often provide insufficient fine-grained coverage for Chinese safety risks, especially implicit, transformed, and boundary cases. CHILLGuard develops a comprehensive safety data and alignment framework specifically for Chinese LLMs.

* We construct a multi-stage safety data pipeline using **RAG, prompt engineering, and multi-model voting**, covering **5 high-level and 31 fine-grained risk categories**, with **405K training samples and 52K test samples**.
* We introduce a **generator-classifier collaborative training framework** with **model-aware DPO (MDPO)** to dynamically adjust KL regularization and improve alignment on difficult safety cases.
* The 8B model achieves an **F1 score of 89.77** on CHILLGuardTest, representing a **15.92% improvement** over Qwen3Guard-8B-Strict.

## 🎓 Education

### Tsinghua University

**M.Eng. in Computer Technology**
*Sep. 2026 – Present*

Research focus: **Multimodal Large Language Models and LLM Agents**

### Harbin Institute of Technology

**B.Eng. in Software Engineering**
*Sep. 2022 – Jun. 2026*

* Ranked **1st** in the major.
* Recommended for graduate study at **Tsinghua University**.
* Recipient of the **National Scholarship** in 2023 and 2025.
* Recipient of the **HIT First-Class Scholarship** in 2023 and 2024.
* Provincial First Prize in the **Lanqiao Cup Algorithm Competition**.

## 🏆 Honors & Awards

* **National Scholarship**, 2023 & 2025
* **HIT First-Class Scholarship**, 2023 & 2024
* **Provincial First Prize**, Lanqiao Cup Algorithm Competition
* **CET-6:** 590
