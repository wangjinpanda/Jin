# Enterprise AI transformation: stages, staff levels, knowledge layer and readiness

Research notes for Jin Wang. Date: 1 Nov 2026.
Scope: rebuild the framework you saw online (individual transformation, then organization transformation, with L0/L1/L2 staff levels), check RAG / GraphRAG / knowledge graph / ontology, define readiness pillars, and list AI transformation consultancies in Singapore and China.

---

## 1. Answer first

**I could not find the exact article or video you saw.** No public source I found combines all 3 things you remember (2 parts x 2 stages, L0/L1/L2 staff levels, and "AI self-evolution" as the last stage). But 6 public sources each cover part of it, and together they support the structure below.

The governing message for your company:

1. **AI transformation runs in 2 parts and 4 stages.** Part A is individual transformation (Stage 1 Individual, Stage 2 Team). Part B is organization transformation (Stage 3 Organization, Stage 4 AI self-evolution).
2. **Most companies stall between Stage 2 and Stage 3.** At that point the bottleneck moves from staff skills to organization fit: approvals, KPIs, department borders, and data that agents cannot act on.
3. **Each stage needs a different staff level and a different knowledge layer.** L0 users and plain RAG are enough for Stages 1 and 2. Stages 3 and 4 need L2 / FDE-type people and an ontology of your key business objects.
4. **Use it as a diagnostic.** Score 4 stages against 6 readiness pillars (strategy, talent, culture, data, infrastructure, governance). The weakest pillar sets your real stage.

The rest of this note gives the evidence for each point, a stress test, and a step-by-step action plan.

---

## 2. Where the framework comes from (closest sources found)

| # | Source | What matches your memory | What differs |
|---|---|---|---|
| 1 | CSDN article, "个人-团队-组织三层九阶段实施框架" | Bottom-up path: 个人AI化 -> 团队AI化 -> 组织AI化. Individual layer starts with 自主学习 and 散点应用 | 3 layers and 9 stages. No self-evolution stage |
| 2 | Tencent Research Institute (腾讯研究院), "从超级个体到超级团队" (2026) | Path 个体觉醒 -> 能力溢出 -> 团队涌现 -> 组织启示. Formula: 组织竞争力 = 人才密度 x AI杠杆 ÷ 组织摩擦 | Describes how teams emerge. No maturity levels |
| 3 | Tencent Research Institute, "FDE模式行业观察与实践" (Aug 2026) | 3 stages: 个人提效, 组织转型, 业务重构. FDE as the delivery model. Business knowledge captured as 本体 (ontology) | 3 stages, not 4 |
| 4 | ANO Lab live session, reported by Huxiu: "一次组织重写正在发生：从FDE到本体" | 组织级AI生产力 ≈ 个体AI能力 x 组织AI适配度. FDE and ontology as the 2 entry points for organization change | No staff levels |
| 5 | NetEase article "突破效率桎梏，系统性构建 Agentic 组织" | L1-L5 organization levels. L5 is 自主进化: the organization sets sub-goals, adjusts processes and creates new agent roles. Says most enterprises sit between L1 and L2 | Levels describe the organization, not staff |
| 6 | Microsoft Work Trend Index 2025, "Frontier Firm" | 3 phases: Human with assistant -> Human-agent teams -> Human-led, agent-operated. New "agent boss" role | Microsoft says firms can be in more than 1 phase at once |

On "the last stage is about AI evaluating itself": the Chinese term is most likely **自进化 / 自主进化 (self-evolution)**. In practice it means agents check their own results against goals and propose improvements, while humans keep direction and control. One technical review lists 4 checks for this capability: can experience be saved as a reusable asset, can the system propose improvements by itself, is there a verifier that filters those improvements, and is there versioning and rollback.

**Verification limit.** Huxiu, Zhihu, 53AI and Agilean pages could not be opened directly from this session, so facts from those sites come from search-result summaries. Open the original page before you quote any number on a slide.

---

## 3. The 4-stage framework (reconstructed)

