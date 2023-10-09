# Ask Again, Then Fail: Large Language Models' Vacillations in Judgement

<i>Qiming Xie, Zengzhi Wang, Yi Feng, Rui Xia</i>

<i>Nanjing University of Science and Technology, China</i>


 📄 [[Paper]](https://arxiv.org/abs/2310.02174) &nbsp; 🖥️ [[Homepage on PaperWithCode]](https://paperswithcode.com/paper/ask-again-then-fail-large-language-models)


 ## Quick links

  - [Overview](#overview)
  - [FOLLOW-UP QUESTIONING MECHANISM](#follow-up-questioning-mechanism)
  - [Evaluation](#evaluation)
    - [Experimental Setup](#experimental-setup)
    - [Results Analysis](#results-analysis)
  - [Further Studies](#further-studies)
    - [The Impact of Sampling Temperature](#the-impact-of-sampling-temperature)
    - [The Impact of Different Prompts](#the-impact-of-different-propmts)
    - [Error Analysis](#error-analysis)
    - [Can the Mechanism Correct Models?](can-the-mechanism-correct-models)
  - [Mitigation Method Exploration](mitigation-method-exploration)
  - [Case Study](#case-study)
  - [Any Question?](#any-questions)
  - [Citation](#citation)


## Overview
With the emergence of generative conversational large language models (LLMs) like ChatGPT, serving as virtual assistants in various fields, the stability and reliability of their responses have become crucial. However, during usage, it has been observed that these models tend to waver in their judgements when confronted with follow-up questions from users expressing skepticism or disagreement. 
In this work, we draw inspiration from questioning strategies in education and propose a **FOLLOW-UP QUESTIONING MECHANISM** along with two evaluation metrics to assess the judgement consistency of LLMs before and after exposure to disturbances. (We define judgement consistency as the consistency of the model’s final answers when handling objective questions with definitive answers.) We evaluate the judgement consistency of ChatGPT, PaLM2-Bison, and Vicuna-13B under this mechanism across eight reasoning benchmarks. Empirical results show that even when the initial answers are correct, judgement consistency sharply decreases when LLMs face disturbances such as questioning, negation, or misleading. 
Additionally, we study these models’ judgement consistency under various settings (sampling temperature and prompts) to validate this issue further, observing the impact of prompt tone and conducting an in-depth error analysis for deeper behavioral insights. Furthermore, we also explore several prompting methods to mitigate this issue and demonstrate their effectiveness.


## FOLLOW-UP QUESTIONING MECHANISM
<div align=center> <img alt="method" src="https://github.com/NUSTM/LLMs-Waver-In-Judgements/assets/84706021/88aee09f-b552-40b2-89f4-759ece0dfb28" width="60%" height="30%"></div>

To evaluate this consistency of large language models, we design a **FOLLOW-UP QUESTIONING MECHANISM**. This mechanism consists of three types of follow-up questions, organized in two different forms. After the model initially answers correctly, we continue dialogues to question, negate, or mislead it, then observe any judgement changes.

We employ two metrics to assess the judgement consistency of LLMs after the execution of the **FOLLOW-UP QUESTIONING MECHANISM**.
- **Modification (M.)** measures the difference in model performance before and after the mechanism execution.
- **Modification Rate (M. Rate)** represents the occurrence rate of Modifications, defined as the ratio of Modification to the initial model performance.


## Evaluation


### Experimental Setup


### Results Analysis


## Further Studies


### The Impact of Sampling Temperature 🌡️


### The Impact of Different Prompts 🎨


### Error Analysis 🔍


### Can the Mechanism Correct Models❓


## Mitigation Method Exploration


## Case Study


## Citation

If you find this work helpful, please cite our paper as follows:

```
xxx
```


## Any Questions?

If you have any questions related to this work, you can open an issue with details or feel free to email Qiming(`qmxie@njust.edu.cn`), Zengzhi(`zzwang@njust.edu.cn`).
