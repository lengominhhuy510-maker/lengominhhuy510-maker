# Le Ngo Minh Huy

**Final-year Logistics and Supply Chain Management**

<a href="https://github.com/lengominhhuy510-maker/Tracking-Shipment-webapp">
  <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=500&size=22&pause=1200&color=2563EB&width=680&lines=Interested+in+digital+supply+chain;Applying+AI+automation+to+everyday+operations;Self-learning%2C+one+small+project+at+a+time;Curious+about+what+can+be+automated" alt="Focus areas" />
</a>

---

## What I'm exploring

Logistics and supply chain is the domain; AI automation is the thing I keep coming back to. The question that holds my attention: inside a routine operational process, which parts are only manual because nobody has modelled them yet, and which parts genuinely need a person to decide.

Not an expert in either. Still reading, still building small things, still checking my own conclusions against what the process actually does.

| Project | The question behind it |
|---|---|
| **[Tracking-Shipment-webapp](https://github.com/lengominhhuy510-maker/Tracking-Shipment-webapp)** | Manual shipment lookup took 11.2 minutes per container, measured with a stopwatch across four to five separate sources. Can live vessel tracking plus AI-read carrier emails bring that under one minute, without letting a machine overwrite an operational record unsupervised? Built as a post-sales monitoring add-on for FCL import and export: live AIS position, rule-based ETA, email-derived proposals that a staff member approves before anything changes. |
| **[challange-C](https://github.com/lengominhhuy510-maker/challange-C)** | If one model answers a question badly, does asking several models and letting them check each other help? Built a multi-agent pipeline for multiple-choice answering that works offline, with retrieval-augmented generation and a degraded mode for when the knowledge base has nothing useful. |
| **[RTCF](https://github.com/lengominhhuy510-maker/RTCF)** | A supply chain simulation handed me a set of results and I wanted to know two things: could the calculation run itself instead of being worked by hand, and was the answer actually the best one or just the first one that worked? Rebuilt the KPI engine to compute automatically, then used Optuna to search the configuration space for a better result. |

---

## Questions I keep asking

Every project above started from one of these, not from a technology choice.

- **Which step in this process costs the most time?** Before changing a process, measure it. The 11.2 minutes in the shipment project came from timing each lookup step separately, not from asking people how long it felt. The expensive step turned out to be switching between sources and retyping the same container number, not the lookup itself.
- **What is the real unit of work here?** A shipment is not one object; it is a booking, a container, a vessel, a voyage, a set of milestones, and a stream of carrier notices that each change on a different schedule. Getting that boundary wrong makes everything downstream wrong.
- **Which part can a machine decide, and which part must a person decide?** A system can compute an arrival estimate and read an email. It cannot accept the operational consequence of being wrong. So proposals get generated automatically and approved by a human — the audit trail stays intact either way.
- **If this automation is wrong, who finds out?** An email parser that misreads a rollover notice is worse than no parser, because it looks authoritative. Every automated output needs a visible source, a confidence, and a way back, and the person who approves it has to be able to see why it fired.
- **Is this the best answer, or just the first one that ran?** The supply chain simulation ended with a working calculation, which was not the same as a good one. Search the space before calling it done.

---

## Where I've used these

**Domain** — FCL import and export operations · Incoterms groups E/F and C/D · post-sales customer care · process mapping · operational time measurement

**Working with AI** — multi-agent orchestration · retrieval-augmented generation · structured extraction from email with validation · human-in-the-loop design · task decomposition when building with AI assistance

**Tools I've picked up** — Python · FastAPI · SQLAlchemy · PostgreSQL · React · TypeScript · Docker Compose · Playwright · R

---

## Contact

[![Email](https://img.shields.io/badge/Email-lengominhhuy510@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:lengominhhuy510@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-lengominhhuy510--maker-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/lengominhhuy510-maker)

---

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/lengominhhuy510-maker/lengominhhuy510-maker/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/lengominhhuy510-maker/lengominhhuy510-maker/output/github-contribution-grid-snake.svg" />
  <img alt="Contribution graph" src="https://raw.githubusercontent.com/lengominhhuy510-maker/lengominhhuy510-maker/output/github-contribution-grid-snake.svg" />
</picture>
