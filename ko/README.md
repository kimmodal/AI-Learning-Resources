# AI Learning Resources
Good AI learning resources I have found useful.<br>
I tried to list them in a suggested reading order.

**TODO**
- Add brief annotations for each resource.

## Table of Contents
1. [AI Engineering Overview](#ai-engineering-overview)  
2. [Architectures](#architectures)  
   - [Transformers](#transformers)
   - [Further Topics](#further-topics)
3. [Training](#training)
   - [How to Train LMs](#how-to-train-lms)
   - [Post-training](#post-training)
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
- 칩 후옌. *AI 엔지니어링*. (Chip Huyen. *AI Engineering*). 2024.

## Architectures
- 제이 알아마르 & 마르턴 흐루턴도르스트. *핸즈온 LLM*, 3장: 대규모 언어 모델 자세히 살펴보기. (Jay Alammar & Maarten Grootendorst. *Hands-on Large Language Models*). 2024.
  - 9장: 멀티모달 대규모 언어 모델
- 마르턴 흐루턴도르스트. [Reasoning LLMs에 관한 비주얼 가이드](https://tulip-phalange-a1e.notion.site/Reasoning-LLMs-190c32470be2806d834ee0ad98aaa0b6) ([A Visual Guide to Reasoning LLMs](https://newsletter.maartengrootendorst.com/pa-visual-guide-to-reasoning-llms)). Feb 2025.
  - [Mixture of Experts (MoE)에 관한 비주얼 가이드](https://tulip-phalange-a1e.notion.site/Mixture-of-Experts-MoE-11ac32470be28055bcc6cd4a78b26243) ([A Visual Guide to Mixture of Experts](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts)). Oct 2024.
  - [양자화에 관한 비주얼 가이드](https://tulip-phalange-a1e.notion.site/a947f0efb8eb4813a533b0d957134f6d) ([A Visual Guide to Quantization](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-quantization)). Jul 2024.
    - Sam Rose. [Quantization from the Ground Up](https://ngrok.com/blog/quantization). *ngrok blog*. Mar 2026. (이걸 먼저 읽으세요)
  - [A Visual Guide to DiffusionGemma](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-diffusiongemma). Jun 2026.
  - [맘바 및 상태 공간 모델에 대한 비주얼 가이드](https://tulip-phalange-a1e.notion.site/05f977226a0e44c6b35ed9bfe0076839) ([A Visual Guide to Mamba and State Space Models](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mamba-and-state)). Feb 2024.
- Sebastian Raschka. *[Machine Learning FAQs](https://sebastianraschka.com/faq/index.html)*

## Training
### How to Train LMs
- Kyongchun Cho. [You Want to Train Language Models Yourself from Scratch](https://drive.google.com/file/d/1ZOk79Q5PWi9u3erpufiejy5HdHd_ybYT/view). CHIL. 2024.
- Yann Dubois. [Introduction to Training LLMs](https://agenticai-learning.org/slides/lecture1.pdf). *CS294/194-196: Agentic AI*. UC Berkeley. Fall 2025.
- Kylo Lo, Akshita Bagia, & Nathan Lambert. [Language Modeling](https://natolambert.com/slides). NeurIPS. Dec 2024.
- Nathan Lambert. [The ML Foundations of LLM Post-Training](https://rlhfbook.com/course#prerequisites). Jun 2026.

### Post-training
- Nathan Lambert. [Building OLMo in the Era of Agents](https://natolambert.com/slides). Feb 2026.
  - [Frontier Post-Training Recipe Survey](https://rlhfbook.com/teach/course/conversation-01). Jun 2026.


## Advanced: Modern LM Systems
- Percy Liang & Tatsunori Hashimoto. *[CS336: Language Modeling from Scratch](https://cs336.stanford.edu)*. Stanford University. Spring 2026.
- Alisa Liu. [Alisa's Book of LLMs](https://alisawuffles.notion.site/alisa-s-book-of-llms). Jun 2026.

## Agents
### What Is an Agent?
- Ben Recht. [Secrets of Intelligence Services](https://www.argmin.net/p/secrets-of-intelligence-services). Feb 2026.
- Thomas Ptacek. [You Should Write an Agent](https://fly.io/blog/everyone-write-an-agent/). *fly.io blog*. Nov 2025.
- 오픈AI 개발자 문서. [Function Calling](https://developers.openai.com/api/docs/guides/function-calling). 
- 오픈AI 엔지니어링 블로그. [Codex 에이전트 루프 풀어보기](https://openai.com/ko-KR/index/unrolling-the-codex-agent-loop/). ([Unrolling the Codex Loop](https://openai.com/index/unrolling-the-codex-agent-loop/)). Jan 2026.
- 자손킴(jasonkim). [Claude API의 Request Body 분석](https://hackers.pub/@jasonkim/2025/claude-api-request-body). Dec 2025.
    - [Claude Code의 거의 모든 것은 Tool Use입니다. MCP도 subagent도 skills 역시요](https://hackers.pub/@jasonkim/2025/agent-tool-use). Dec 2025.
    - [Subagent는 Tool Use입니다](https://hackers.pub/@jasonkim/2025/subagent-is-tool-use). Dec 2025.
    - [MCP도 Tool Use를 사용합니다](https://hackers.pub/@jasonkim/2025/mcp-is-tool-use). Dec 2025.
- 클라우드플레어 블로그. [Glasswing 프로젝트: 저희가 Mythos를 통해 관찰한 내용](https://blog.cloudflare.com/ko-kr/cyber-frontier-models/) ([Project Glasswing: What Mythos Showed Us](https://blog.cloudflare.com/cyber-frontier-models/)). May 2026.

### Agentic Engineering
- Mario Zechner. [Prompts Are Code, .json/.md Files Are State](https://mariozechner.at/posts/2025-06-02-prompts-are-code/). Jun 2025.
- Nader Dabit. [You Could've Invented OpenClaw](https://gist.github.com/dabit3/bc60d3bea0b02927995cd9bf53c3db32). Feb 2026.

### Agent Security
- Simon Willison. [The Lethal Trifecta for AI Agents: Private data, Untrusted Content, and External Communication](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/). Jun 2025.
- 영미권 5개국 정보기관 합동 발간. *[Careful Adoption of Agentic AI Services](https://www.cyber.gov.au/business-government/secure-design/artificial-intelligence/careful-adoption-of-agentic-ai-services)*. May 2026.
- 엔비디아 기술 블로그. [Practical Security Guidance for Sandboxing Agentic Workflows and Managing Execution Risk](https://developer.nvidia.com/blog/practical-security-guidance-for-sandboxing-agentic-workflows-and-managing-execution-risk/). Jan 2026.
- Luis Cardoso. [A Field Guide to Sandboxes for AI](https://www.luiscardoso.dev/blog/sandboxes-for-ai). Jan 2026.
- 오픈AI. ["정렬 문제(Misalignment)"의 유형]([Types of Misalignment](https://github.com/kimmodal/AI-Learning-Resources/blob/57b4fc6223e2b5ea43ac214e0a2dc1e8bc6e47f5/misalignment.md)). 오픈AI 안전 블로그 [OpenAI가 내부 코딩 에이전트의 정렬 문제를 관찰하고 점검하는 방법](https://openai.com/ko-KR/index/how-we-monitor-internal-coding-agents-misalignment/) 발췌. ([How We Monitor Internal Coding Agents for Misalignment](https://openai.com/index/how-we-monitor-internal-coding-agents-misalignment/)). Mar 2026.

## AI "Safety"
### Overview
- Ben Recht. [The Banal Evil of AI Safety](https://www.argmin.net/p/the-banal-evil-of-ai-safety). Aug 2025.
- Peter Slattery et al. [Taxonomy of AI Risks](https://github.com/kimmodal/AI-Learning-Resources/blob/main/DomainTaxonomyofAIRisks.md). Adapted from *[AI Risk Repository](https://airisk.mit.edu/risks)*. Mar 2026.
- Yoshua Bengio et al. *[International AI Safety Report 2026](https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026)*. Feb 2026.

### "Alignment"
- Séb Krier. [Scary Model Cards and the Discourse Shifting](https://x.com/sebkrier/status/2020561261751062664). Feb 2026.
- Christopher Summerfield et al. [Lessons from a Chimp: AI ‘Scheming’ and the Quest for Ape Language](https://arxiv.org/pdf/2507.03409). Jul 2025.

## AI Writing Smells
- 뉴욕타임즈. [Why Does A.I. Write Like … That?](https://www.nytimes.com/2025/12/03/magazine/chatbot-writing-style.html). Dec 2025.
- 위키피디아. [Signs of AI Writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing). 
- Shiv Bosale. [Various LLM Smells](https://shvbsle.in/various-llm-smells/). May 2026.
- Sarah Perez. [OpenAI Says It’s Fixed ChatGPT’s Em dash Problem](https://techcrunch.com/2025/11/14/openai-says-its-fixed-chatgpts-em-dash-problem/). *TechCrunch*. Nov 2025.
- Shaina Mishkin. [It's Not Just a Trend, It's a Phenomenon](images/itsnot.webp). From [AI Is Changing How Companies Talk to Shareholders. Here Is the Red Flag for Readers](https://www.barrons.com/articles/ai-corporate-communications-shareholders-red-flag-63211618). *Barron's*. Apr 2026. 
- Nathan Lambert. [Why AI Writing is Mid](https://www.interconnects.ai/p/why-ai-writing-is-mid). Nov 2025.
- Lina Abushouk. [How to Read Postcolonial Writing](https://africasacountry.com/2026/05/how-to-read-postcolonial-writing). *Africa Is a Country*. May 2026.
