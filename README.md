# Murilo Bellatini

> +8 years · Software, data, and cloud engineering  
> M.Sc. Robotics & AI, Technical University of Munich

I work on AI platforms and the systems around them.

At BMW, I help shape the technical direction of an internal platform for building and sharing AI agents, working with teams across architecture, quality, and delivery.

Based in Munich, Germany.

[About Me ↗](https://muriloapps.dpdns.org/me) · [CV ↗](https://muriloapps.dpdns.org/me/cv.pdf) · [LinkedIn ↗](https://www.linkedin.com/in/mbellatini/)

---

## Portfolio

> Click on the rows to expand or collapse.

<details open>
<summary><strong>Enterprise AI Platforms</strong></summary>

<blockquote>

<details open>
<summary>BMW — AI Platform Engineering</summary>

<blockquote>

BMW employees needed an accessible, safe way to build their own AI agents.

We built an internal self-service platform that is now used by more than 70,000 people each month.

I contributed to the technical direction from concept through company-wide release.

<details>
<summary>Scope and outcomes</summary>

<blockquote>

- Internal self-service platform for building and sharing AI agents.
- Contributed to technical direction from concept through company-wide release.

</blockquote>

</details>

<details>
<summary>Technical contributions</summary>

<blockquote>

<details>
<summary>Delivery and quality</summary>

<blockquote>

- Co-designed branching, testing, and deployment strategies across teams.
- Helped introduce user acceptance testing and staged rollouts.
- Added automated Playwright end-to-end checks.

</blockquote>

</details>

<details>
<summary>Agent evaluation</summary>

<blockquote>

- Worked on self-service benchmarking for agent builders.
- Contributed to a quality-analysis framework for agent performance.

</blockquote>

</details>

<details>
<summary>Team collaboration</summary>

<blockquote>
Supported cross-functional teams through shadowing and reverse shadowing.

</blockquote>

</details>

</blockquote>

</details>

</blockquote>

</details>

</blockquote>

</details>
<details>
<summary><strong>AI-Native Product Delivery</strong></summary>

<blockquote>

<details>
<summary>FitGo — Home Fitness Application</summary>

<blockquote>

I wanted a simpler way to exercise at home: one button, press play, follow along.

I started FitGo for myself and as a way to explore AI-native development.

AI agents wrote much of the code. I focused on product direction, architecture, specifications, review, and quality.

The application is now entering validation with real users.

[Open FitGo ↗](https://muriloapps.dpdns.org/fitgo/)

<details>
<summary>Product Pitch</summary>

<blockquote>

<p>
  <video src="https://github.com/user-attachments/assets/47fb315b-e386-4b86-aff1-ef136eb6063d" controls width="320" muted playsinline>
    <a href="https://github.com/user-attachments/assets/47fb315b-e386-4b86-aff1-ef136eb6063d">Watch the pich ↗</a>
  </video>
</p>

</blockquote>

</details>

<details>
<summary>Technical implementation</summary>

<blockquote>

<details>
<summary>Architecture and hosting</summary>

<blockquote>

[![](https://mermaid.ink/img/pako:eNptUs1u2zAMfhWBpw2zjcRxms4YCtROHOSwtljWHWbnoNqMLVQWA0ZukgZ592mut_Uw6iLy-yEl8AwlVQgxbDUdykayFd_nhREuHvPHPfJG-P6NSLM81dRVWy0ZN294mvVQtsgzJmPRVF-e-CZTdknigE9C7nZaldIqMoMiW_SKZJEnsnweBHe1MkfxSTycbENG3D6sHPsfPxBLolqjWKva-CsjAuewvM-H6v1tZ5vBPunpP5DV9iRWc2HJ9Rj47y19X6Tz_EPCdHAPFJW08uM7CwevHbxGfvkPGog7POw1WutAbKXSfYfkW54wvtAGPKhZVRBb7tCDFtlxXArn3x4F2AZbLCB2V8aqO_qV5Ge_JE1cQGEuTr-T5idR-8eCqasbiLdS713W7dxEOFeyZtn-rbL7TOSUOmMhDiej3gTiMxwh9kfByMV4El3P3Imi2edRFIahByeIp8HU1aOr8fV4MruKpiH6s4sHr31_02ntAVbKEn99W5N-Wy6_AAXcrN0?type=png)](https://mermaid.live/edit#pako:eNptUs1u2zAMfhWBpw2zjcR1mtYYCtROHOSwtljaHWbnoNqMLVQWA0ZukgV592muu_Uw6iLy-yEl8AQlVQgxbDTty0ayFY-zwggXT_nTDnktfP9GpFmeauqqjZaM6zc8zXoom-cZk7Foqq_PfJMpuyCxx2cht1utSmkVmUGRzXtFMs8TWb4MgrtamYP4Ih6OtiEjbh-Wjv2PH4gFUa1RrFRt_KURgXNY3OdD9f62s81gn_T0H8hqcxTLmbDkegz8j5a-L9JZ_ilh2rsHikpa-fmDhYNXDl4hv_4HDcQd7ncarXUgtlLpvkPyPU8YX2kNHtSsKogtd-hBi-w4LoXTH48CbIMtFhC7K2PVHfxK8otfkiYuoDBnp99K85Oofbdg6uoG4o3UO5d1WzcRzpSsWbZ_q-w-EzmlzliIw_C6N4H4BAeI_VEwcjG-iK6m7kTR9HoUhWHowRHiSTBx9ehyfDW-mF5GkxD96dmDX31_02ntAVbKEn97W5N-W86_AQjbrOU)

<details>
<summary>Mermaid code</summary>

</details>


```mermaid
flowchart TD
    U[User] --> CF[Cloudflare]
    CF --> FE[Frontend<br>FitGo web application]
    FE --> BE[Backend<br>Nginx + Python API]

    FE -. Google Sign-In .-> GO[Google OAuth]
    BE -. Verify ID token .-> GO

    FE --- CD[(Browser data)]
    BE --- SD[(Server data)]
    BE -. Newsletter email .-> BR[Brevo]
```

</blockquote>

</details>

<details>
<summary>Authentication and email</summary>

<blockquote>

- Google Sign-In for cross-device data synchronisation.
- Brevo for newsletter delivery.

</blockquote>

</details>

<details>
<summary>Testing and deployment</summary>

<blockquote>

- 34 Playwright end-to-end tests included in the pre-merge checks.
- Staged integration and production deployments.
- Automated smoke and core-test checks.

</blockquote>

</details>

<details>
<summary>Privacy and data handling</summary>

<blockquote>

- Opt-in analytics.
- Consent-based feedback.
- Retention controls.
- Scheduled data purges.

</blockquote>

</details>

</blockquote>

</details>

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>Applied AI Research</strong></summary>

<blockquote>

<details>
<summary>Alma PHIL — Conversational Knowledge Graphs</summary>

<blockquote>

Conversations contain personal context: people, places, and the things that matter to them.

For my master’s research at [Alma PHIL ↗](https://almaphil.de/), I explored how to represent that context as a personal knowledge graph and retrieve information relevant to the current conversation.

This work became my master’s thesis at the [Technical University of Munich ↗](https://www.tum.de/).

<details>
<summary>Research and evaluation</summary>

<blockquote>

<details>
<summary>Approach</summary>

<blockquote>

- Explored training models to extract relationships from conversations.
- Built a knowledge graph from the extracted entities and relationships.
- Used the graph to retrieve relevant people, places, and topics.

</blockquote>

</details>

<details>
<summary>Evaluation</summary>

<blockquote>

Evaluated relationship extraction using precision, recall, and F1 score.

</blockquote>

</details>

<details>
<summary>Limitations</summary>

<blockquote>

The public training data did not closely match real healthcare conversations, limiting how well the evaluation represented the intended setting.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary>Demonstration</summary>

<blockquote>

[Watch the demonstration on YouTube ↗](https://youtu.be/K1lbAF3LXgk)

</blockquote>

</details>

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>Teaching and Knowledge Sharing</strong></summary>

<blockquote>

<details>
<summary>Practical Data Analysis Course</summary>

<blockquote>

I created *Estratégias de Análise de Dados* (*Strategies for Data Analysis*), a practical course for people moving into data analysis.

The course grew from a simple aim: make data analysis less abstract and connect the tools to real questions.

[View the course ↗](https://hotmart.com/pt-br/marketplace/produtos/estrategias-de-analise-de-dados)

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>Earlier Projects</strong></summary>

<blockquote>

<details>
<summary>Dialog2Rasa</summary>

<blockquote>

A tool for migrating chatbots from Dialogflow to Rasa.

[View on GitHub ↗](https://github.com/murilobellatini/dialog2rasa)

</blockquote>

</details>

<details>
<summary>Smart Poster</summary>

<blockquote>

A tool for generating social-media posts.

[View on GitHub ↗](https://github.com/murilobellatini/smart-poster)

</blockquote>

</details>

<details>
<summary>SegmentStyler</summary>

<blockquote>

Text-driven 3D styling, developed at the Technical University of Munich with [Maximilian Winter](https://github.com/MaximilianWinter).

[View on GitHub ↗](https://github.com/MaximilianWinter/SegmentStyler)

</blockquote>

</details>

</blockquote>

</details>

---

## Technical Skills

<details>
<summary><strong>Software, Cloud, and Delivery</strong></summary>

<blockquote>

<details>
<summary>Language</summary>

<blockquote>

- Python
- JavaScript

</blockquote>

</details>

<details>
<summary>Cloud and infrastructure</summary>

<blockquote>

- AWS
- Google Cloud
- Docker
- Nginx
- Cloudflare
- Terraform
- Floci (local cloud emulation)

</blockquote>

</details>

<details>
<summary>Testing and automation</summary>

<blockquote>

- GitHub Actions
- Playwright

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>AI Platforms</strong></summary>

<blockquote>

<details>
<summary>Agents and interoperability</summary>

<blockquote>

- LLM agents
- Model Context Protocol (MCP)
- Agent-to-Agent communication (A2A)
- Skills and tool use

</blockquote>

</details>

<details>
<summary>Retrieval and evaluation</summary>

<blockquote>

- Retrieval-augmented generation (RAG)
- GraphRAG
- LLM evaluation
- Human-in-the-loop workflows
- Multimodal AI

</blockquote>

</details>

<details>
<summary>Safety & governance</summary>

<blockquote>

- Moderation and guardrails
- OWASP LLM security
- Security and compliance

</blockquote>

</details>
</blockquote>

</details>

</blockquote>

</details>
