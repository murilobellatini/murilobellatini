# AI agents on a Raspberry Pi: architecture

Agents are only useful if you can trust them.

I run a small home server where AI agents build and run my apps.

I send daily commands from my phone. For deep work I use a code server.

The agents work inside a harness with guardrails. They send me a demo and a pull request. I approve. That is how I move fast and stay safe.

The source code is closed. This page shows how it is built.

[Back to profile](README.md)

> Click on the rows to expand or collapse.

<details open>
<summary><strong>Architecture</strong></summary>

<blockquote>

<details open>
<summary>Overview</summary>

<blockquote>

```mermaid
flowchart TD
    ME[Me<br>Phone for daily commands<br>Code server for deep dev work] --> AG[AI agents<br>Work inside a harness with guardrails]
    AG --> T[Pre-merge tests<br>Long Playwright journeys<br>Act like a real user]
    T --> PR[Demo and pull request<br>Sent to me by the AI]
    PR --> OK[I approve]
    OK --> LIVE[Live for users]

    PI[Raspberry Pi<br>Self-heals when it runs hot] -. Keeps running .-> AG

    classDef flow fill:#1e293b,stroke:#94a3b8,color:#f8fafc;
    classDef gate fill:#0f766e,stroke:#5eead4,color:#ffffff;
    classDef pi fill:#b45309,stroke:#fcd34d,color:#ffffff;
    class ME,AG,LIVE flow;
    class T,PR,OK gate;
    class PI pi;
```

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>AI guardrails</strong></summary>

<blockquote>

<details>
<summary>Before every merge</summary>

<blockquote>

- Git hooks run all unit tests.
- Long Playwright tests walk through each app like a real user.
- A merge queue merges one change at a time.

</blockquote>

</details>

<details>
<summary>Before it goes live</summary>

<blockquote>

- The AI sends me a demo and a pull request.
- Test site first. Live site only after my approval.
- Paid services are never called in tests.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>Self-healing</strong></summary>

<blockquote>

<details>
<summary>If the Pi runs hot</summary>

<blockquote>

- Heat, load and memory are checked all the time. The phone alerts me.
- A watchdog restarts what is down. Restarts are capped, then I get an alert.
- Agent sessions are saved every minute and reopened after a restart.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>Control</strong></summary>

<blockquote>

<details>
<summary>Phone and code server</summary>

<blockquote>

- Phone: one page to see, pause and resume every agent. Google login.
- Code server: a full editor in the browser for deep work.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>How it was built</strong></summary>

<blockquote>

<details>
<summary>Roles</summary>

<blockquote>

- AI agents wrote much of the code.
- I set the direction, the rules and the specifications.
- I review the result and own the quality.

</blockquote>

</details>

</blockquote>

</details>
