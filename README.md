# AI Learning Resources
last updated: July 6, 2026

A curated list of AI learning resources I’ve found useful, roughly in the order I’d recommend reading them.

#### TODO
- Add resources on inference optimization, agentic engineering, cognitive/societal effects of AI, trustworthy AI, etc.
- Add intermediate courses between CME295 and CS336

## Table of Contents
1. [AI Engineering Overview](#ai-engineering-overview)  
2. [Architectures](#architectures)
   - [Transformers](#transformers)
   - [LLMs](#llms)
3. [Training](#training)
   - [How to Train LMs](#how-to-train-lms)
   - [Post-training](#post-training)
4. [Inference Optimization](#inference-optimization)
5. [Advanced: Modern LM Systems](#advanced-modern-lm-systems)
6. [Agents](#agents)
   - [What Is an Agent?](#what-is-an-agent)
   - [Agentic Engineering](#agentic-engineering)
   - [Agent Security](#agent-security)
7. [AI "Safety"](#ai-safety)
   - [Overview](#overview)
   - ["Alignment"](#alignment)
8. [AI Writing Smells](#ai-writing-smells)


## AI Engineering Overview
- Chip Huyen. *AI Engineering*. O'Reilly. Dec 2024.
  > 칩 후옌. *AI 엔지니어링*. 한빛미디어.<br>
  > a very good overview of the full AI engineering stack. If you read only one thing from this list, make it this. it covers the basics of llm systems, evaluation, data, rag, finetuning, agents, inference optimization, prompt engineering, and more. 

## Architectures
### Transformers
- Jay Alammar & Maarten Grootendorst. Ch 3: Inside Large Language Models, in *Hands-on Large Language Models*. O'Reilly. Sep 2024. 
  > 제이 알아마르 & 마르턴 흐루턴도르스트. *핸즈온 LLM*. 3장: 대규모 언어 모델 자세히 살펴보기. 한빛미디어.<br>
  > based on Jay Alammar's [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) (2017),  but better and more comprehensive. 

#### Optional: More on Transformers
- 0xkato. [How LLMs Actually Work](https://www.0xkato.xyz/how-llms-actually-work/). June 2026.
  > a bit more on transformers, including residual connections and layer norm
- Lucas Bayer. [Transformer Tutorial](lucasb.eyer.be/transformer). Sep 2022.
  > includes a tiny bit of math; assumes basic knowledge of probability and linear algebra
- Devi's blog. [Beyond the Curve: A Holistic Guide to Activation Functions (From Sigmoid to SwiGLU)](https://ai.plainenglish.io/beyond-the-curve-a-holistic-guide-to-activation-functions-from-sigmoid-to-swiglu-3e96faaa7a84). Jan 2026.

### LLMs
- Jay Alammar & Maarten Grootendorst. Ch 9: Multimodal Large Language Models, in *Hands-on Large Language Models*. O'Reilly. Sep 2024.
  > 제이 알아마르 & 마르턴 흐루턴도르스트. *핸즈온 LLM*. 9장: 멀티모달 대규모 언어 모델. 한빛미디어.<br>
- Maarten Grootendorst. [A Visual Guide to Reasoning LLMs](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-reasoning-llms). Feb 2025.
  - [A Visual Guide to Mixture of Experts](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts). Oct 2024.
  - [A Visual Guide to Quantization](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-quantization). Jul 2024.
    - Sam Rose. [Quantization from the Ground Up](https://ngrok.com/blog/quantization). *ngrok blog*. Mar 2026.
      > read this before the article above
  - [A Visual Guide to Gemma 4](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-gemma-4). Apr 2026.
    > a good snapshot of early-2026 model architecture: multimodality, MoE, GQA, speculative decoding, MTP, etc.
  - [A Visual Guide to DiffusionGemma](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-diffusiongemma). Jun 2026.
    > also a good intro to diffusion
  - [A Visual Guide to Mamba and State Space Models](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mamba-and-state). Feb 2024.

## Training
### How to Train LMs
- Kyongchun Cho. [You Want to Train Language Models Yourself from Scratch](https://drive.google.com/file/d/1ZOk79Q5PWi9u3erpufiejy5HdHd_ybYT/view). CHIL. 2024.
  > we need much more transparency across every part of AI systems: data, pre-training, post-training, safeguards, deployment, monitoring, versioning, and everything between 
- Yann Dubois. [Introduction to Training LLMs](https://agenticai-learning.org/slides/lecture1.pdf). *CS294/194-196: Agentic AI*. UC Berkeley. Fall 2025.
  > might be a bit difficult if you are new to training llms. but it's a good overview of the entire process
- Nathan Lambert. [The ML Foundations of LLM Post-Training](https://rlhfbook.com/course#prerequisites). Jun 2026.
  > includes a bit of math; assumes basic knowledge of ml, probability, and linear algebra<br>
  > [Nathan Lambert](https://x.com/natolambert) is a must follow for post-training
- Kylo Lo, Akshita Bagia, & Nathan Lambert. [Language Modeling](https://natolambert.com/slides). NeurIPS. Dec 2024.

### Post-training
- Nathan Lambert. [Building Language Models in the Era of Agents](https://natolambert.com/slides). Feb 2026.
  - [Frontier Post-Training Recipe Survey](https://rlhfbook.com/teach/course/conversation-01). Jun 2026.

## Inference Optimization
> under construction

## Advanced: Modern LM Systems
- Sebastian Raschka. *[Machine Learning FAQs](https://sebastianraschka.com/faq/index.html)*
  > a good list of questions that you can learn a lot from
- Afshine Amidi & Shervine Amidi. *[CME295: Transformer & Large Language Models](https://cme295.stanford.edu)*. Stanford University. Fall 2025.
  > assumes basic knowledge of ml, probability, and linear algebra
- Percy Liang & Tatsunori Hashimoto. *[CS336: Language Modeling from Scratch](https://cs336.stanford.edu)*. Stanford University. Spring 2026.
  > assumes basic knowledge of ml, probability, and linear algebra + transformers/llms. the assignments are the heart of the course, but they take a lot of work. still highly worthwhile even if you only read through the materials
- Alisa Liu. [Alisa's Book of LLMs](https://alisawuffles.notion.site/alisa-s-book-of-llms). Jun 2026.
  > a good cs336-level summary

## Agents
### What Is an Agent?
- Ben Recht. [Secrets of Intelligence Services](https://www.argmin.net/p/secrets-of-intelligence-services). Feb 2026.
- Thomas Ptacek. [You Should Write an Agent](https://fly.io/blog/everyone-write-an-agent/). *fly.io blog*. Nov 2025.
  > shows the "magic" of agents
- Grant Bourzikas. [Project Glasswing: What Mythos Showed Us](https://blog.cloudflare.com/cyber-frontier-models/). *The Cloudflare Blog*. May 2026.
  > putting this here instead of under [Agent Security](#agent-security) on purpose

#### Optional: Mechanics of an Agent
> for a closer look at how agents actually work
- Hugging Face. [Agent Course: Unit 1](https://huggingface.co/learn/agents-course/unit1/introduction). Feb 2025.
- OpenAI. [Function Calling](https://developers.openai.com/api/docs/guides/function-calling). *OpenAI Developer Docs.*
- Michael Bolin. [Unrolling the Codex Loop](https://openai.com/index/unrolling-the-codex-agent-loop/). *OpenAI Engineering Blog*. Jan 2026.
- Bo Xu et al. [From model to agent: Equipping the Responses API with a computer environment](https://openai.com/index/equip-responses-api-computer-environment/). *OpenAI Engineering Blog*. Mar 2026.
- 자손킴(jasonkim). [Claude API의 Request Body 분석](https://hackers.pub/@jasonkim/2025/claude-api-request-body). Dec 2025.
  - [Claude Code의 거의 모든 것은 Tool Use입니다. MCP도 subagent도 skills 역시요](https://hackers.pub/@jasonkim/2025/agent-tool-use). Dec 2025.
  - [Subagent는 Tool Use입니다](https://hackers.pub/@jasonkim/2025/subagent-is-tool-use). Dec 2025.
  - [MCP도 Tool Use를 사용합니다](https://hackers.pub/@jasonkim/2025/mcp-is-tool-use). Dec 2025.

### Agentic Engineering
- Mario Zechner. [Prompts Are Code, .json/.md Files Are State](https://mariozechner.at/posts/2025-06-02-prompts-are-code/). Jun 2025.
  > the creator of Pi was early to the current "loop engineering" trend
- Nader Dabit. [You Could've Invented OpenClaw](https://gist.github.com/dabit3/bc60d3bea0b02927995cd9bf53c3db32). Feb 2026.
  > explains how openclaw works

### Agent Security
- Simon Willison. [The Lethal Trifecta for AI Agents: Private data, Untrusted Content, and External Communication](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/). Jun 2025.
  > as Willison himself says, "lethal trifecta" is a catchy phrase. and it's a good framework
- ACSC, CISA, NSA, Cyber Center, NCSC NZ, & NCSC UK. *[Careful Adoption of Agentic AI Services](https://www.cyber.gov.au/business-government/secure-design/artificial-intelligence/careful-adoption-of-agentic-ai-services)*. May 2026.
  > should be required reading for anyone implementing ai agents in real systems
- Rich Harang. [Practical Security Guidance for Sandboxing Agentic Workflows and Managing Execution Risk](https://developer.nvidia.com/blog/practical-security-guidance-for-sandboxing-agentic-workflows-and-managing-execution-risk/). *NVIDIA Technical Blog*. Jan 2026.
  > should also be required reading for anyone implementing ai agents in real systems
  - David Dworken & Oliver Weller-Davie. [Beyond permission prompts: making Claude Code more secure and autonomous](https://www.anthropic.com/engineering/claude-code-sandboxing). *Engineering at Anthropic*. Oct 2025.
    > "It is worth noting that **effective sandboxing requires both filesystem and network isolation**. Without network isolation, a compromised agent could exfiltrate sensitive files like SSH keys; without filesystem isolation, a compromised agent could easily escape the sandbox and gain network access."
  - Luis Cardoso. [A Field Guide to Sandboxes for AI](https://www.luiscardoso.dev/blog/sandboxes-for-ai). Jan 2026.
    > a thorough introduction to containers, gVisor, microVMs, and WASM/isolates<br>
    > > "containers are not a sufficient security boundary for hostile code. ... they still share the host kernel."
  - [Sandboxing Agents with AI Workbench](https://docs.nvidia.com/ai-workbench/user-guide/latest/concepts/sandboxing-concept.html). *NVIDIA AI Workbench User Guide*
    > "What Sandboxing Does Not Cover
    > - Process sandboxes in containers do not isolate environment variables.
    > - Some agent sandboxes fail silently in containers.
    > - **Agent guidance does not actually enforce anything, so make sure to use permissions and hooks.** <br>
    >   MDC rules, skills, and CLAUDE.md files inform the agent about constraints and conventions, but **the agent can ignore them.**"
- Marcus Williamson et al. [Types of Misalignment](misalignment.md). Adapted from [How We Monitor Internal Coding Agents for Misalignment](https://openai.com/index/how-we-monitor-internal-coding-agents-misalignment/). *OpenAI Safety Blog*. May 2026.
  > how agents can fail to work as intended

## AI "Safety"
### Overview
- Ben Recht. [The Banal Evil of AI Safety](https://www.argmin.net/p/the-banal-evil-of-ai-safety). Aug 2025.
  > every AI "safety" researcher should read this
- Peter Slattery et al. [Taxonomy of AI Risks](DomainTaxonomyofAIRisks.md). Adapted from [The AI risk repository: A meta-review, database, and taxonomy of risks from artificial intelligence](https://airisk.mit.edu/risks). Mar 2026.
  > a good framework
- Yoshua Bengio et al. *[International AI Safety Report 2026](https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026)*. Feb 2026.
  > a good reference

### "Alignment"
- Séb Krier. [Scary Model Cards and the Discourse Shifting](https://x.com/sebkrier/status/2020561261751062664). Feb 2026.
  > "many public readings of some evaluations implicitly treat chat outputs as direct evidence of properties inherent to models, while LLM behavior is often strongly role- and context-conditioned. As a result commentators sometimes miss what the model is actually doing (simulating a role given textual context), design tests that are highly stylized (because they don't bother to make the scenarios psychologically plausible to the model), and interpret the results through a framework (goal-directed rational agency) that doesn't match the underlying mechanism (text prediction via theory-of-mind-like inference). <br>
  > 1. The model is completing a text, not answering a question 
  > 2. The assistant persona is a fictional character, not the model itself 
  > 3. Apparent errors are often correct completions of the world implied by the prompt
  > 4. “Evaluation awareness” isn't mystical: the model can recognize contrivance because it’s a strong reader
  > 5. Post-training mostly narrows/reshapes behavior, and it can both help and distort."
- Christopher Summerfield et al. [Lessons from a Chimp: AI ‘Scheming’ and the Quest for Ape Language](https://arxiv.org/pdf/2507.03409). Jul 2025.
  > " 1. Many of the claims hinge on anecdotal evidence.
  >   2. Studies often lack hypotheses and control conditions
  >   3. Studies have weak or unclear theoretical motivation
  >   4. Findings are often interpreted in exaggerated or unwarranted ways"

## AI Writing Smells
- Sam Kriss. [Why Does A.I. Write Like … That?](https://www.nytimes.com/2025/12/03/magazine/chatbot-writing-style.html). *The New York Times*. Dec 2025.
  - Wikipedia. [Signs of AI Writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).
  - Shiv Bosale. [Various LLM Smells](https://shvbsle.in/various-llm-smells/). May 2026.
  - Sarah Perez. [OpenAI Says It’s Fixed ChatGPT’s Em dash Problem](https://techcrunch.com/2025/11/14/openai-says-its-fixed-chatgpts-em-dash-problem/). *TechCrunch*. Nov 2025.
  - Shaina Mishkin. [It's Not Just a Trend, It's a Phenomenon](images/itsnot.webp). From [AI Is Changing How Companies Talk to Shareholders. Here Is the Red Flag for Readers](https://www.barrons.com/articles/ai-corporate-communications-shareholders-red-flag-63211618). *Barron's*. Apr 2026.
- Nathan Lambert. [Why AI Writing is Mid](https://www.interconnects.ai/p/why-ai-writing-is-mid). Nov 2025.
- Lina Abushouk. [How to Read Postcolonial Writing](https://africasacountry.com/2026/05/how-to-read-postcolonial-writing). *Africa Is a Country*. May 2026.