| Part | Stage | What it looks like | Main bottleneck | Microsoft Frontier Firm phase (my mapping) |
|---|---|---|---|---|
| A. Individual transformation | **1. Individual** | Staff use AI every day for their own tasks: drafting, summarising, analysis | Skills and habits. "放羊式全员AI": licences handed out with no guidance (Zhang Peng, GeekPark, Jul 2026) | Phase 1, Human with assistant |
| A. Individual transformation | **2. Team** | Teams share prompts, agents and flows. AI is part of the team's way of working | No shared knowledge base, no standards, good ideas stay with 1 person | Phase 2, Human-agent teams |
| B. Organization transformation | **3. Organization** | Cross-function processes are redesigned around agents. Decision rights and handoffs change | Organization fit: approvals, KPIs, department borders. Data that agents cannot act on | Phase 2 to 3 |
| B. Organization transformation | **4. AI self-evolution** | Agents run whole processes, measure outcomes and propose improvements. Humans set direction and approve changes | Evaluation, audit, rollback, accountability | Phase 3, Human-led, agent-operated |

Why Stage 2 to 3 is the hard step: the ANO Lab session reports cases where individuals became much faster with AI but company output did not improve, because processes, approvals and performance reviews stayed the same. Deloitte research, as cited by Worklytics, says organizations that redesign work are 2 times more likely to beat their expected AI ROI. Both are secondary sources, so treat the direction as reliable and the exact figures as unverified.

---

## 4. Staff levels L0, L1, L2

No source I found uses exactly L0 / L1 / L2 with FDE as the top level. The definitions below are **my proposal**, built to match what you remember and the closest public models.

| Level | Name | Who | Can do | Microsoft 365 tools | Needed from stage |
|---|---|---|---|---|---|
| **L0** | AI user | All knowledge workers | Uses AI freely and safely in daily work. Knows what data must not go into prompts | Copilot Chat, Microsoft 365 Copilot in Word, Excel, Outlook, Teams | Stage 1 |
| **L1** | AI builder / champion | 1 or more per team | Builds and shares simple agents and flows for the team. Maintains team knowledge sources | Agent Builder in Microsoft 365 Copilot, Copilot Studio, Power Automate, SharePoint | Stage 2 |
| **L2** | AI engineer / FDE | Small central group, placed inside business functions | Maps the process and business objects, connects systems, builds multi-agent workflows, sets evaluations and guardrails, moves pilots to production | Copilot Studio, Power Platform, Dataverse, Microsoft Fabric, Azure AI Foundry, APIs | Stages 3 and 4 |

Public models that support this design:

- **Zapier AI fluency rubric.** 4 levels: Unacceptable, Capable, Adoptive, Transformative. V2 (31 Mar 2026) scores mindset, strategy, building and accountability. "Capable" is the minimum hiring bar. For current staff it is not pass/fail: people pick the level they work at most of the time and aim 1 level up.
- **Wuhan East Lake High-tech Zone (东湖高新区) training.** 3 classes: basic for all staff with no coding, intermediate for business and tech key staff using real business cases, advanced to develop the company's own CAIO.
- **Lean-FDE certification (China).** L0 to L6 path. L1 AI Coding Builder, L2 Field Researcher, L3 Agent Engineer. Each level is judged on a portfolio of real work.
- **A practitioner blog** argues the goal for teams is "L2, not L4": everyone should reach a solid middle level rather than chasing the top level. Its L-scale is different from yours, but the logic fits: L0 for everyone, L1 widely, L2 for a few.

### What FDE means

FDE = Forward Deployed Engineer. The model started at Palantir: engineers sit with the customer or business unit and build until the solution works in real operations.

- Tencent Research Institute describes FDE as a delivery model that combines presales, implementation, product and customer success in 1 front-line team. The test that separates FDE from on-site outsourcing is whether knowledge is captured and reused after the project.
- Mininglamp (明略科技, 2718.HK) says about 30% of its delivery staff moved into FDE roles. This is a company statement.
- Counter-view: Andrew Ng is reported as saying FDE is valuable but will not become the main form of AI employment, partly because most companies prefer to use their own employees.

For an enterprise this means L2 can be built internally (business analysts, product owners and tech support staff retrained over months), bought from partners, or mixed.

