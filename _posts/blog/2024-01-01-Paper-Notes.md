---
layout: post
title: Research Notes
categories: blog
description: Hey, welcome to my research notes.
keywords: AI Papers, Publications
---
Welcome! This blog contains my notes on reading papers related to LMs-agents and emotional dialog.

---

# Research Note

> Welcome! This blog is a collection of my notes on papers related to language model agents and the realm of emotional dialogues.

## Markdown Template

> Markdown Note Template
> 这是模板
> [Vscode snippets prefix : "paper_note_template"]

```markdown
### Title

* **Keywords**:
#### Intensive Reading 

##### Link

* **Github\ArXiv**: 

* **Demo**:  

##### Evaluate

* **Usefulness(1~5)**: 
* **Timing**: 

##### Abstract
```

## Methodology

* [How to Search and Read a Paper](https://github.com/qiyuangong/How_to_Search_and_Read_a_Paper)
* 

## LLM / LLM-Agent Related Papers

### Title: WEBARENA: A REALISTIC WEB ENVIRONMENT FOR BUILDING AUTONOMOUS AGENTS

Keyword: Web-agent，
Link：

* Github\Arixiv: <https://arxiv.org/pdf/2307.13854.pdf>
* Open-source: yes
* **Demo**:  <https://webarena.dev/>
Evaluate:
* **Usefulness(1~5)**: 3
* **Timing**: 2023.10
* **Intensive Reading**: No
* Abstract:

A useful LLM-base agent that can manipulate Web UI. The demo is interesting. The interaction between LLM and Webs is valuable.

### Title: Hierarchical Prompting Assists Large Language Model on Web Navigation

* Keyword: Web Agent, Hierarchical Prompting, EMNLP fINDINGS
Link

* **Github**: <https://github.com/robert1003/ash-prompting>
* **Demo**:  No

* Evaluate

* **Usefulness(1~5)**: 4.5
* **Timing**: Oct 25th, 2023
* **Intensive Reading**: TODO
* Abstract:

He looks like he wrote a framework/system into two articles. This method is similar to the ReAct.

<p align="center">
<img src="https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image.png" alt="image" style="zoom:80%;" />
</p>

### Title: FIREACT: Toward LANGUAGE AGENT FINE-TUNING

Keywords: ReACT+ Finetune, Ablation Experiment, LM fine-tuning，
Link

* Github:

* **Demo**: 
  Evaluate

* **Usefulness(1~5)**: 5

* **Timing**: Oct 9,2023

* **Intensive Reading**: yes
  Abstract:

* The article's structure is logical, coherent and complete, making it easy to follow.

* The related work part of the article is detailed, in-depth and informative, providing valuable conclusions.

* This paper compares the many methods, including fine-tune & prompt & TOOL, reAct & Reflexion & CoT.

![image-20231217110322487](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217110322487.png)

Useful Conclusion:

* Finetuning GPT-3.5 only cost 10 dollars.
* LLama-7B models could be fine-tuned to catch up with GPT-3.5 performances.
* Dr. Yao has in-depth and extensive investigations of LMagent-related works.

![image-20231217112034478](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217112034478.png)

### Title: SWE-BENCH: CAN LANGUAGE MODELS RESOLVE REAL-WORLD GITHUB ISSUES?

Keywords: LLM-assist Code-generation, Github issues
Link

* **Github**:  <https://www.swebench.com>.
* **Demo**: 
Evaluate
* **Usefulness(1~5)**: 2
* **Timing**: Oct 10, 2023
* **Intensive Reading**:
Abstract:


### Title: Embers of Autoregression: Understanding Large Language Models Through the Problem Trained to Solve

Keywords: Summarize, interesting figures, comprehensive, wonderful explanation of next-word prediction, Frequency determines quality (main idea).
Link

* **Github**: <https://github.com/tommccoy1/embers-of-autoregression> (mission impossible of LLMs)
* **Demo**:  
Evaluate
* **Usefulness(1~5)**: 
* **Timing**: 
* **Intensive Reading**: 
Abstract: 

* This figure can be improved. (What are the capacities of Human & LLM?)
![Alt text](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-1.png)
* This paper exhibits what might seem like surprising failures of LLMs on tasks that are straightforward for humans to perform.

![image-20231217150042407](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217150042407.png)

* Supplement

|           | Unique Human Capacities               | Shared | LLM Capacities |
| --------- | ---------------------------------------- | ------ | ---------------- |
| Math      | Counting、Ciphers、Linear Functions      |        | COT?             |
| Language  | Word/letter reverse、Acronyms、Pig latin |        | World knowledge  |
| Physical  | LeCun's world models                     |        |                  |
| Training  | Efficiency                               |        |                  |
| Frequency |                                          |        |                  |
|(failures of planning in arithmetic and text generation)||||

Effects on the performance of large language models that are attributable to the fact that they are statistical next-word prediction systems.

![image-20231217153534032](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217153534032.png)

### Title: Cognitive Architectures for Language Agents

Keywords: New agents' framework, Control flow, Symbolic AGI
Link

* **Github**:  <https://github.com/ysymyth/awesome-language-agents>
* <img src="https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217165037780.png" alt="image-20231217165037780" style="zoom:25%;" />
* **Demo**: 
Evaluate
* **Usefulness(1~5)**: 4.9
* **Timing**: Sep 25, 2023
* **Intensive Reading**: True
  Abstract: Proposed a complex agent frameworks

![image-20231217164349549](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164349549.png)

![image-20231217164558289](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164558289.png)

![image-20231217164657449](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164657449.png)

![image-20231217164848939](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164848939.png)

### Title: Agents: An Open-source Framework for Autonomous Language Agents 【Multi-Agents】

Keyword： multi-Agents, Autonomous Agents
Link

* **Github**: <https://github.com/aiwaves-cn/agents>

* **Demo**: 

   ![image-20231228131805241](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231228131805241.png)
  Evaluate：

  ![image-20231228131902233](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231228131902233.png)

* **Usefulness(1~5)**: 5

* **Timing**: 

* **Intensive Reading**: 
Abstract: 

> TO-DO 12-29
> Read <https://arxiv.org/pdf/2311.16832.pdf>
> Reproduce Code
> Try Character.ai
> Finish Dynamic Memory Component

### Title: AgentVerse 【Multi-Agent】

* **Keywords**: Multiple LLM-based agents for task-solving and simulation,
  Link
* **Github**: <https://github.com/OpenBMB/AgentVerse>
* **Demo**:  <https://github.com/OpenBMB/AgentVerse>
* **OpenReview[review+rebuttal]** <https://openreview.net/forum?id=EHg5GDnyq1> highlight&highquality
* **Usefulness(1~5)**: 5
* **Timing**: Aug,2023
* **Intensive Reading**: Todo Openreview & code 

#### Intensive Reading: yes

#####　Abstract

* AGENTVERSE which can effectively orchestrate a collaborative group of expert agents
  as a **greater-than-the-sum-of-its-parts system.** 

* **AgentVerse** is designed to facilitate the deployment of multiple LLM-based agents in various applications. AgentVerse primarily provides two frameworks: **task-solving** and **simulation**.

  * Task-solving: This framework assembles multiple agents as an automatic multi-agent system ([AgentVerse-Tasksolving](https://arxiv.org/pdf/2308.10848.pdf), [Multi-agent as system](https://arxiv.org/abs/2309.02427)) to collaboratively accomplish the corresponding tasks. Applications: software development system, consulting system, etc.

  [![Screen Shot 2023-09-01 at 12 08 57 PM](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/264917097-6db1c907-b7fc-42f9-946c-89853a28f386.png)](https://private-user-images.githubusercontent.com/11704492/264917097-6db1c907-b7fc-42f9-946c-89853a28f386.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDM5Mzc5MDgsIm5iZiI6MTcwMzkzNzYwOCwicGF0aCI6Ii8xMTcwNDQ5Mi8yNjQ5MTcwOTctNmRiMWM5MDctYjdmYy00MmY5LTk0NmMtODk4NTNhMjhmMzg2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyMzEyMzAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjMxMjMwVDEyMDAwOFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTkwNDk5Mjk1ZGM5MTBjODE5NzA0ZTFhYTVhNTlkMDViNWYwYjVkOTYyMDdmMmVmNGU0ZGNkZTI3OGVmNmI1NjkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.LcJ8qjM00WMDeCV6cjraehSUPn8XpQfA2Y43OGCk6Eg)

* AgentVerse split the problem-solving process into four pivotal Stages as shown in Figure 2

  * **Expert Recruitment** (还需要招募专家？): 

  * <img src="https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240102164930868.png" alt="image-20240102164930868" style="zoom:25%;" />

  * **Collaborative Decision Making**

    <img src="https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240102164948596.png" alt="image-20240102164948596" style="zoom:25%;" />

  * **Action Execution**

  * Simulation: This framework allows users to set up custom environments to observe behaviors among, or interact with, multiple agents. ⚠️⚠️⚠️ We're refactoring the code. If you require a stable version that exclusively supports the simulation framework, you can use [`release-0.1`](https://github.com/OpenBMB/AgentVerse/tree/release-0.1) branch. Applications: game, social behavior research of LLM-based agents, etc.

  [![Screen Shot 2023-10-16 at 10 53 49 PM](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/275622325-4102d1e2-3fe7-4656-aa2c-a218ce1f2c95.png)](https://private-user-images.githubusercontent.com/11704492/275622325-4102d1e2-3fe7-4656-aa2c-a218ce1f2c95.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDM5Mzc5MDgsIm5iZiI6MTcwMzkzNzYwOCwicGF0aCI6Ii8xMTcwNDQ5Mi8yNzU2MjIzMjUtNDEwMmQxZTItM2ZlNy00NjU2LWFhMmMtYTIxOGNlMWYyYzk1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyMzEyMzAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjMxMjMwVDEyMDAwOFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWE0NTgyMzdiMjI4NDg3MzRkZTFmMzVmYTlmNjMzMTgwNTNkODQyZTY4NmU3MzAzOWVmODBjYzkwZmQ1MjU0YTkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.AeHkR0ZdsWHoJaduvXBB89ZKRWbkYvTljeRn5CMWho0)

### Title：CharacterChat 【Role-Play Agents】

* Keyword： Personalized Social Support = Emotional Support + Multi-Agents, MBTI Persona Scale+ wonderful dataset

* Link (<https://arxiv.org/abs/2308.10278>)

* **Github**: <https://github.com/morecry/CharacterChat>

* **Demo**:  
  Evaluate

* **Usefulness(1~5)**: 5【TODO: reproduce】

* **Timing**:  Aug 2023

* **Intensive Reading**:

* **TODO**: 20min code reading

* **Proper noun learning:** ESC, social support

#### Intensive Reading: yes

##### Abstract

* Traditional methods such as **Emotional Support Conversations (ESC)** face challenges in effectively addressing a diverse range of individual personalities. In response, we introduce the **Social Support Conversation (S2Conv)** framework. It comprises a series of support **agents** and the **interpersonal** **matching** mechanism, linking individuals with persona-compatible virtual supporters【Same as I thought in August】. Utilizing persona decomposition based on the MBTI (Myers Briggs Type Indicator)【a scale】, we have created the MBTI-1024 Bank, a group of virtual characters with distinct profiles. Through improved role-playing prompts with behavior preset and dynamic memory, we facilitate the development of the MBTI-S2Conv dataset, which contains conversations between the characters in the MBTI-1024 Bank. Building upon these foundations, we present CharacterChat, a comprehensive S2Conv system, which includes a conversational model driven by personas and memories, along with an **interpersonal matching plugin model** 【Calculate Attention between personality 】 that dispatches the optimal supporters from t**he MBTI-1024 Bank** for individuals with specific personas. Empirical results indicate the remarkable efficacy of CharacterChat in providing personalized social support and highlight the substantial advantages derived from interpersonal matching. The source code is available at https://github.com/morecry/CharacterChat.

##### Methodology

Within the S2Conv framework

* Characters profiles include the **persona（Name, Gender, Tone, Personality） and dynamic memory**
* Memory:
  * Housing multifaceted factual knowledge by social with a character-> as a contextual reference
  * triggers for a Seeker's mental health Problem
  * 就是使用memory作为事实验证
  * **Supporters Sharing similar backgrounds with seekers** [interesting]

###### Difference between Information Support and Emotional Support

  ![image-20240102152650148](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240102152650148.png)

##### Data

* Create characters with chat GPT

  ![image-20240104104102283](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240104104102283.png)
  
  ![image-20240102152405520](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240102152405520.png)

###### Offered Dataset

>  MBTI-S2Conv dataset

<img src="https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240102153139639.png" alt="image-20240102153139639" style="zoom:33%;" />

##### Evaluation Using AI

Evaluate MBTI-S2Conv【典型的认知行为疗法】

* **Emotional Improvement**: Does the conversation improve the emotional state of the seeker?
* **Problem Solving**: Is the problem solved after the conversation?
* **Active Engagement**: Is the seeker actively **engaged in the conversation？**【interesting】

##### Overview

![image-20240102153715973](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240102153715973.png)

> HHHH, this paper just make chatGPT agent play role-play game, and them expand dataset, and than dynamic retrieve examples for reference.

![image-20240102155221352](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240102155221352.png)

> And this paper also evaluate How different personalities can influent the emotional dialog 

##### Highlights

* **Evaluation using ChatGPT and other LLMs**

* **Beautiful Code for dynamic memory**

* **MBTI-dataset**

* **How to expand the dataset using ChatGPT**


<div style="text-align:center;">
<img src="https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20240102155000886.png" alt="image-20240102155000886" style="zoom:25%;" />
</div>


### Title： E-CORE: Emotion Correlation Enhanced Empathetic Dialogue Generation

* **Keywords**: Emotional Dialog， Small Language Model, Emotional Correlation

#### Link

* **Github\ArXiv\OpenReview**:  [pdf (openreview.net)](https://openreview.net/pdf?id=MbKRJUowYX)

* **Demo**:  close-source

* **One of Authors:** Dr. wang quan [北京邮电大学教师个人主页系统 王泉--中文主页 (bupt.edu.cn)](https://teacher.bupt.edu.cn/wangquan/zh_CN/index.htm)

#### Evaluate

* **Usefulness(1~5)**: 
* **Timing**: 
* **Intensive Reading**: 

#### Abstract



### Title: Towards Interpretable Mental Health Analysis with Large Language Models

* **Keywords**: Kailai Yang, analysing emotional posts using ChatGPT, authors of mental-roberta

#### Link

* **Github\ArXiv\OpenReview**: <https://openreview.net/forum?id=e5UzmaR8EE>

* **Demo**:  

#### Evaluate

* **Usefulness(1~5)**: 5+ Top-tier and relevant paper
* **Timing**:  08 Oct 2023
* **Intensive Reading**: Reproducing

#### Abstract

## Extended Reading

### What is the autonomous agent？

> Autonomous agents are software programs which respond to states and events in their environment independent from direct instruction by the user or owner of the agent, but acting on behalf and in the interest of the owner.

**Reference**

* General autonomous agents capable of reasoning and decision-making in a variety of environments
  (Wooldridge & Jennings, 1995) have been of long-standing interest in the field of artificial intelligence.[[2310.04406\] Language Agent Tree Search Unifies Reasoning Acting and Planning in Language Models (arxiv.org)](https://arxiv.org/abs/2310.04406)

* [Autonomous Agents - ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/B0080430767005349)

Autonomous agents are software programs that **respond**** to states** and events in their environment independent** from direct instruction by the user or owner of the agent, but acting **on behalf** and **in the interest of the owner**. The term agent is not defined precisely, and agent software can range from simple programs composed of a small number of rules to large and complex systems. Agent technology was developed in artificial intelligence (AI) research and can include complex AI techniques. Important application areas are those where the human user can benefit from continuous data analysis, monitoring of data streams and large databases, and where routine reactions to events are required. Many applications are related to user interface technology and the Internet**. A weak position sees agents as tools** that relieve humans from routine tasks suited to computational solutions, but there is also a strong position that asserts that agents can be constructed to mimic or even surpass the cognitive functions of the human.

### How to Scaling LLM

#### SOLAR 10.7B

**SOLAR 10.7B Scaling Large Language Models with Simple yet Effective Depth Up-Scaling**

> 大道至简
> "Simple is the best"

* Keywords: Scaling AI
* Link: <https://arxiv.org/abs/2312.15166>
* **Github**: Invalided
* **Demo**:  <https://huggingface.co/upstage/SOLAR-10.7B-v1.0>
* Chinese Blog: <https://mp.weixin.qq.com/s/uXkLQGd1J8AYh5I5LwWskQ>
Evaluate
* **Usefulness(1~5)**: 2
* **Timing**: 
* **Intensive Reading**: 
* Its method is instinctive and instructive.
* ![](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231229151138905.png)

#### Title： On the Humanity of Conversational AI: Evaluating the Psychological Portrayal of LLMs

* **Keywords**: How to evaluate the psychological Portrayal画像 of LLMs, interesting 

##### Link

* **Github\ArXiv\ OpenReview**: 

* **Demo**:  

##### Evaluate

* **Usefulness(1~5)**: 3
* **Timing**: 
* **Intensive Reading**: 

##### Abstract

Large Language Models (LLMs) have recently showcased their remarkable capacities, not only in natural language processing tasks but also across diverse domains such as clinical medicine, legal consultation, and education. LLMs become more than mere applications, evolving into assistants capable of addressing diverse user requests. This narrows the distinction between human beings and artificial intelligence agents, raising intriguing questions regarding the potential manifestation of personalities, temperaments, and emotions within LLMs. In this paper, we propose a framework, PPBench, for **evaluating diverse psychological aspects of LLMs**. Comprising thirteen scales commonly used in clinical psychology, **PPBench further classifies these scales into four distinct categorie**s: **personality traits,** interpersonal relationships, motivational tests, and emotional abilities. Our study examines five popular models, **namely text-davinci-003, ChatGPT, GPT-4, LLaMA-2-7b, and LLaMA-2-13b.** Additionally, we employ a jailbreak approach to bypass the safety alignment protocols and test the intrinsic natures of LLMs. We have made PPBench openly accessible via The link is hidden due to anonymity. For reviewers, please refer to the supplementary materials.


### Markdown Template

```python
### Title

* **Keywords**:

#### Link

* **Github\ArXiv\OpenReview**: 

* **Demo**:  

#### Evaluate

* **Usefulness(1~5)**: 
* **Timing**: 
* **Intensive Reading**: 


#### Abstract
```

## TODO list

* E-CORE: Emotion Correlation Enhanced Empathetic Dialogue Generation
* Language and Mental Health: Measures of Emotion Dynamics from Text as Linguistic Biosocial Markers
* Discovering Divergences between Language Models and Human Brains （emotional relate）
* VISUO-EMOTIONAL PERCEPTION AND HUMAN COGNITI0ON TO ENGINEER CONTENT GENERATION USING GENERATIVE AI
* Aligning Language Models with Human Preferences via a Bayesian Approach. [long-term works]
* [Complementary Explanations for Effective In-Context Learning](https://arxiv.org/abs/2211.13892) []

## Ideas

* Propose new metricses to calculate efficiency [result/tokens, GPU, step]

## Comments/tips

* OpenReview is a good website, with abundant review \ rebuttal. Interesting!
* The number of emotional dialog papers is so limited! (after 2023) Ah! The ChatGPT eliminates many small domain researches.
* <https://openreview.net/forum?id=e5UzmaR8EE>
* An Annotated Dataset for Explainable Interpersonal Risk Factors of Mental Disturbance in Social Media Posts [ACL2023 FINDING]
* [YeRyeongLee/mental-bert-base-uncased-finetuned-0505 · Adding `safetensors` variant of this model (huggingface.co)](https://huggingface.co/YeRyeongLee/mental-bert-base-uncased-finetuned-0505/discussions/1) Reproduce
* [mental/mental-bert-base-uncased · Hugging Face](https://huggingface.co/mental/mental-bert-base-uncased) Reproduce
* <!-- 其实现在就是两个可以借鉴的地方，第一个就是agent！agent think tank +人工评测+第二就是加上token/时间 Tokens/显存 计算的agent智囊团 后面再探索自我组织！ 下一步探索什么？agent 相关度？让孙泽楷负责写streamlit 我必须竟可能快的实现动态提示改写-动态内存-多智能体改写-多智能体自组织！先实现功能，再重写代码 尽快推进 -->
* <!-- Emotional Dialog papers are scarce -->
<!-- 做个屁的共情对话，赶紧润了，妈的 -->
<!-- 尽快测试agentVerse 吧，赶紧抄一个做可视化 -->
