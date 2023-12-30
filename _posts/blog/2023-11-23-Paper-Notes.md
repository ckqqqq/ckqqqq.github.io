---
layout: post
title: Research Notes
categories: blog
description: Hey, welcome to my research notes.
keywords: AI Papers, Publications
---
Welcome! This blog contains my notes on reading papers related to LMs-agents and emotional dialog.





​                               

## Markdown Template

这是模板

### Title:
Keyword：
Link
* Github: 
* Demo: 
Evaluate
* Usefulness(1~5): 
* Timing: 
* Intensive Reading: 
Abstract: 


## LLM

Large language model

### Title:WEBARENA: A REALISTIC WEB ENVIRONMENT FOR BUILDING AUTONOMOUS AGENTS
Keyword：Web-agent，
Link：
* Github\Arixiv: https://arxiv.org/pdf/2307.13854.pdf
* Open-source: yes
* Demo: https://webarena.dev/
Evaluate:
* Usefulness(1~5): 3
* Timing: 2023.10
* Intensive Reading: No
Abstract:
A useful LLM-base agent that can manipulate Web UI. The demo is interesting.The interaction way between LLM and web is of reference value.

### Title: Hierarchical Prompting Assists Large Language Model on Web Navigation
Keyword：Web Agent, Hierarchical Prompting, EMNLP fINDINGS
Link
* Github: https://github.com/robert1003/ash-prompting
* Demo: No
Evaluate
* Usefulness(1~5): 4.5
* Timing: Oct 25th, 2023
* Intensive Reading: TODO
  Abstract: 
  He looks like he wrote a framework/system into two articles.This meod is similar with ReAct.
  ![Alt text](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image.png)

### FIREACT: TOward LANGUAGE AGENT FINE-TUNING
Keyword: ReACT+ Finetune, Ablation Experiment, LM fine-tuning，
Link
* Github: 

* Demo: 
  Evaluate

* Usefulness(1~5): 5

* Timing: Oct 9,2023

* Intensive Reading: yes
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
* Github:  https://www.swebench.com.
* Demo: 
Evaluate
* Usefulness(1~5): 2
* Timing: Oct 10, 2023
* Intensive Reading: 
Abstract: 


### Title:Embers of Autoregression: Understanding Large Language Models Through the Problem They are Trained to Solve
Keyword：Summarize, interesting figures, comprehensive, wonderful explanation of next-word prediction, Frequency determines quality (mian idea).
Link
* Github: https://github.com/tommccoy1/embers-of-autoregression (mission impossible of LLMs)
* Demo: 
Evaluate
* Usefulness(1~5): 
* Timing: 
* Intensive Reading: 
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

Effects on the performance of large language models that are attributable to the fact that they are statistical next-word prediction systems 

![image-20231217153534032](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217153534032.png)

### Title: Cognitive Architectures for Language Agents
Keyword：New agents' framework, Control flow, Symbolic AGI, 
Link
* Github:  https://github.com/ysymyth/awesome-language-agents
* <img src="https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217165037780.png" alt="image-20231217165037780" style="zoom:25%;" />
* Demo: 
Evaluate
* Usefulness(1~5): 4.9
* Timing: Sep 25, 2023
* Intensive Reading: 
  Abstract: Porposed a complex agent frameworks

![image-20231217164349549](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164349549.png)

![image-20231217164558289](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164558289.png)


![image-20231217164657449](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164657449.png)


![image-20231217164848939](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231217164848939.png)

### TODO-12-17

* Practice Oral English and prepare for interview
* Check the reference papers of  [CoALA](https://github.com/ysymyth/awesome-language-agents?tab=readme-ov-file)
*  Step1:Finetune
*  Step2:Framework

### 12-28 

Phase I completed

### Agents: An Open-source Framework for Autonomous Language Agents

Keyword： multi-Agents, Autonomous Agents
Link

* Github: https://github.com/aiwaves-cn/agents

* Demo:

   ![image-20231228131805241](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231228131805241.png)
  Evaluate：

  ![image-20231228131902233](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231228131902233.png)

* Usefulness(1~5): 

* Timing: 

* Intensive Reading: 
Abstract: 

> TO-DO 12-29
> Read https://arxiv.org/pdf/2311.16832.pdf
> Reproduce Code
> Try Character.ai
> Finish Dynamic Memory Component
### CharacterChat
* Keyword： Personalized Social Support

* Link (https://arxiv.org/abs/2308.10278)

* Github: https://github.com/morecry/CharacterChat
* Demo: 
Evaluate
* Usefulness(1~5): 
* Timing: 
* Intensive Reading: 
Abstract: 
* 

 Traditional methods such as **Emotional Support Conversations (ESC)** face challenges in effectively addressing a diverse range of individual personalities. In response, we introduce the **Social Support Conversation (S2Conv)** framework. It comprises a series of support **agents** and the **interpersonal** **matching** mechanism, linking individuals with persona-compatible virtual supporters【Same as I thought in August】. Utilizing persona decomposition based on the MBTI (Myers Briggs Type Indicator)【a scale】, we have created the MBTI-1024 Bank, a group that of virtual characters with distinct profiles. Through improved role-playing prompts with behavior preset and dynamic memory, we facilitate the development of the MBTI-S2Conv dataset, which contains conversations between the characters in the MBTI-1024 Bank. Building upon these foundations, we present CharacterChat, a comprehensive S2Conv system, which includes a conversational model driven by personas and memories, along with an **interpersonal matching plugin model** 【Calculate Attention between personality 】 that dispatches the optimal supporters from the MBTI-1024 Bank for individuals with specific personas. Empirical results indicate the remarkable efficacy of CharacterChat in providing personalized social support and highlight the substantial advantages derivedfrom interpersonal matching. The source code is available in https://github.com/morecry/CharacterChat.

## Extended Reading



## Scaling AI
### SOLAR 10.7B: Scaling Large Language Models with Simple yet Effective Depth Up-Scaling

> 大道至简
> "Simple is the best"

* Keyword: Scaling AI
* Link: https://arxiv.org/abs/2312.15166
* Github: Invalided
* Demo: https://huggingface.co/upstage/SOLAR-10.7B-v1.0
* Chinese Blog: https://mp.weixin.qq.com/s/uXkLQGd1J8AYh5I5LwWskQ
Evaluate
* Usefulness(1~5): 2
* Timing: 
* Intensive Reading: 
Abstract: 
* Its method is instinctive and instructive.
* ![](https://ckqqqq-qiker-image-service.oss-cn-beijing.aliyuncs.com/typora-image/image-20231229151138905.png)