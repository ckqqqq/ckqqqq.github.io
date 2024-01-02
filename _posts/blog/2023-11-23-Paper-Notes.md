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

* **Keyword**:

#### Link

* **Github\ArXiv**: 

* **Demo**:  

#### Evaluate

* **Usefulness(1~5)**: 
* **Timing**: 
* **Intensive Reading**: 


#### Abstract
```


## LLM / LLM-Agent Related Papers

### Title: WEBARENA: A REALISTIC WEB ENVIRONMENT FOR BUILDING AUTONOMOUS AGENTS

Keyword：Web-agent，
Link：

* Github\Arixiv: <https://arxiv.org/pdf/2307.13854.pdf>
* Open-source: yes
* **Demo**:  <https://webarena.dev/>
Evaluate:
* **Usefulness(1~5)**: 3
* **Timing**: 2023.10
* **Intensive Reading**: No
Abstract:
A useful LLM-base agent that can manipulate Web UI. The demo is interesting.The interaction way between LLM and web is of reference value.

### Title: Hierarchical Prompting Assists Large Language Model on Web Navigation

Keyword：Web Agent, Hierarchical Prompting, EMNLP fINDINGS
Link

* **Github**: <https://github.com/robert1003/ash-prompting>
* **Demo**:  No
Evaluate
* **Usefulness(1~5)**: 4.5
* **Timing**: Oct 25th, 2023
* **Intensive Reading**: TODO
  Abstract:
  He looks like he wrote a framework/system into two articles.This meod is similar with ReAct.
  ![Alt text](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image.png)

### Title: FIREACT: Toward LANGUAGE AGENT FINE-TUNING

Keyword: ReACT+ Finetune, Ablation Experiment, LM fine-tuning，
Link

* Github:

* **Demo**: 
  Evaluate

* **Usefulness(1~5)**: 5

* **Timing**: Oct 9,2023

* **Intensive Reading**: yes
  Abstract:

* The article's structure is logical, conherent and complete, making is easy to follow.

* The related work part of the article is detailed, in-depth and informative,providing valuable conclusion

* This paper compare the many methods, including fine-tune & prompt & TOOL, reAct & reflexion & CoT.

![image-20231217110322487](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217110322487.png)

Useful Conclusion:

* Finetuning GPT-3.5 only cost 10 dollars.
* LLama-7B models could be fine-tuned to catch up with GPT-3.5 performances.
* Dr. Yao has in-depth and extensive investigations of LMagent-related works.

![image-20231217112034478](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217112034478.png)

### Title: SWE-BENCH: CAN LANGUAGE MODELS RESOLVE REAL-WORLD GITHUB ISSUES?

Keyword：LLM-assist Code-generation, Github issues
Link

* **Github**:  <https://www.swebench.com>.
* **Demo**: 
Evaluate
* **Usefulness(1~5)**: 2
* **Timing**: Oct 10, 2023
* **Intensive Reading**:
Abstract:


### Title:Embers of Autoregression: Understanding Large Language Models Through the Problem They are Trained to Solve

Keyword：Summarize, interesting figures, comprehensive, wonderful explanation of next-word prediction, Frequency determines quality (mian idea).
Link

* **Github**: <https://github.com/tommccoy1/embers-of-autoregression> (mission impossible of LLMs)
* **Demo**:  
Evaluate
* **Usefulness(1~5)**: 
* **Timing**: 
* **Intensive Reading**: 
Abstract: 

* This figure can be improved.(What are the capacities of Human & LLM?)
![Alt text](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-1.png)
* This paper exhibit what might seem like surpriging failunres of LLMs on tasks taht are straightforward for humans to perform.

![image-20231217150042407](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217150042407.png)

* Supplement

|           | Unique human capacities                  | Shared | LLM's capacities |
| --------- | ---------------------------------------- | ------ | ---------------- |
| Math      | Counting、Ciphers、Linear Functions      |        | COT?             |
| Language  | Word/letter reverse、Acronyms、Pig latin |        | World knowledge  |
| Physical  | LeCun's world models                     |        |                  |
| Training  | Efficiency                               |        |                  |
| Frequency |                                          |        |                  |
(failures of planning in arithmetic and text generation)

Effects on the performance of large language models that are attributable to the fact that they are statistical next-word prediction systems.

![image-20231217153534032](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217153534032.png)

### Title: Cognitive Architectures for Language Agents
Keyword：New agents' framework, Control flow, Symbolic AGI
Link

* **Github**:  <https://github.com/ysymyth/awesome-language-agents>
* <img src="https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217165037780.png" alt="image-20231217165037780" style="zoom:25%;" />
* **Demo**: 
Evaluate
* **Usefulness(1~5)**: 4.9
* **Timing**: Sep 25, 2023
* **Intensive Reading**: True
  Abstract: Porposed a complex agent frameworks

![image-20231217164349549](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164349549.png)

![image-20231217164558289](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164558289.png)

![image-20231217164657449](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164657449.png)

![image-20231217164848939](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164848939.png)

### TODO-12-17

* Practice Oral English and prepare for interview
* Check the reference papers of  [CoALA](https://github.com/ysymyth/awesome-language-agents?tab=readme-ov-file)
* Step1:Finetune
* Step2:Framework

### 12-28

Phase I completed

### Agents: An Open-source Framework for Autonomous Language Agents 【Multi-Agents】

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

### AgentVerse 【Multi-Agent】

* **Keyword**：Multiple LLM-based agents for task-solving and simulation,
  Link

* **Github**: <https://github.com/OpenBMB/AgentVerse>

* **Demo**:  <https://github.com/OpenBMB/AgentVerse>
  Evaluate

* **Usefulness(1~5)**: 4

* **Timing**: Aug,2023

* **Intensive Reading**: TODO 

* Abstract: **AgentVerse** is designed to facilitate the deployment of multiple LLM-based agents in various applications. AgentVerse primarily provides two frameworks: **task-solving** and **simulation**.

  * Task-solving: This framework assembles multiple agents as an automatic multi-agent system ([AgentVerse-Tasksolving](https://arxiv.org/pdf/2308.10848.pdf), [Multi-agent as system](https://arxiv.org/abs/2309.02427)) to collaboratively accomplish the corresponding tasks. Applications: software development system, consulting system, etc.

  [![Screen Shot 2023-09-01 at 12 08 57 PM](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/264917097-6db1c907-b7fc-42f9-946c-89853a28f386.png)](https://private-user-images.githubusercontent.com/11704492/264917097-6db1c907-b7fc-42f9-946c-89853a28f386.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDM5Mzc5MDgsIm5iZiI6MTcwMzkzNzYwOCwicGF0aCI6Ii8xMTcwNDQ5Mi8yNjQ5MTcwOTctNmRiMWM5MDctYjdmYy00MmY5LTk0NmMtODk4NTNhMjhmMzg2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyMzEyMzAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjMxMjMwVDEyMDAwOFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTkwNDk5Mjk1ZGM5MTBjODE5NzA0ZTFhYTVhNTlkMDViNWYwYjVkOTYyMDdmMmVmNGU0ZGNkZTI3OGVmNmI1NjkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.LcJ8qjM00WMDeCV6cjraehSUPn8XpQfA2Y43OGCk6Eg)

  * Simulation: This framework allows users to set up custom environments to observe behaviors among, or interact with, multiple agents. ⚠️⚠️⚠️ We're refactoring the code. If you require a stable version that exclusively supports simulation framework, you can use [`release-0.1`](https://github.com/OpenBMB/AgentVerse/tree/release-0.1) branch. Applications: game, social behavior research of LLM-based agents, etc.

  [![Screen Shot 2023-10-16 at 10 53 49 PM](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/275622325-4102d1e2-3fe7-4656-aa2c-a218ce1f2c95.png)](https://private-user-images.githubusercontent.com/11704492/275622325-4102d1e2-3fe7-4656-aa2c-a218ce1f2c95.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDM5Mzc5MDgsIm5iZiI6MTcwMzkzNzYwOCwicGF0aCI6Ii8xMTcwNDQ5Mi8yNzU2MjIzMjUtNDEwMmQxZTItM2ZlNy00NjU2LWFhMmMtYTIxOGNlMWYyYzk1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyMzEyMzAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjMxMjMwVDEyMDAwOFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWE0NTgyMzdiMjI4NDg3MzRkZTFmMzVmYTlmNjMzMTgwNTNkODQyZTY4NmU3MzAzOWVmODBjYzkwZmQ1MjU0YTkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.AeHkR0ZdsWHoJaduvXBB89ZKRWbkYvTljeRn5CMWho0)

### CharacterChat 【Role-Play Agents】

* Keyword： Personalized Social Support = Emotional Support + Multi Agents, MBTI Persona Scale.

* Link (<https://arxiv.org/abs/2308.10278>)

* **Github**: <https://github.com/morecry/CharacterChat>
* **Demo**:  
Evaluate
* **Usefulness(1~5)**: 5【TODO: reproduce】
* **Timing**:  Aug 2023
* **Intensive Reading**:
* **TODO**: 20min code reading 
* <font color=red> Proper noun learning</font>: ESC, social support
Abstract: Traditional methods such as **Emotional Support Conversations (ESC)** face challenges in effectively addressing a diverse range of individual personalities. In response, we introduce the **Social Support Conversation (S2Conv)** framework. It comprises a series of support **agents** and the **interpersonal** **matching** mechanism, linking individuals with persona-compatible virtual supporters【Same as I thought in August】. Utilizing persona decomposition based on the MBTI (Myers Briggs Type Indicator)【a scale】, we have created the MBTI-1024 Bank, a group that of virtual characters with distinct profiles. Through improved role-playing prompts with behavior preset and dynamic memory, we facilitate the development of the MBTI-S2Conv dataset, which contains conversations between the characters in the MBTI-1024 Bank. Building upon these foundations, we present CharacterChat, a comprehensive S2Conv system, which includes a conversational model driven by personas and memories, along with an **interpersonal matching plugin model** 【Calculate Attention between personality 】 that dispatches the optimal supporters from the MBTI-1024 Bank for individuals with specific personas. Empirical results indicate the remarkable efficacy of CharacterChat in providing personalized social support and highlight the substantial advantages derivedfrom interpersonal matching. The source code is available in <https://github.com/morecry/CharacterChat>.

## Extended Reading 

## Scaling LLM

### SOLAR 10.7B: Scaling Large Language Models with Simple yet Effective Depth Up-Scaling

> 大道至简
> "Simple is the best"
 
* Keyword: Scaling AI
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