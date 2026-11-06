# Murilo Bellatini

> +8 years · Software, data, and cloud engineering  
> M.Sc. Robotics & AI, Technical University of Munich

I help companies get AI agents to work.

At BMW, I am technical lead for the generative AI agent platform. Employees build and run their own AI agents on it.

Based in Munich, Germany.

[About Me ↗](https://muriloapps.dpdns.org/me/) · [CV ↗](https://muriloapps.dpdns.org/me/cv.pdf) · [LinkedIn ↗](https://www.linkedin.com/in/mbellatini/)

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

First test version after 3 months, company-wide launch after 6.

I own the platform core and co-designed the delivery process. 5+ teams ship on it.

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
<summary>AI Agents on a Raspberry Pi — Safe Agent Operations</summary>

<blockquote>

Agents are only useful if you can trust them.

I run AI agents on a small home server. They send me a demo and a pull request. I approve. I only review demos, so I move faster.

[Architecture ↗](projects/pi-agents.md) (the code is closed source)

<details>
<summary>Technical implementation</summary>

<blockquote>

<details>
<summary>Architecture and hosting</summary>

<blockquote>

[![](https://mermaid.ink/img/pako:eNp1km9r2zAQh7_KobzpwA7dknaNOzoC6YLpP-OFwWj6QrZPtjZZ8iQ5JYR8953tkJJC9dK657nfnbVjuSmQRUwo85pX3HpYLdYa6DzcPq_ZA37L7M1ZUhmN8Cp9BUtjSoXgZKlDqQPoeHBoN2g_rdkLhOENzJeEzmPgJWrvekOsnaTCsuW2sFwq1xUPjebLHlp1TOtNzb3MwaM7kClyFbbUAf6Y1mrcugCMBqSGW6DIusQ314pUkHDnemWSknOBtQGuC2hapcDiv5bUQybwpJAe6q1DJU4sY_hBKWHcTzN8TdJe-nS3I6kBGq9prNng9zXbDxVPd1373zh0v49_3T7fyw2-vN2O4dF42KI_mg_umJKm3DUZWsqUyD7gT0oVVjS_G1Z7yuSK5lyggO7fgZBKRaPP-GU2yQLnrfmL0Wg25ZPsKsiNMjYaiSvBRX79ji65xwN9Lr5eXuKRvkDkxfRI9-c93cgDm00vJuezIyvyYjItPmbpeQXzZdDtqM9_crcKkjSgdXXRTi6SmBpes4DVaGsuCxbtmK-w7l5wgYK3yrP9_j-DmeHw?type=png&bgColor=ffffff)](https://mermaid.live/edit#pako:eNp1km9r2zAQh7_KobzpwA7dknaNOzoC6YLpP-OFwWj6QrZPtjZZ8iQ5JYR8953tkJJC9dK657nfnbVjuSmQRUwo85pX3HpYLdYa6DzcPq_ZA37L7M1ZUhmN8Cp9BUtjSoXgZKlDqQPoeHBoN2g_rdkLhOENzJeEzmPgJWrvekOsnaTCsuW2sFwq1xUPjebLHlp1TOtNzb3MwaM7kClyFbbUAf6Y1mrcugCMBqSGW6DIusQ314pUkHDnemWSknOBtQGuC2hapcDiv5bUQybwpJAe6q1DJU4sY_hBKWHcTzN8TdJe-nS3I6kBGq9prNng9zXbDxVPd1373zh0v49_3T7fyw2-vN2O4dF42KI_mg_umJKm3DUZWsqUyD7gT0oVVjS_G1Z7yuSK5lyggO7fgZBKRaPP-GU2yQLnrfmL0Wg25ZPsKsiNMjYaiSvBRX79ji65xwN9Lr5eXuKRvkDkxfRI9-c93cgDm00vJuezIyvyYjItPmbpeQXzZdDtqM9_crcKkjSgdXXRTi6SmBpes4DVaGsuCxbtmK-w7l5wgYK3yrP9_j-DmeHw)

<details>
<summary>Mermaid code</summary>

```mermaid
flowchart TD
    ME["Me<br>(Phone with Google sign-in, code server)"] --> AG["AI agents<br>(Inside guardrails)"]
    AG --> T["Automatic tests<br>(Real-user journeys, on every change)"]
    T -- Pass --> PR["Demo and pull request<br>(I try it myself)"]
    T -. Fail .-> AG
    PR --> OK{"Do I approve?"}
    OK -- Yes --> LIVE[Live]
    OK -. Not yet .-> AG

    PI["Raspberry Pi<br>(Self-heals)"] -.-> AG

    classDef flow fill:#1e293b,stroke:#94a3b8,color:#f8fafc;
    classDef gate fill:#0f766e,stroke:#5eead4,color:#ffffff;
    classDef pi fill:#b45309,stroke:#fcd34d,color:#ffffff;
    class ME,AG,LIVE flow;
    class T,PR,OK gate;
    class PI pi;
```

</details>

</blockquote>

</details>

<details>
<summary>AI guardrails</summary>

<blockquote>

- Automatic Playwright tests act like a real user, on every change.
- Old features keep working: all tests run each time.
- I try the demo myself, then approve.

</blockquote>

</details>

<details>
<summary>Self-healing</summary>

<blockquote>

- Phone alert. A watchdog restarts what is down.

</blockquote>

</details>

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary>FitGo — Home Fitness Application</summary>

<blockquote>

I wanted a simpler way to exercise at home: one button, press play, follow along.

I started FitGo for myself and as a way to explore AI-native development.

AI agents wrote much of the code. I focused on product direction, architecture, specifications, review, and quality.

The application is now entering validation with real users.

[Open FitGo ↗](https://muriloapps.dpdns.org/fitgo/) · [Architecture ↗](projects/fitgo.md) (the code is closed source)

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

[![](https://mermaid.ink/img/pako:eNptUs1u2zAMfhWBpw2zjcRxms4YCtROHOSwtljaHWbnoNqMLVQWA0ZukgV592muu_Uw6iLy-yEl8AQlVQgxbDTty0ayFY-zwggXT_nTDnktfP9GpFmeauqqjZaM6zc8zXoom-cZk7Foqq_PfJMpuyCxx2cht1utSmkVmUGRzXtFMs8TWb4MgrtamYP4Ih6OtiEjbh-Wjv2PH4gFUa1RrFRt_KURgXNY3OdD9f62s81gn_T0H8hqcxTLmbDkegz8j5a-L9JZ_ilh2rsHikpa-fmDhYNXDl4hv_4HDcQd7ncarXUgtlLpvkPyPU8YX2kNHtSsKogtd-hBi-w4LoXTH48CbIMtFhC7K2PVHfxK8otfkiYuoDBnp99K85Oofbdg6uoG4o3UO5d1WzcRzpSsWbZ_q-w-EzmlzliIw_C6N4H4BAeI_VEwcjG-iK6m7kTR9HoUhWHowRHiSTBx9ehyfDW-mF5GkxD96dmDX31_02ntAVbKEn97W5N-W86_AQjbrOU)

<details>
<summary>Mermaid code</summary>

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

</details>

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

[Watch the demonstration on YouTube ↗](https://youtu.be/K1lbAF3LXgk) · [Code: RelNetCare ↗](https://github.com/murilobellatini/RelNetCare)

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary>SegmentStyler</summary>

<blockquote>

Text-driven 3D styling, co-developed at the Technical University of Munich with [Maximilian Winter](https://github.com/MaximilianWinter).

[View on GitHub ↗](https://github.com/MaximilianWinter/SegmentStyler)

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
<summary>Newspapers Text Mining</summary>

<blockquote>

A classifier that sorts newspaper articles into 6 topics, with 82% accuracy. It runs as a containerized API.

[View on GitHub ↗](https://github.com/murilobellatini/newspapers-text-mining)

</blockquote>

</details>

<details>
<summary>iFood Data Architect Test</summary>

<blockquote>

A local data lake prototype with PySpark, Jupyter and Docker.

[View on GitHub ↗](https://github.com/murilobellatini/ifood-data-architect-test)

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
