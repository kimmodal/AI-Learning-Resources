# AI 학습 자료
마지막 업데이트: 2026년 7월 6일

제가 유용하다고 느낀 AI 학습 자료를, 대략 추천해서 읽으실 만한 순서대로 정리한 목록입니다.

#### 할 일
- 추론 최적화, 에이전트형 엔지니어링, AI의 인지적/사회적 영향, 신뢰할 수 있는 AI 등에 관한 자료를 추가합니다
- CME295와 CS336 사이 수준의 중급 강의를 추가합니다

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
  > 전체 AI 엔지니어링 스택을 훑기에 아주 좋은 개론서입니다. 이 목록에서 하나만 읽으신다면, 적어도 이 책은 읽어보시면 좋습니다. LLM 시스템, 평가, 데이터, RAG, 파인튜닝, 에이전트, 추론 최적화, 프롬프트 엔지니어링 등의 기본을 다룹니다. 

## Architectures
### Transformers
- Jay Alammar & Maarten Grootendorst. Ch 3: Inside Large Language Models, in *Hands-on Large Language Models*. O'Reilly. Sep 2024. 
  > 제이 알아마르 & 마르턴 흐루턴도르스트. *핸즈온 LLM*. 3장: 대규모 언어 모델 자세히 살펴보기. 한빛미디어.<br>
  > 알라마르의 [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) (2017)를 바탕으로 하지만, 더 좋고 훨씬 더 포괄적입니다. 

