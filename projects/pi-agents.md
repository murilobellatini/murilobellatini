# AI agents on a Raspberry Pi: architecture

Agents are only useful if you can trust them.

I run AI agents on a small home server.

They send me a demo and a pull request. I approve.

I only review demos, so I move faster.

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

- Phone: daily commands, pause and resume. Behind Google sign-in, so only I can reach it.
- Code server: deep dev work in the browser.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>AI guardrails</strong></summary>

<blockquote>

<details>
<summary>Before it goes live</summary>

<blockquote>

- Automatic Playwright tests act like a real user, on every change.
- Old features keep working: all tests run each time.
- I try the demo myself, then approve.

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

- Phone alert. A watchdog restarts what is down.
- Agent sessions reopen after a restart.

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
- I set the rules and own the quality.

</blockquote>

</details>

</blockquote>

</details>
