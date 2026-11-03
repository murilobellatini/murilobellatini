# Murilo Bellatini

> Software, data, and cloud engineering · 8+ years  
> M.Sc. Robotics & AI, Technical University of Munich

I work on AI platforms and the systems around them.

At BMW, I contribute to the technical direction of an internal platform for building and sharing AI agents.

I work on architecture, quality, and delivery, together with the teams involved.

📍 Munich, Germany  
🎯 Open to Staff AI Platform Engineer and hands-on Tech Lead roles

[About Me](https://muriloapps.dpdns.org/me/d) · [CV](https://muriloapps.dpdns.org/me/cv.pdf) · [LinkedIn](https://www.linkedin.com/in/mbellatini/)

***

## Portfolio

<details open>
<summary><strong>Enterprise AI Platforms</strong></summary>

<br>

<details open>
<summary><strong>BMW — AI Platform Engineering</strong></summary>

<br>

BMW employees wanted to build their own AI agents, but had no simple or safe way to do so.

An internal self-service platform was built to address this. It is now used by more than 70,000 people each month.

I contributed to the platform’s technical direction from its early concept through company-wide release.

**Role:** Technical Lead · AI Platform Engineering

<details>
<summary>Context and outcomes</summary>

- The initial platform concept was delivered within three months; general availability followed within six.
- The platform now serves more than 70,000 monthly users, with approximately 7,000 daily users.
- I worked with a cross-functional group of more than 15 engineers across development, quality assurance, and user experience.
- The platform has operated without reported security or compliance breaches since 2024.

</details>

<details>
<summary>Areas of contribution</summary>

- Contributed to the branching, testing, and deployment strategy across contributing teams.
- Helped introduce user acceptance testing, staged rollouts, and automated Playwright end-to-end checks.
- Built self-service benchmarking for agent builders.
- Contributed to a quality-analysis framework for evaluating agent performance.
- Supported cross-functional teams through shadowing and reverse shadowing.

</details>

</details>

</details>

<details>
<summary><strong>AI-Native Product Delivery</strong></summary>

<br>

<details>
<summary><strong>FitGo — Home Fitness Application</strong></summary>

<br>

Fitness applications often introduce more complexity than many users need.

FitGo takes a simpler approach: one button, press play, follow along.

I built it as a personal project and as a way to explore AI-native development. AI agents wrote much of the code; I handled the product direction, architecture, specifications, review, and quality.

**Role:** Product Owner · Architect · Engineer

**[Open FitGo](https://muriloapps.dpdns.org/fitgo/)**

<details>
<summary>Demonstration</summary>

<p>
  <video src="https://github.com/user-attachments/assets/47fb315b-e386-4b86-aff1-ef136eb6063d" controls width="320px" muted playsinline>
    <a href="https://github.com/user-attachments/assets/47fb315b-e386-4b86-aff1-ef136eb6063d">Watch the demonstration</a>
  </video>
</p>

</details>

<details>
<summary>Architecture</summary>

```mermaid
flowchart LR
    U[User] --> CF[Cloudflare]
    CF --> FE[Frontend<br>FitGo web application]
    FE --> BE[Backend<br>Nginx + Python API]

    FE -. Google Sign-In .-> GO[Google OAuth]
    FE --- CD[(Browser data)]
    BE --- SD[(Server data)]
    BE -. Email .-> BR[Brevo]
```

- **Infrastructure:** Cloudflare edge, web frontend, and a Python API behind Nginx, hosted on a Raspberry Pi.
- **Authentication and communication:** Google Sign-In for cross-device synchronisation and Brevo for newsletter delivery.
- **Data:** Browser-based and server-side storage, separated by responsibility.

</details>

<details>
<summary>Engineering practices</summary>

- Included 34 Playwright end-to-end tests as part of the pre-merge quality gate.
- Used staged integration and production deployments.
- Automated smoke and core-test checks before release.
- Applied opt-in analytics, consent-based feedback, retention controls, and scheduled data purges.

</details>

</details>

</details>

<details>
<summary><strong>Applied AI Research</strong></summary>

<br>

<details>
<summary><strong>Alma PHIL — Conversational Knowledge Graphs</strong></summary>

<br>

Conversations contain context that is easy to lose: the people involved, where they live, and what matters to them. Chatbots, however, typically do not retain this context.

For my master’s research at [Alma PHIL](https://almaphil.de/), I explored whether conversations could be represented as a personal knowledge graph and used to retrieve relevant people, places, and topics.

This work became my master’s thesis at the [Technical University of Munich](https://www.tum.de/).

**Role:** Researcher · Machine Learning Engineer

<details>
<summary>Approach</summary>

- Trained machine-learning models to extract relationships from conversations.
- Constructed a knowledge graph from the extracted entities and relationships.
- Used the graph to retrieve contextually relevant people, places, and topics.

</details>

<details>
<summary>Evaluation and limitations</summary>

- Evaluated relationship extraction using precision, recall, and F1 score.
- A key limitation was that publicly available training data did not closely match real healthcare conversations.
- These findings informed the scope and limitations of the approach.

</details>

<details>
<summary>Demonstration</summary>

<a href="https://youtu.be/K1lbAF3LXgk">
  <img src="https://img.youtube.com/vi/K1lbAF3LXgk/hqdefault.jpg" alt="Alma PHIL demonstration video" width="480"><br>
  Watch the demonstration on YouTube
</a>

</details>

</details>

</details>

<details>
<summary><strong>Teaching and Knowledge Sharing</strong></summary>

<br>

<details>
<summary><strong>Practical Data Analysis Course</strong></summary>

<br>

Data analysis can feel abstract: tools, theory, and terminology often appear before learners have the chance to work through a real question.

I developed **Estratégias de Análise de Dados** (*Strategies for Data Analysis*), a practical course for people moving into data analysis.

**Role:** Course Creator · Instructor

**[View the course](https://hotmart.com/pt-br/marketplace/produtos/estrategias-de-analise-de-dados)**

</details>

</details>

<details>
<summary><strong>Earlier Projects</strong></summary>

<br>

<details>
<summary><strong>Dialog2Rasa</strong></summary>

A tool for migrating chatbots from Dialogflow to Rasa.

**[View on GitHub](https://github.com/murilobellatini/dialog2rasa)**

</details>

<details>
<summary><strong>Smart Poster</strong></summary>

A tool for generating social-media posts.

**[View on GitHub](https://github.com/murilobellatini/smart-poster)**

</details>

<details>
<summary><strong>SegmentStyler</strong></summary>

A 3D styling tool driven by text input, developed at the Technical University of Munich with [Maximilian Winter](https://github.com/MaximilianWinter).

**[View on GitHub](https://github.com/MaximilianWinter/SegmentStyler)**

</details>

</details>

***

## Technical Skills

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)

<details>
<summary>AI platform focus</summary>

- Large language model agents
- Model Context Protocol (MCP)
- Agent-to-Agent communication (A2A)
- Skills and tool use
- Retrieval-augmented generation (RAG)
- LLM evaluation
- Human-in-the-loop workflows
- Security and compliance

</details>
