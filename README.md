# AI Learning Resources
Also available in [한국어](https://github.com/kimmodal/AI-Learning-Resources/blob/d58ad091a03009c8df15f24781e762068a89a784/ko/README.md) / Last updated: July 6, 2026

Good AI learning resources I have found useful.
tried to list them in a suggested reading order.

#### TODO
- add annotations
- add materials on: inference optimization, agentic engineering, cognitive/societal effects of AI, trustworthy AI, etc.
- needs to fill the gap between cme295 and cs366

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
  > a very good overview on everything ai engineering. covers: basics of llm systems, evaluation, data, rag, finetuning, agents, inference optimization, agents, prompt engineering. 

## Architectures
### Transformers
- Jay Alammar & Maarten Grootendorst. Ch 3: Inside Large Language Models, in *Hands-on Large Language Models*. O'Reilly. Sep 2024.
  > based on Jay Alammar's [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) (2017) but better and more extensive. 

#### Optional: More on Transformers
- 0xkato. [How LLMs Actually Work](https://www.0xkato.xyz/how-llms-actually-work/). June 2026.
  > a bit more about transformers such as residual connection and layer norm
- Lucas Bayer. [Transformer Tutorial](lucasb.eyer.be/transformer). Sep 2022.
  > a bit more mathematical 
- Devi's blog. [Beyond the Curve: A Holistic Guide to Activation Functions (From Sigmoid to SwiGLU)](https://ai.plainenglish.io/beyond-the-curve-a-holistic-guide-to-activation-functions-from-sigmoid-to-swiglu-3e96faaa7a84). *Artificial Intelligence in Plain English*. Jan 2026.

### LLMs
- Jay Alammar & Maarten Grootendorst. Ch 9: Multimodal Large Language Models, in *Hands-on Large Language Models*. O'Reilly. Sep 2024. 
- Maarten Grootendorst. [A Visual Guide to Reasoning LLMs](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-reasoning-llms). Feb 2025.
  - [A Visual Guide to Mixture of Experts](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts). Oct 2024.
  - [A Visual Guide to Quantization](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-quantization). Jul 2024.
    - Sam Rose. [Quantization from the Ground Up](https://ngrok.com/blog/quantization). *ngrok blog*. Mar 2026.
      > read this before the article above
  - [A Visual Guide to Gemma 4](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-gemma-4). Apr 2026.
    > incorporates everything so far: multimodality, mixture of exports, gqa, speculative decoding + mtp, etc.
  - [A Visual Guide to DiffusionGemma](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-diffusiongemma). Jun 2026.
    > also a good intro to diffusion
  - [A Visual Guide to Mamba and State Space Models](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mamba-and-state). Feb 2024.

## Training
### How to Train LMs
- Kyongchun Cho. [You Want to Train Language Models Yourself from Scratch](https://drive.google.com/file/d/1ZOk79Q5PWi9u3erpufiejy5HdHd_ybYT/view). CHIL. 2024.
- Yann Dubois. [Introduction to Training LLMs](https://agenticai-learning.org/slides/lecture1.pdf). *CS294/194-196: Agentic AI*. UC Berkeley. Fall 2025.
  > could be a bit difficult if you are new to training llms. but a great summary/overview of the entire process. 
- Nathan Lambert. [The ML Foundations of LLM Post-Training](https://rlhfbook.com/course#prerequisites). Jun 2026.
- Kylo Lo, Akshita Bagia, & Nathan Lambert. [Language Modeling](https://natolambert.com/slides). NeurIPS. Dec 2024.

### Post-training
- Nathan Lambert. [Building Language Models in the Era of Agents](https://natolambert.com/slides). Feb 2026.
  - [Frontier Post-Training Recipe Survey](https://rlhfbook.com/teach/course/conversation-01). Jun 2026.

## Inference Optimization

## Advanced: Modern LM Systems
- Sebastian Raschka. *[Machine Learning FAQs](https://sebastianraschka.com/faq/index.html)*
- Afshine Amidi & Shervine Amidi. *[CME295: Transformer & Large Language Models](https://cme295.stanford.edu)*. Stanford University. Fall 2025.
  > assumes a basic knowledge of ml, probability, and linear algebra
- Percy Liang & Tatsunori Hashimoto. *[CS336: Language Modeling from Scratch](https://cs336.stanford.edu)*. Stanford University. Spring 2026.
  > assumes a basic knowledge of ml, probability, and linear algebra + transformers/llms. assignments are the most critical parts and extremely load-bearing, but course material (including assignments guide) are highly valuable too
- Alisa Liu. [Alisa's Book of LLMs](https://alisawuffles.notion.site/alisa-s-book-of-llms). Jun 2026.
  > a good summary at the level of cs336

## Agents
### What Is an Agent?
- Ben Recht. [Secrets of Intelligence Services](https://www.argmin.net/p/secrets-of-intelligence-services). Feb 2026.
- Thomas Ptacek. [You Should Write an Agent](https://fly.io/blog/everyone-write-an-agent/). *fly.io blog*. Nov 2025.
  > shows the "magic" of agents
- Grant Bourzikas. [Project Glasswing: What Mythos Showed Us](https://blog.cloudflare.com/cyber-frontier-models/). *The Cloudflare Blog*. May 2026.
  > it's not a mistake to have it on this section instead of agent security. 

#### Optional: Mechanics of an Agent
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
  > the creator of pi foresaw the current "loop engineering" trend
- Nader Dabit. [You Could've Invented OpenClaw](https://gist.github.com/dabit3/bc60d3bea0b02927995cd9bf53c3db32). Feb 2026.
  > how openclaw works

### Agent Security
- Simon Willison. [The Lethal Trifecta for AI Agents: Private data, Untrusted Content, and External Communication](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/). Jun 2025.
- ACSC, CISA, NSA, Cyber Center, NCSC NZ, & NCSC UK. *[Careful Adoption of Agentic AI Services](https://www.cyber.gov.au/business-government/secure-design/artificial-intelligence/careful-adoption-of-agentic-ai-services)*. May 2026.
  > should be a required reading for anyone who implements ai agents to their systems
- Rich Harang. [Practical Security Guidance for Sandboxing Agentic Workflows and Managing Execution Risk](https://developer.nvidia.com/blog/practical-security-guidance-for-sandboxing-agentic-workflows-and-managing-execution-risk/). *Nvidia Technical Blog*. Jan 2026.
  > also should be a required reading for anyone who implements ai agents to their systems
  - David Dworken & Oliver Weller-Davie. [Beyond permission prompts: making Claude Code more secure and autonomous](https://www.anthropic.com/engineering/claude-code-sandboxing). *Engineering at Anthropic*. Oct 2025.
    > "It is worth noting that **effective sandboxing requires both filesystem and network isolation**. Without network isolation, a compromised agent could exfiltrate sensitive files like SSH keys; without filesystem isolation, a compromised agent could easily escape the sandbox and gain network access. It’s by using both techniques that we can provide a safer and faster agentic experience for Claude Code users."
  - Luis Cardoso. [A Field Guide to Sandboxes for AI](https://www.luiscardoso.dev/blog/sandboxes-for-ai). Jan 2026.
    > "containers are not a sufficient security boundary for hostile code. They can be hardened, and that matters. But they still share the host kernel. The failure modes I see most often are misconfiguration and kernel/runtime bugs — plus a third one that shows up in AI systems: policy leakage."
- Marcus Williamson et al. [Types of Misalignment](misalignment.md). Adapted from [How We Monitor Internal Coding Agents for Misalignment](https://openai.com/index/how-we-monitor-internal-coding-agents-misalignment/). *OpenAI Safety Blog*. May 2026.
  > how agents don't work as intended

## AI "Safety"
### Overview
- Ben Recht. [The Banal Evil of AI Safety](https://www.argmin.net/p/the-banal-evil-of-ai-safety). Aug 2025.
- Peter Slattery et al. [Taxonomy of AI Risks](DomainTaxonomyofAIRisks.md). Adapted from [The AI risk repository: A meta-review, database, and taxonomy of risks from artificial intelligence](https://airisk.mit.edu/risks). Mar 2026.
- Yoshua Bengio et al. *[International AI Safety Report 2026](https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026)*. Feb 2026.

### "Alignment"
- Séb Krier. [Scary Model Cards and the Discourse Shifting](https://x.com/sebkrier/status/2020561261751062664). Feb 2026.
- Christopher Summerfield et al. [Lessons from a Chimp: AI ‘Scheming’ and the Quest for Ape Language](https://arxiv.org/pdf/2507.03409). Jul 2025.

## AI Writing Smells
- Sam Kriss. [Why Does A.I. Write Like … That?](https://www.nytimes.com/2025/12/03/magazine/chatbot-writing-style.html). *The New York Times*. Dec 2025.
  - Wikipedia. [Signs of AI Writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing). 
  - Shiv Bosale. [Various LLM Smells](https://shvbsle.in/various-llm-smells/). May 2026.
  - Sarah Perez. [OpenAI Says It’s Fixed ChatGPT’s Em dash Problem](https://techcrunch.com/2025/11/14/openai-says-its-fixed-chatgpts-em-dash-problem/). *TechCrunch*. Nov 2025.
  - Shaina Mishkin. [It's Not Just a Trend, It's a Phenomenon](images/itsnot.webp). From [AI Is Changing How Companies Talk to Shareholders. Here Is the Red Flag for Readers](https://www.barrons.com/articles/ai-corporate-communications-shareholders-red-flag-63211618). *Barron's*. Apr 2026. 
- Nathan Lambert. [Why AI Writing is Mid](https://www.interconnects.ai/p/why-ai-writing-is-mid). Nov 2025.
- Lina Abushouk. [How to Read Postcolonial Writing](https://africasacountry.com/2026/05/how-to-read-postcolonial-writing). *Africa Is a Country*. May 2026.