#### Optional: More on Transformers
- 0xkato. [How LLMs Actually Work](https://www.0xkato.xyz/how-llms-actually-work/). June 2026.
  > 트랜스포머에 대해 조금 더 다루며, 잔차 연결과 레이어 정규화도 포함합니다
- Lucas Bayer. [Transformer Tutorial](lucasb.eyer.be/transformer). Sep 2022.
  > 수학이 아주 조금 포함되어 있으며, 확률과 선형대수의 기본 지식을 전제로 합니다
- Devi's blog. [Beyond the Curve: A Holistic Guide to Activation Functions (From Sigmoid to SwiGLU)](https://ai.plainenglish.io/beyond-the-curve-a-holistic-guide-to-activation-functions-from-sigmoid-to-swiglu-3e96faaa7a84). Jan 2026.

### LLMs
- Jay Alammar & Maarten Grootendorst. Ch 9: Multimodal Large Language Models, in *Hands-on Large Language Models*. O'Reilly. Sep 2024.
  > 제이 알아마르 & 마르턴 흐루턴도르스트. *핸즈온 LLM*. 9장: 멀티모달 대규모 언어 모델. 한빛미디어.<br>
- Maarten Grootendorst. [A Visual Guide to Reasoning LLMs](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-reasoning-llms). Feb 2025.
  - [A Visual Guide to Mixture of Experts](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts). Oct 2024.
  - [A Visual Guide to Quantization](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-quantization). Jul 2024.
    - Sam Rose. [Quantization from the Ground Up](https://ngrok.com/blog/quantization). *ngrok blog*. Mar 2026.
      > 위 글을 읽기 전에 이것부터 읽어보세요
  - [A Visual Guide to Gemma 4](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-gemma-4). Apr 2026.
    > 2026년 초 모델 아키텍처를 잘 보여주는 스냅샷입니다: 멀티모달리티, MoE, GQA, 추론적 디코딩, MTP 등.
  - [A Visual Guide to DiffusionGemma](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-diffusiongemma). Jun 2026.
    > 확산 모델 입문으로도 좋습니다
  - [A Visual Guide to Mamba and State Space Models](https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mamba-and-state). Feb 2024.

## Training
### How to Train LMs
- Kyongchun Cho. [You Want to Train Language Models Yourself from Scratch](https://drive.google.com/file/d/1ZOk79Q5PWi9u3erpufiejy5HdHd_ybYT/view). CHIL. 2024.
  > AI 시스템의 모든 부분에서 훨씬 더 많은 투명성이 필요합니다: 데이터, 사전 학습, 사후 학습, 보호 장치, 배포, 모니터링, 버전 관리, 그리고 그 사이의 모든 것 
- Yann Dubois. [Introduction to Training LLMs](https://agenticai-learning.org/slides/lecture1.pdf). *CS294/194-196: Agentic AI*. UC Berkeley. Fall 2025.
  > LLM 학습이 처음이시라면 조금 어려울 수 있습니다. 그래도 전체 과정을 훑기에 좋은 개론입니다
- Nathan Lambert. [The ML Foundations of LLM Post-Training](https://rlhfbook.com/course#prerequisites). Jun 2026.
  > 수학이 조금 포함되어 있으며, ML, 확률, 선형대수의 기본 지식을 전제로 합니다<br>
  > 사후 학습을 따라가시려면 [Nathan Lambert](https://x.com/natolambert)를 꼭 팔로우해 보세요
- Kylo Lo, Akshita Bagia, & Nathan Lambert. [Language Modeling](https://natolambert.com/slides). NeurIPS. Dec 2024.

### Post-training
- Nathan Lambert. [Building Language Models in the Era of Agents](https://natolambert.com/slides). Feb 2026.
  - [Frontier Post-Training Recipe Survey](https://rlhfbook.com/teach/course/conversation-01). Jun 2026.

## Inference Optimization
> 작성 중입니다

## Advanced: Modern LM Systems
- Sebastian Raschka. *[Machine Learning FAQs](https://sebastianraschka.com/faq/index.html)*
  > 질문 목록이 좋고, 읽어보시면 배울 것이 많습니다
- Afshine Amidi & Shervine Amidi. *[CME295: Transformer & Large Language Models](https://cme295.stanford.edu)*. Stanford University. Fall 2025.
  > ML, 확률, 선형대수의 기본 지식을 전제로 합니다
- Percy Liang & Tatsunori Hashimoto. *[CS336: Language Modeling from Scratch](https://cs336.stanford.edu)*. Stanford University. Spring 2026.
  > ML, 확률, 선형대수, 트랜스포머/LLM의 기본 지식을 전제로 합니다. 과제가 이 강의의 핵심이지만 시간이 많이 듭니다. 자료만 훑어보셔도 여전히 충분히 가치 있습니다
- Alisa Liu. [Alisa's Book of LLMs](https://alisawuffles.notion.site/alisa-s-book-of-llms). Jun 2026.
  > CS336 수준의 좋은 요약입니다

## Agents
### What Is an Agent?
- Ben Recht. [Secrets of Intelligence Services](https://www.argmin.net/p/secrets-of-intelligence-services). Feb 2026.
- Thomas Ptacek. [You Should Write an Agent](https://fly.io/blog/everyone-write-an-agent/). *fly.io blog*. Nov 2025.
  > 에이전트의 "마법"이 어떻게 보이는지 보여줍니다
- Grant Bourzikas. [Project Glasswing: What Mythos Showed Us](https://blog.cloudflare.com/cyber-frontier-models/). *The Cloudflare Blog*. May 2026.
  > 일부러 [Agent Security](#agent-security)가 아니라 여기에 둡니다

#### Optional: Mechanics of an Agent
> 에이전트가 실제로 어떻게 작동하는지 더 자세히 보고 싶으시다면
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
  > Pi를 만든 사람이 지금의 "루프 엔지니어링" 흐름을 일찍 짚었습니다
- Nader Dabit. [You Could've Invented OpenClaw](https://gist.github.com/dabit3/bc60d3bea0b02927995cd9bf53c3db32). Feb 2026.
  > OpenClaw가 어떻게 작동하는지 설명합니다

### Agent Security
- Simon Willison. [The Lethal Trifecta for AI Agents: Private data, Untrusted Content, and External Communication](https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/). Jun 2025.
  > 윌리슨 본인이 말하듯, "치명적 삼중 조합"은 기억에 잘 남는 표현이고 좋은 프레임워크이기도 합니다
- ACSC, CISA, NSA, Cyber Center, NCSC NZ, & NCSC UK. *[Careful Adoption of Agentic AI Services](https://www.cyber.gov.au/business-government/secure-design/artificial-intelligence/careful-adoption-of-agentic-ai-services)*. May 2026.
  > 실제 시스템에서 AI 에이전트를 구현하시는 분이라면 필독해야 할 글입니다
- Rich Harang. [Practical Security Guidance for Sandboxing Agentic Workflows and Managing Execution Risk](https://developer.nvidia.com/blog/practical-security-guidance-for-sandboxing-agentic-workflows-and-managing-execution-risk/). *NVIDIA Technical Blog*. Jan 2026.
  > 이 역시 실제 시스템에서 AI 에이전트를 구현하시는 분이라면 필독해야 할 글입니다
  - David Dworken & Oliver Weller-Davie. [Beyond permission prompts: making Claude Code more secure and autonomous](https://www.anthropic.com/engineering/claude-code-sandboxing). *Engineering at Anthropic*. Oct 2025.
    > "**효과적인 샌드박싱에는 파일시스템 격리와 네트워크 격리가 모두 필요합니다.** 이 점에 주목해야 합니다. 네트워크 격리가 없으면 침해된 에이전트가 SSH 키 같은 민감한 파일을 외부로 유출할 수 있고, 파일시스템 격리가 없으면 침해된 에이전트가 샌드박스를 쉽게 벗어나 네트워크 접근 권한을 얻을 수 있습니다."
  - Luis Cardoso. [A Field Guide to Sandboxes for AI](https://www.luiscardoso.dev/blog/sandboxes-for-ai). Jan 2026.
    > 컨테이너, gVisor, 마이크로VM, WASM/아이솔레이트에 대한 탄탄한 입문서입니다<br>
    > > "컨테이너는 적대적 코드에 충분한 보안 경계가 아닙니다. ... 여전히 호스트 커널을 공유하기 때문입니다."
  - [Sandboxing Agents with AI Workbench](https://docs.nvidia.com/ai-workbench/user-guide/latest/concepts/sandboxing-concept.html). *NVIDIA AI Workbench User Guide*
    > "샌드박싱이 다루지 않는 내용입니다
    > - 컨테이너 안의 프로세스 샌드박스는 환경 변수를 격리하지 않습니다.
    > - 일부 에이전트 샌드박스는 컨테이너 안에서 조용히 실패합니다.
    > - **에이전트 지침은 실제로 아무것도 강제하지 않으므로, 반드시 권한과 훅을 사용해야 합니다.** <br>
    >   MDC 규칙, skills, CLAUDE.md 파일은 에이전트에게 제약과 관례를 알려주지만, **에이전트는 그것들을 무시할 수 있습니다.**"
- Marcus Williamson et al. [Types of Misalignment](misalignment.md). Adapted from [How We Monitor Internal Coding Agents for Misalignment](https://openai.com/index/how-we-monitor-internal-coding-agents-misalignment/). *OpenAI Safety Blog*. May 2026.
  > 에이전트가 의도대로 작동하지 않을 수 있는 방식들입니다

## AI "Safety"
### Overview
- Ben Recht. [The Banal Evil of AI Safety](https://www.argmin.net/p/the-banal-evil-of-ai-safety). Aug 2025.
  > 모든 AI "안전성" 연구자가 읽어야 할 글입니다
- Peter Slattery et al. [Taxonomy of AI Risks](DomainTaxonomyofAIRisks.md). Adapted from [The AI risk repository: A meta-review, database, and taxonomy of risks from artificial intelligence](https://airisk.mit.edu/risks). Mar 2026.
  > 좋은 프레임워크입니다
- Yoshua Bengio et al. *[International AI Safety Report 2026](https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026)*. Feb 2026.
  > 좋은 참고 자료입니다

### "Alignment"
- Séb Krier. [Scary Model Cards and the Discourse Shifting](https://x.com/sebkrier/status/2020561261751062664). Feb 2026.
  > "일부 평가를 공개적으로 해석하는 많은 방식은 채팅 출력을 모델에 내재한 속성의 직접적인 증거로 암묵적으로 취급하지만, LLM의 행동은 역할과 맥락에 강하게 조건화되는 경우가 많습니다. 그 결과 논평자들은 때때로 모델이 실제로 무엇을 하고 있는지(텍스트 맥락에 따라 역할을 시뮬레이션하는 것)를 놓치고, 테스트를 지나치게 양식화하며(시나리오를 모델에게 심리적으로 그럴듯하게 만들려는 노력을 하지 않기 때문에), 결과를 기저 메커니즘(마음 이론 같은 추론을 통한 텍스트 예측)과 맞지 않는 프레임워크(목표 지향적 합리적 행위자성)로 해석합니다. <br>
  > 1. 모델은 질문에 답하는 것이 아니라 텍스트를 완성하고 있습니다 
  > 2. 어시스턴트 페르소나는 모델 자체가 아니라 허구의 인물입니다 
  > 3. 겉보기 오류는 프롬프트가 암시한 세계에 대한 올바른 완성인 경우가 많습니다
  > 4. “평가 인식”은 신비로운 것이 아닙니다: 모델은 강한 독자이기 때문에 인위성을 알아차릴 수 있습니다
  > 5. 사후 학습은 대체로 행동을 좁히거나 재형성하며, 도움이 될 수도 있지만 왜곡할 수도 있습니다."
- Christopher Summerfield et al. [Lessons from a Chimp: AI ‘Scheming’ and the Quest for Ape Language](https://arxiv.org/pdf/2507.03409). Jul 2025.
  > "1. 많은 주장이 일화적 증거에 기대고 있습니다  
  > 2. 연구가 가설과 통제 조건을 갖추지 못한 경우가 많습니다  
  > 3. 이론적 동기가 약하거나 불분명한 경우가 많습니다  
  > 4. 발견이 과장되거나 정당화하기 어려운 방식으로 해석되는 경우가 많습니다"

## AI Writing Smells
- Sam Kriss. [Why Does A.I. Write Like … That?](https://www.nytimes.com/2025/12/03/magazine/chatbot-writing-style.html). *The New York Times*. Dec 2025.
  - Wikipedia. [Signs of AI Writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).
  - Shiv Bosale. [Various LLM Smells](https://shvbsle.in/various-llm-smells/). May 2026.
  - Sarah Perez. [OpenAI Says It’s Fixed ChatGPT’s Em dash Problem](https://techcrunch.com/2025/11/14/openai-says-its-fixed-chatgpts-em-dash-problem/). *TechCrunch*. Nov 2025.
  - Shaina Mishkin. [It's Not Just a Trend, It's a Phenomenon](images/itsnot.webp). From [AI Is Changing How Companies Talk to Shareholders. Here Is the Red Flag for Readers](https://www.barrons.com/articles/ai-corporate-communications-shareholders-red-flag-63211618). *Barron's*. Apr 2026.
- Nathan Lambert. [Why AI Writing is Mid](https://www.interconnects.ai/p/why-ai-writing-is-mid). Nov 2025.
- Lina Abushouk. [How to Read Postcolonial Writing](https://africasacountry.com/2026/05/how-to-read-postcolonial-writing). *Africa Is a Country*. May 2026.