---

## 5. Knowledge layer: RAG, GraphRAG, knowledge graph, ontology

### 5.1 Plain definitions

| Term | What it is | Good for | Limit |
|---|---|---|---|
| **RAG** (retrieval-augmented generation) | Search for relevant text chunks, give them to the LLM, and the LLM answers from them | "Find the answer in our documents" | Weak on questions that need the whole document set, relationships or business rules |
| **GraphRAG** | LLM extracts entities and relationships from documents into a graph, groups them into communities, writes summaries, and answers from those summaries | Broad questions across a large document set ("What are the main themes in 3 years of audit findings?") | Indexing cost. Plain vector RAG still gives more direct answers to specific questions |
| **Knowledge graph** | The actual data network: nodes (entities) and edges (relationships). Example: Customer A - ordered - Product B - made at - Plant C | Following relationships, impact analysis, root cause | Needs a schema and upkeep, or it drifts |
| **Ontology** | The schema behind the graph: what types of business objects exist, their properties, relationships, rules, and (in Palantir's model) the actions allowed on them | Letting agents act safely on business objects, with rules and permissions | Heavy design work. Needs business owners to agree on definitions |

A simple way to remember the order (from a Chinese technical blog): data cleaning makes data usable, ontology gives it meaning, and the knowledge graph makes that meaning usable for reasoning. Ontology is the schema. The knowledge graph is the filled-in instance.

### 5.2 Key facts checked

- **GraphRAG** comes from Microsoft Research (Edge et al., "From Local to Global: A Graph RAG Approach to Query-Focused Summarization", arXiv 2404.16130). It uses Leiden community detection and map-reduce answering over community summaries. On corpora of about 1 million tokens it beat plain RAG on comprehensiveness and diversity for broad questions. Plain vector RAG scored highest on directness. Testing covered 2 corpora only. Code is open source at github.com/microsoft/graphrag.
- **Palantir Ontology** models objects, links and properties, plus actions and the logic behind them, under security rules. Palantir's own docs say it is more than a thin "semantic layer". It is bundled with the Foundry platform.
- **Microsoft Fabric IQ** (announced at Ignite 2025) includes an Ontology item that maps business concepts to entity types, relationships and rules. It can be generated from existing Power BI semantic models. **The Ontology item is in preview**, so do not plan production use on it yet.
- **Microsoft's 3 "IQ" layers**: Work IQ (Microsoft 365 content), Fabric IQ (business data), Foundry IQ (knowledge and agentic retrieval for custom agents).
- **Copilot Studio knowledge sources** (Microsoft Learn): SharePoint uses Graph search with a limit of 4 URLs per source. Dataverse uses RAG, with up to 2 sources and 15 tables each. With user authentication, the agent only shows content that the asking user already has access to.
- **China**: a secondary source reports a national standard on ontology modelling, GB/T 48000.3, effective 1 Aug 2026. I could not find the standard text, so check the official standards platform before citing it.

### 5.3 Why it matters for agents

- Stages 1 and 2 can run on RAG over SharePoint and Teams content. The main work is cleaning permissions and curating content.
- Stages 3 and 4 need agents that change records, route approvals and trigger actions. For that, agents need to know what an "order", "supplier" or "deviation" is, who owns it, who may change it, and what the exceptions are. The ANO Lab session makes the same point: building an ontology forces the company to answer who is responsible, who decides and what the exception conditions are.

| Need | Technique | Microsoft option | Stage |
|---|---|---|---|
| Answer from policies and documents | RAG | Microsoft 365 Copilot, Copilot Studio with SharePoint knowledge | 1-2 |
| Answer from structured business data | RAG over tables | Copilot Studio with Dataverse knowledge | 2-3 |
| Broad questions across large document sets | GraphRAG | Azure AI Foundry with open-source GraphRAG | 3 |
| Agents that act on business objects with rules | Ontology + knowledge graph | Fabric IQ Ontology (preview), Dataverse data model | 3-4 |

---

## 6. Readiness pillars and diagnostic matrix

The best-documented readiness model is the **Cisco AI Readiness Index**: 6 pillars (strategy, infrastructure, data, governance, talent, culture) measured by 49 indicators. The 2025 edition surveyed 8,161 business and IT leaders in 30 markets and rated 13% of companies as "Pacesetters". Your "individual ready, infra ready, data ready" fit inside these 6 pillars (individual = talent + culture).

The matrix below combines the 6 pillars with the 4 stages. Each cell is what "ready" means at that stage. This is my synthesis, not a published standard.

| Pillar | Stage 1 Individual | Stage 2 Team | Stage 3 Organization | Stage 4 AI self-evolution |
|---|---|---|---|---|
| **Strategy** | Top management sponsor, AI use policy | Use-case backlog per team | Process-level business cases with named owners | Outcome targets for agent-run processes |
| **Talent** | L0 training for all staff | L1 champion in each team | L2 / FDE placed in key functions | Agent operations roles (agent ops, skill engineer, AI governance) |
| **Culture** | Safe to try, no blame for early mistakes | Sharing agents and prompts is recognised | KPIs and approval rules updated for AI work | Managers act as "agent boss" |
| **Data** | Sensitivity labels, oversharing cleaned up | Curated team knowledge in SharePoint | Master data and ontology for key business objects | Feedback data and test sets for evaluation |
| **Infrastructure** | Copilot Chat / Microsoft 365 Copilot licences | Copilot Studio environments, Power Platform DLP policies | Connectors and APIs to ERP and CRM, Fabric | Agent monitoring, versioning, rollback |
| **Governance** | Acceptable use rules, Microsoft Purview | Agent sharing approval, environment strategy | Decision rights, human-in-the-loop points | Evaluation, audit trail, external testing (e.g. AI Verify in Singapore) |

How to score: rate each cell 0 to 3 with evidence (usage data, survey, document check). Take the **weakest pillar** as your real stage. Tencent Cloud's AI Coding maturity model uses the same rule: the level is set by the weakest capability line.

---

## 7. AI transformation consultancies and programmes

Many rankings in this market are written or paid for by vendors. The tables only list what a cited source states, with the source type noted.

### 7.1 Singapore

| Organisation | What was found | Source type |
|---|---|---|
| **IMDA Digital Leaders Accelerator Bootcamp (AI Bootcamp)** | Launched Mar 2026. Run with **BCG** and **EY-Parthenon**. EY-Parthenon ran the first run | IMDA press release |
| **IMDA GenAI x Digital Leaders** | Funding plus tech partners. Listed partners include Axrail.ai, iNextLabs, IntentAI (list as of 6 Feb 2026). A vendor page says up to 50% funding | IMDA partner list, vendor page |
| **Microsoft AI QuickStart** | Launched 6 Feb 2026 with IMDA and UOB. For digitally mature SMEs and large non-ICT firms. Delivered by Microsoft partners (aka.ms/AIQuickStart). **Most relevant to an M365 / Copilot Studio stack** | Microsoft press release |
| **Databricks + EDB Enterprise AI Transformation programme** | Announced 16 Sep 2026. Participating companies get a Databricks-sponsored FDE. Databricks plans to invest more than US$350M in Singapore over 3 years | Databricks and EDB releases |
| **NCS** (Singtel group) | AI Central unit uses a forward-deployed engineering model to move projects from POC to production | Job listing and aggregator |
| **NTT DATA** (Japanese) | Smart AI Agent services: consulting, platforms, integration, managed services. Global offering, Singapore details not confirmed | NTT DATA press release |
| **Accenture, Thoughtworks, Zühlke, PALO IT** | Listed as global consultancies with local Singapore teams | Aggregator list |
| **AI Singapore 100 Experiments (100E)** | Co-investment programme that matches companies with university AI researchers | AI Singapore / PDPC |
| **AI Verify Foundation** | Governance testing toolkit, useful for Stage 4 controls. IMDA says it now covers both traditional and generative AI | IMDA |

### 7.2 China

| Organisation | What was found | Source type |
|---|---|---|
| **Alibaba Cloud (阿里云)** | Launched a public-cloud partner FDE system at Apsara Conference, 22 Sep 2026, and signed the first certified FDE service partners | Media report |
| **Mininglamp (明略科技, 2718.HK)** | FDE model, knowledge graph background, Octo platform. Reports agentic service revenue up 605.7% in H1 2026 | Company results (self-reported) |
| **Tezign (特赞)** | "AI FullStack" AI-native consulting. 3 layers: GEA agent infrastructure, business solutions, ABC+ organization programme. Gartner Cool Vendor 2024 | Company site, Gartner |
| **Tencent Research Institute (腾讯研究院)** | Publishes the FDE and "super individual to super team" reports. Research body, no consulting service found | Reports |
| **360** | Launched an AI transformation consulting service in Jun 2026 with a security focus | Media report |
| **传世智慧** | Ranked top in several Chinese lists for manufacturing AI transformation, TransClaw platform (2026) | Self-promotional rankings, verify first |
| **Accenture, Deloitte, EY, PwC, KPMG** | Active in China. Accenture names FDE as a core role globally. KPMG signed a global alliance with Anthropic | Industry articles |

Not found: I found no 2026 source on China-specific AI transformation work by McKinsey (QuantumBlack), BCG X, NRI or NTT DATA China. That does not mean they are inactive. Ask them directly for China case references.

---

## 8. Stress test

Points that could weaken this framework if you present it internally:

1. **Source risk.** The exact framework you remember is unverified. Present it as your company's own framework, built from cited public sources. Avoid calling it an "industry standard".
2. **Stages are not a straight line.** Microsoft says firms often sit in more than 1 phase at once. Expect Finance at Stage 3 while Sales is still at Stage 1. Score each function and region separately.
3. **L2 / FDE supply.** People who understand both the business and the tech are scarce in every market (Alibaba Cloud names this as 1 of 3 main pain points). Plan a build-buy mix and budget time for internal retraining.
4. **Ontology effort.** Ontology work is heavy and political because business units must agree on definitions. Fabric IQ Ontology is still in preview. Palantir requires Foundry adoption. Start with a small set of business objects in 1 process.
5. **Data exposure.** Microsoft 365 Copilot and Copilot Studio respect existing permissions. If SharePoint and Teams permissions are too open, Copilot will surface content people should not see. Fix oversharing before Stage 1 scale-up.
6. **China operations.** Microsoft 365 in mainland China is operated by 21Vianet, and Microsoft says some features are not enabled there. I could not confirm current Microsoft 365 Copilot availability on 21Vianet. **Check with your Microsoft or 21Vianet account team before including China in the rollout plan**, and check cross-border data rules with Legal.
7. **Stage 4 governance.** Agents that change their own processes need evaluation sets, approval gates, audit trails and rollback. Without these, Stage 4 creates control and audit findings.
8. **HQ alignment.** In a Japanese-affiliated group, organization changes in Stage 3 (KPIs, approval routes, decision rights) usually need HQ consensus. Start the conversation with HQ early, or Stage 3 will stall even if regions are ready.
9. **Value proof.** Usage counts will not convince top management for long. Define outcome metrics (time saved per process, error rate, cycle time) from Stage 2 onward, and collect a baseline before each pilot starts.

---

## 9. Action plan

| Step | Action | Output | Owner |
|---|---|---|---|
| 1 | Confirm the original source if possible (ask whoever shared the video, check the platform history) | Final naming of stages and levels | You |
| 2 | Adapt the 4-stage, L0/L1/L2 and 6-pillar model as your own framework. Keep the sources in an appendix | 1-page framework | You + AI CoE |
| 3 | Run a baseline: Copilot usage data, staff self-assessment on L0/L1/L2, document check per pillar | Scored 4 x 6 matrix per region and function | AI CoE + HR |
| 4 | Fix Stage 1 blockers: oversharing clean-up, sensitivity labels, acceptable use policy, L0 training | Stage 1 ready in [regions] | IT security + HR |
| 5 | Pick [number] pilot teams for Stage 2 and name an L1 champion in each | Shared team agents with usage and outcome data | Business heads |
| 6 | Pick 1 cross-function process for Stage 3. Define the key business objects, owners, decision rights and exceptions (first ontology) | Process redesign + ontology draft | L2 / FDE + process owner |
| 7 | Decide the L2 / FDE model: internal retraining, partner, or mix. In Singapore check Microsoft AI QuickStart and IMDA programmes. In China check Alibaba Cloud certified FDE partners and confirm Copilot availability | Sourcing decision and budget | You + Procurement |
| 8 | Set agent governance: environment strategy, sharing approval, evaluation sets, audit and rollback | Agent lifecycle standard | IT governance |
| 9 | Re-score the matrix every quarter and report outcome metrics to top management | Quarterly AI readiness report | AI CoE |

---

## Sources

Framework and stages
- [CSDN: 个人-团队-组织三层九阶段实施框架](https://blog.csdn.net/weixin_72959097/article/details/154080611)
- [腾讯研究院: 从超级个体到超级团队 (summary, Sohu)](https://www.sohu.com/a/1032477828_121503203)
- [腾讯云开发者社区: 超级个体不是终点，超级团队才是 AI 组织的分水岭](https://developer.cloud.tencent.com/article/2695173)
- [36Kr: 前线共创，双向赋能：FDE 模式行业观察与实践报告](https://www.36kr.com/p/3926404419910018)
- [Huxiu: 一次组织重写正在发生：从FDE到本体](https://www.huxiu.com/article/4891472.html)
- [NetEase: 突破效率桎梏，系统性构建 Agentic 组织](https://www.163.com/dy/article/L80QKHS205118O92.html)
- [GeekPark: 给「AI 组织」交了好几波学费后，终于看清了这五级台阶](https://www.geekpark.net/news/367345)
- [Huxiu: AI原生组织搭建：从三次实践到四层爬坡](https://www.huxiu.com/article/4867608.html)
- [cnblogs: RSI综述 Self-Evolving Agents](https://www.cnblogs.com/sddai/p/22302741)
- [Microsoft WorkLab: The CEO guide to building a Frontier Firm](https://www.microsoft.com/en-us/worklab/the-ceo-guide-to-building-a-frontier-firm)
- [Petri: Microsoft 2025 Work Trend Index](https://petri.com/microsoft-2025-work-trend-index-ai-agents/)
- [Worklytics: AI workflow redesign](https://www.worklytics.co/blog/ai-workflow-redesign)
- [Tencent Cloud: 企业级AI Coding成熟度模型](https://cloud.tencent.com/developer/article/2666317)

Staff levels and FDE
- [Zapier: AI fluency rubric](https://zapier.com/blog/ai-fluency-rubric/)
- [Disco: Zapier's 4-tier AI fluency framework](https://www.disco.co/blog/zapiers-4-tier-ai-fluency-framework-a-playbook-for-hr-and-people-leaders)
- [Blog: The AI fluency goal for teams is L2, not L4](https://anirudhwarrier.bearblog.dev/the-ai-fluency-goal-for-teams-is-l2-not-l4/)
- [Lean-FDE certification](https://www.leanfde.com/fde/certification)
- [21jingji: AI落地催生FDE人才刚需，地方培训加速布局](https://m.21jingji.com/article/20260917/herald/26f023e22b984c9a6e27e6203c4d67a9.html)
- [NetEase: 明略科技如何用三年时间把FDE从概念变成组织能力](https://www.163.com/dy/article/L71UUVLJ0534A4SC.html)
- [Caixin Global: China's AI boom creates demand for a new kind of engineer](https://www.caixinglobal.com/2026-07-16/in-depth-chinas-ai-boom-creates-demand-for-a-new-kind-of-engineer-102464555.html)

Knowledge layer
- [arXiv 2404.16130: From Local to Global, a GraphRAG approach](https://arxiv.org/html/2404.16130v2)
- [Microsoft Research: GraphRAG paper page](https://www.microsoft.com/en-us/research/?p=1029069)
- [Palantir docs: The Ontology system](https://palantir.com/docs/foundry/architecture-center/ontology-system/)
- [Palantir docs: Why create an Ontology](https://www.palantir.com/docs/foundry/ontology/why-ontology)
- [Info-Tech: Microsoft adopts ontology-based IQ layer for agentic AI](https://www.infotech.com/research/microsoft-adopts-ontology-based-iq-layer-for-agentic-ai)
- [Atlan: What is Fabric IQ](https://atlan.com/know/microsoft-fabric/what-is-fabric-iq.md)
- [Microsoft Learn: Knowledge in Copilot Studio](https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-copilot-studio)
- [DA技术分享: FDE、本体建模与AI落地](https://www.darkathena.top/archives/fde-ontology-ai-delivery)
- [BestHub: GB/T 48000.3 three shifts for enterprise knowledge modeling](https://www.besthub.dev/articles/gb-t-48000-3-three-shifts-for-enterprise-knowledge-modeling-from-documents-to-actionable-ontologies-1487918cdc24)

Readiness
- [Cisco AI Readiness Index methodology](https://www.cisco.com/c/m/en_us/solutions/ai/readiness-index/methodology.html)
- [Cisco AI Readiness Index assessment tool](https://www.cisco.com/c/m/en_us/solutions/ai/readiness-index/assessment-tool.html)

Singapore
- [IMDA: AI Bootcamp for enterprises](https://www.imda.gov.sg/resources/press-releases-factsheets-and-speeches/press-releases/2026/imda-launches-ai-bootcamp-for-enterprises)
- [IMDA: GenAI x Digital Leaders partner list](https://www.imda.gov.sg/-/media/imda/files/infocomm-media-landscape/research-and-statistics/generative-ai/genai-x-digital-leaders-details-of-participating-tech-partners.pdf)
- [Microsoft: AI QuickStart programme with IMDA and UOB](https://news.microsoft.com/source/asia/2026/02/06/microsoft-launches-ai-quickstart-programme-with-support-from-imda-and-uob/)
- [Databricks: partners with EDB and IMDA](https://www.databricks.com/company/newsroom/press-releases/databricks-partners-edb-and-imda-support-singapores-national-ai)
- [EDB: Databricks to invest more than US$350 million in Singapore](https://www.edb.gov.sg/en/news-and-insights/databricks-to-invest-more-than-us-350-million-in-singapore)
- [NTT DATA: Smart AI Agent launch](https://businesswire.com/news/home/20250220598238/en/NTT-DATA-Launches-Smart-AI-Agent%E2%84%A2-to-Accelerate-Generative-AI-Adoption-and-Drive-2-Billion-in-Revenue-by-2027)
- [Second Talent: AI outsourcing companies in Singapore](https://www.secondtalent.com/resources/ai-outsourcing-companies-singapore/)
- [IMDA: AI Verify](https://imda.gov.sg/How-We-Can-Help/AI-Verify)
- [PDPC: Singapore's approach to AI governance](https://www.pdpc.gov.sg/ai)

China
- [Media coverage of FDE moves by Chinese cloud vendors, incl. Alibaba Cloud partner system (bjnews)](https://www.bjnews.com.cn/detail/1790235076129483.html)
- [Media coverage of FDE moves by Chinese cloud vendors (mrjjxw)](https://www.mrjjxw.com/articles/2026-09-29/4595127.html)
- [10jqka: 明略科技 2026 interim results](https://stock.10jqka.com.cn/20260831/c679442002.shtml)
- [Tezign: AI FullStack](https://www.tezign.com/en/resources/ai-fullstack)
- [Tezign: Gartner 2024 Cool Vendor](https://tezign.com/en/updates/gartner-2024-genai-cool-vendor)
- [证券市场周刊: 360发布AI转型咨询服务](https://static.weeklyonstock.com/26/0629/zbf160054.html)
- [自动化网: 2026年中国AI+系统性变革咨询公司榜](https://www.zidonghua.com.cn/MSupplyChain/InfoWin/256164.html)
- [53AI: 埃森哲押注 FDE](https://www.53ai.com/news/zhinenghuagaizao/2026060291028.html)
- [Microsoft Learn: Microsoft 365 operated by 21Vianet](https://learn.microsoft.com/en-us/office365/servicedescriptions/office-365-platform-service-description/microsoft-365-operated-by-21vianet)
