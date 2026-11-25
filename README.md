<h1 align="center">Reitumetse Mafojane</h1>

<p align="center">
  Second-year BSc Computer Science at Eduvos, finishing 2027 &nbsp;·&nbsp; Johannesburg<br>
  <b>Heading for IT support, cloud and infrastructure</b>
</p>

<p align="center">
  <a href="https://tumi-devs-portfolio.vercel.app"><b>Portfolio and write-ups</b></a>
  &nbsp;·&nbsp;
  <a href="https://citadelfitness.app">Citadel Fitness</a>
  &nbsp;·&nbsp;
  <a href="https://linkedin.com/in/mafojaner">LinkedIn</a>
</p>

---

> Most of what I can actually do, I learned by building something that then broke in a way
> I had to understand.

## Built

### Citadel Fitness

An Android app for gym beginners, on Google Play, built and directed on my own from concept
to release. TypeScript with React Native and Expo, with iOS and web building from the same
source. Built with AI-assisted development using Claude.

Two decisions it is worth knowing I made, and why:

**The workout draft is persisted to device storage.** Android closes backgrounded apps, so
a lifter who takes a call mid-session does not come back to an empty screen.

**Rewards, tiers and quotas are decided in security-definer SQL, not in the client.**
Whoever is holding the phone can reach anything the client decides.

<details>
<summary><b>How the rest of it is put together</b></summary>

<br>

| | |
| --- | --- |
| **Backend** | Supabase. PostgreSQL across 105 migrations, row-level security on every table, 20 Deno edge functions covering the admin, billing and email paths |
| **App** | React Navigation, Zustand, offline persistence, native notifications, secure store, image handling |
| **Quality** | 1 200 Jest tests, type checking and linting on every push and again in GitHub Actions |
| **Operations** | EAS Build on four profiles, Sentry for crashes, PostHog for analytics, RevenueCat billing wired up but switched off at the key |
| **Website** | citadelfitness.app and the developer dashboard are hand-written HTML, CSS and JavaScript on Vercel, every third-party script vendored and hash-checked so the Content Security Policy can stay strict |

I also audited the product against its own claims. A checklist item marked verified turned
out to be a migration that had never run, and backup retention could outlive the deletion
window the privacy policy promises. Neither drifts unnoticed now: a 42-check probe
re-derives the security claims against the live backend, and a test fails when the
retention number and the policy disagree.

</details>

## Coursework, done by hand

Nine written reports, with the code and the marks, are on
[the portfolio](https://tumi-devs-portfolio.vercel.app). The four I would read first:

| Write-up | What it shows |
| --- | --- |
| **Database paradigms** | One library modelled three times over, in Oracle, MongoDB and Neo4j, so the trade-off between them is tested rather than quoted |
| **Pico environmental monitoring** | MicroPython, ARMv6-M Thumb assembly and C with a Makefile, on a breadboard, reading a thermistor through Steinhart-Hart |
| **Cloud architecture** | A multi-region platform on AWS, with the VPC half provisioned in the console rather than drawn in a diagram |
| **Smart campus software design** | Two systems designed against SOLID, then argued against rather than defended |

Scenario write-ups are hypothetical teaching cases, not client work, and say so on the page.

## The code

| Repository | What is in it |
| --- | --- |
| [database-paradigms](https://github.com/mafojaner/database-paradigms) | The Oracle schema and procedures, the Mongo collections, the Neo4j dump |
| [cpp-phonebook-and-utilities](https://github.com/mafojaner/cpp-phonebook-and-utilities) | A file-backed phonebook and two console utilities |
| [it-support-networking-fundamentals](https://github.com/mafojaner/it-support-networking-fundamentals) | The scenario-based support and networking write-up |
| [cpp-console-programs](https://github.com/mafojaner/cpp-console-programs) | Four C++ console programs, standard library only |

## What I work with

| Area | What I use |
| --- | --- |
| **Operating systems** | Linux on VirtualBox, Windows, macOS; shell scripting for routine tasks |
| **Networking and security** | LAN, WAN and WLAN design, IP addressing, routing and switching, Cisco Packet Tracer, two-factor authentication |
| **Cloud** (coursework) | AWS using EC2, ECS, VPC, Aurora, CloudFront and Route 53, against Well-Architected principles |
| **Programming** | C++, C#, SQL, TypeScript, JavaScript, HTML, CSS, MicroPython, PHP. Java and Python at foundation level |
| **Databases** | Oracle with PL/SQL procedures, MongoDB, Neo4j and Cypher, PostgreSQL and Supabase, database design, row-level security |
| **Deployment and quality** | Vercel, EAS Build, GitHub Actions, Jest, Sentry, PostHog, Content Security Policy |
| **Hardware** | PC component installation and assembly, operating system setup on new builds, Raspberry Pi, Arduino |

**Currently studying:** Network Security · Data Structures and Algorithms in C# · Digital
Electronics and Microcontrollers

## Before university

I ran a photography business, booking three or four clients a month, and then My Port,
doing technology work for small businesses. Both taught me things a module cannot: what a
client means as opposed to what they say, what to charge, and when to say no.

---

<p align="center">
  16 distinctions out of 19 modules passed &nbsp;·&nbsp; Top Achiever Award, Eduvos, 2026
</p>

<!--
  DESIGN NOTES, so nobody undoes this by accident.

  Every visual element here is doing a job:
    - The centred header is the three-second answer: who, where, heading for what, and the
      three places to click. Nothing competes with it.
    - The pull quote is the one line that is yours and nobody else's. It gets the only
      piece of real estate that interrupts the page.
    - Citadel's two "why" paragraphs are above the fold; the stack table is behind
      <details> so depth is one click away instead of a wall. A reader who does not care
      about Deno edge functions never has to scroll past them.
    - The tables exist because comma-separated prose does not scan. Seven paragraphs of
      technologies is seven paragraphs nobody reads; seven rows is a five-second skim.

  WHAT IS DELIBERATELY NOT HERE, and why:
    - Shields.io language badges. They say the same as the Programming row and cannot
      express "Java and Python at foundation level", so they would make the page less
      honest, not more attractive.
    - GitHub stats, streak and trophy cards. They measure commit frequency, not work, they
      are on every student profile, and they break when the third-party service goes down.
    - A header banner image. It would need to work in GitHub dark mode and light mode and
      carry no information either way.

  THE FOUR REPOS WENT PUBLIC ON 25 NOVEMBER 2026, so "The code" is now in the page above
  rather than waiting in here.

  DONE ON THE ACCOUNT: the four are pinned, in the order of that table. python-training
  is archived.

  Git-CS and MD-GUIDE are staying active, her decision on 25 November 2026, until there
  is more cloud work to put beside them. Do not raise it again. Pinning was the step that
  mattered anyway: "Popular repositories" is replaced by "Pinned" the moment anything is
  pinned, so those two no longer lead the page either way.

  STILL OPEN: none of the four repositories has a GitHub description, so the pinned cards
  show a name and a language and nothing else. The description is the one line a visitor
  reads before deciding to click. Set it with the gear beside "About" on each repo page.

  tumi-devs-portfolio stays PRIVATE, her decision on 25 November 2026. The site is linked
  twice above, which is what a reader wants: the work, not the repository that builds it.

  CHECK THE PREVIEW TAB BEFORE COMMITTING. The <details> block and the tables render
  correctly on github.com but not in every editor.
-->
