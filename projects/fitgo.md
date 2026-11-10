# FitGo: architecture

FitGo is a home fitness web app. One button, press play, follow along.

The source code is closed. This page shows how it is built.

[Open FitGo ↗](https://muriloapps.dpdns.org/fitgo/) · [Back to profile](../README.md)

> Click on the rows to expand or collapse.

<details>
<summary><strong>Background</strong></summary>

<blockquote>

I wanted a simpler way to exercise at home: one button, press play, follow along.

I started FitGo for myself, and to learn how to build with AI agents.

AI agents wrote much of the code. I set the product direction, architecture and specifications, and I review the quality.

It is now being tested with real users.

[Watch the pitch ↗](https://github.com/user-attachments/assets/47fb315b-e386-4b86-aff1-ef136eb6063d)

</blockquote>

</details>

<details open>
<summary><strong>Architecture</strong></summary>

<blockquote>

<details open>
<summary>Overview</summary>

<blockquote>

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

</blockquote>

</details>

<details>
<summary><strong>Quality and delivery</strong></summary>

<blockquote>

<details>
<summary>Testing</summary>

<blockquote>

- 34 Playwright end-to-end tests in the pre-merge checks.
- Automated smoke and core-test checks.

</blockquote>

</details>

<details>
<summary>Deployment</summary>

<blockquote>

- Staged integration and production deployments.

</blockquote>

</details>

</blockquote>

</details>

<details>
<summary><strong>Privacy and data handling</strong></summary>

<blockquote>

<details>
<summary>Consent</summary>

<blockquote>

- Opt-in analytics.
- Consent-based feedback.

</blockquote>

</details>

<details>
<summary>Retention</summary>

<blockquote>

- Retention controls.
- Scheduled data purges.

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
- I set the product direction, architecture and specifications.
- I review the code and own the quality.

</blockquote>

</details>

</blockquote>

</details>
