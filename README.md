# AI Learning Resources
Good AI learning resources I have found useful.<br>
I tried to list them in a suggested reading order.

**TODO**
- Add links for ToC
- Add brief annotations for each resource.
- Add a Korean version.

## Table of Contents
1. AI Engineering Overview
2. Architectures
   - Transformers
   - Further Topics
3. Training
4. Advanced: Modern Language Model Systems
5. Agents
   - What Is an Agent?
   - Agentic Engineering
   - Agent Security
6. AI "Safety"
   - Overview
   - "Alignment"
7. AI Writing Smells

## AI Engineering Overview
- Chip Huyen. *AI Engineering*. O'Reilly. 2024.

## Architectures
### Transformers
- Jay Alammar & Maarten Grootendorst. Ch 3: Inside Large Language Models. In *Hands-on Large Language Models*. O'Reilly. 2024. 
- 0xkato. [How LLMs Actually Work](https://www.0xkato.xyz/how-llms-actually-work/). Apr 2026.
- Lucas Beyer. [Transformer Tutorial](https://lucasb.eyer.be/transformer). Sep 2022.

### Further Topics
- Jay Alammar & Maarten Grootendorst. Ch 9: Multimodal Large Language Models. In *Hands-on Large Language Models*. O'Reilly. 2024. 
- Jay Alammar. [The Illustrated Stable Diffusion](https://jalammar.github.io/illustrated-stable-diffusion/). Oct 2022.
- Maarten Grootendorst. [A Visual Guide to Reasoning LLMs](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-reasoning-llms). Feb 2025.
  - [A Visual Guide to Mixture of Experts](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts). Oct 2024.
  - [A Visual Guide to Quantization](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-quantization). Jul 2024.
    - Sam Rose. [Quantization from the Ground Up](https://ngrok.com/blog/quantization). *ngrok blog*. Mar 2026. (read this before the article above)
  - [A Visual Guide to Mamba and State Space Models](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mamba-and-state). Feb 2024.
  - [A Visual Guide to DiffusionGemma](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-diffusiongemma). Jun 2026.
- Devi. [Beyond the Curve: A Holistic Guide to Activation Functions (from Sigmoid to SwiGLU)](https://ai.plainenglish.io/beyond-the-curve-a-holistic-guide-to-activation-functions-from-sigmoid-to-swiglu-3e96faaa7a84). *AI in Plain English*. Jan 2026.
- 자손킴(jasonkim). [Claude Code가 모델이 하지도 않은 말을 했다고 하는 이유](https://hackers.pub/@jasonkim/2025/claude-code-prefill). Dec 2025.
- Sebastian Raschka. *[Machine Learning FAQs](https://sebastianraschka.com/faq/index.html)*

## Training
- Kyongchun Cho. [You Want to Train Language Models Yourself from Scratch](https://drive.google.com/file/d/1ZOk79Q5PWi9u3erpufiejy5HdHd_ybYT/view). CHIL. 2024.
- Yann Dubois. [Introduction to Training LLMs](https://agenticai-learning.org/slides/lecture1.pdf). *CS294/194-196: Agentic AI*. UC Berkeley. Fall 2025.
- Nathan Lambert. [Building OLMo in the Era of Agents](https://natolambert.com/slides). Feb 2026.
  - [Frontier Post-Training Recipe Survey](https://rlhfbook.com/teach/course/conversation-01). Jun 2026.
- Kylo Lo, Akshita Bagia, & Nathan Lambert. [Language Modeling](https://natolambert.com/slides). NeurIPS. Dec 2024.

## Advanced: Modern Language Model Systems
- Tatsunori Hashimoto & Percy Liang. *[CS336: Language Modeling from Scratch](https://cs336.stanford.edu)*. Stanford University. Spring 2026.
- Alisa Liu. [Alisa's Book of LLMs](https://alisawuffles.notion.site/alisa-s-book-of-llms). Jun 2026.

## Agents
### What Is an Agent?
- Ben Recht. [Secrets of Intelligence Services](https://www.argmin.net/p/secrets-of-intelligence-services). Feb 2026.
- Thomas Ptacek. [You Should Write an Agent](https://fly.io/blog/everyone-write-an-agent/). *fly.io blog*. Nov 2025.
- Hugging Face. *[Agents Course](https://huggingface.co/learn/agents-course/unit1/introduction)*, Unit 1: Introduction. 2025.
- OpenAI. [Function Calling](https://developers.openai.com/api/docs/guides/function-calling). *OpenAI Developer Docs.*
- Michael Bolin. [Unrolling the Codex Loop](https://openai.com/index/unrolling-the-codex-agent-loop/). *OpenAI Engineering Blog*. Jan 2026.
- 자손킴(jasonkim). [Claude API의 Request Body 분석](https://hackers.pub/@jasonkim/2025/claude-api-request-body). Dec 2025.
    - [Claude Code의 거의 모든 것은 Tool Use입니다. MCP도 subagent도 skills 역시요](https://hackers.pub/@jasonkim/2025/agent-tool-use). Dec 2025.
    - [Subagent는 Tool Use입니다](https://hackers.pub/@jasonkim/2025/subagent-is-tool-use). Dec 2025.
    - [MCP도 Tool Use를 사용합니다](https://hackers.pub/@jasonkim/2025/mcp-is-tool-use). Dec 2025.
- Grant Bourzikas. [Project Glasswing: What Mythos Showed Us](https://blog.cloudflare.com/cyber-frontier-models/). *The Cloudflare Blog*. May 2026.

### Agentic Engineering
- Mario Zechner. [Prompts Are Code, .json/.md Files Are State](https://mariozechner.at/posts/2025-06-02-prompts-are-code/). Jun 2025.
- Nader Dabit. [You Could've Invented OpenClaw](https://gist.github.com/dabit3/bc60d3bea0b02927995cd9bf53c3db32). Feb 2026.

### Agent Security
- Simon Willison. [The Lethal Trifecta for AI Agents: Private data, Untrusted Content, and External Communication](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/). Jun 2025.
- ACSC, CISA, NSA, Cyber Center, NCSC NZ, & NCSC UK. *[Careful Adoption of Agentic AI Services](https://www.cyber.gov.au/business-government/secure-design/artificial-intelligence/careful-adoption-of-agentic-ai-services)*. May 2026.
- Rich Harang. [Practical Security Guidance for Sandboxing Agentic Workflows and Managing Execution Risk](https://developer.nvidia.com/blog/practical-security-guidance-for-sandboxing-agentic-workflows-and-managing-execution-risk/). *Nvidia Technical Blog*. Jan 2026.
- Luis Cardoso. [A Field Guide to Sandboxes for AI](https://www.luiscardoso.dev/blog/sandboxes-for-ai). Jan 2026.
- OpenAI. [Types of Misalignment](https://github.com/kimmodal/AI-Learning-Resources/blob/57b4fc6223e2b5ea43ac214e0a2dc1e8bc6e47f5/misalignment.md). Adapted from [How We Monitor Internal Coding Agents for Misalignment](https://openai.com/index/how-we-monitor-internal-coding-agents-misalignment/). *OpenAI Safety Blog*. May 2026.

## AI "Safety"
### Overview
- Ben Recht. [The Banal Evil of AI Safety](https://www.argmin.net/p/the-banal-evil-of-ai-safety). Aug 2025.
- Peter Slattery et al. [Taxonomy of AI Risks]([DomainTaxonomyofAIRisks.md](https://github.com/kimmodal/AI-Learning-Resources/blob/main/DomainTaxonomyofAIRisks.md). Adapted from *[AI Risk Repository](https://airisk.mit.edu/risks)*. Mar 2026.
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
- Nathan Lambert. [Why AI writing is Mid](https://www.interconnects.ai/p/why-ai-writing-is-mid). Nov 2025.
- Lina Abushouk. [How to Read Postcolonial Writing](https://africasacountry.com/2026/05/how-to-read-postcolonial-writing). *Africa Is a Country*. May 2026.
