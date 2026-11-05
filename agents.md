# AI agents on a Raspberry Pi: architecture

Agents are only useful if you can trust them.

I run a small home server where AI agents build and run my apps. One Raspberry Pi, 8 GB of memory.

I built the safety first: limits, a stop button, and tests before every change.

The source code is closed. This page shows how it is built.

[Back to profile](README.md)

> Click on the rows to expand or collapse.

<details open>
<summary><strong>Architecture</strong></summary>

<blockquote>

<details>
<summary>Overview</summary>

<blockquote>

```mermaid
flowchart TD
    ME[Me, on my phone] --> CF[Cloudflare tunnel + Google login]
    CF --> NG[Nginx]
    NG --> CTL[Agent control page]
    NG --> APPS[My apps]

    CTL --> AG[AI agent sessions]
    AG --> GIT[Git: tests run before every merge]
    GIT --> APPS

    WATCH[Watchdog: heat, load, memory] -. alert + pause .-> AG
    WATCH -. phone alert .-> ME
    BOOT[Boot restore] -. reopens sessions .-> AG
```

</blockquote>

</details>

<details>
<summary>Control</summary>

<blockquote>

- One phone page lists every running agent.
- Pause or resume one agent, or all of them.
- Each agent shows its state, its last request and what it is doing now.
- Scheduled tasks start agents on a timer, each in its own copy of the code.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>Safety and self-repair</strong></summary>

<blockquote>

<details>
<summary>Safety</summary>

<blockquote>

- Heat, load and memory limits. The phone alerts me.
- Google login on everything public. Admin actions need a PIN.
- Paid services are never called in tests.
- No outside messages without my approval.

</blockquote>

</details>

<details>
<summary>Self-repair</summary>

<blockquote>

- Open agent sessions are saved every minute and reopened after a restart.
- A watchdog restarts what is down.
- Restarts are capped. After that I get a red alert.
- A rebuild kit sets the Pi up again from scratch. Its test checks it against the live machine.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>Quality and delivery</strong></summary>

<blockquote>

<details>
<summary>Testing</summary>

<blockquote>

- Git hooks run all tests before every merge.
- Playwright tests walk through each app like a user.

</blockquote>

</details>

<details>
<summary>Deployment</summary>

<blockquote>

- A merge queue merges one change at a time, on top of the latest code.
- Test site first, live site after my approval.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>How it was built</strong></summary>

<blockquote>

- AI agents wrote much of the code.
- I set the direction, the rules and the specifications.
- I review the result and own the quality.

</blockquote>

</details>
