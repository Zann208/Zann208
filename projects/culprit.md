# Culprit! — Research Website for The Cults of Privacy Technologies

**Role:** Documentation Lead  
**Course:** 261361 Software Engineering  
**Customer:** Asst. Prof. Dr. Jenjira Jaimunk, Lab Director, The Cults of Privacy Technologies, Department of Computer Engineering, Chiang Mai University  
**Team:** Culprit!, six members, Scrum  
**Status:** Delivered 9 October 2026; live in production  
**Live site:** https://www.culprits-mystery.party/  
**Staging:** https://culprit.wyco-dev.com/  
**Team repository:** https://github.com/Wyco68/CulpritWeb

## Project

Culprit! built the public website of The Cults of Privacy Technologies, a research lab working on information security, privacy for cloud-IoT platforms and privacy by design. The site covers About, Research, Publications, Team, Events and Make Appointment, with a page for every lab member and Calendly scheduling embedded on the appointment page. One administrator manages all content, signing in with a password and an emailed code.

## My contribution

As Documentation Lead, I maintain the project record and keep the documentation aligned with the team's actual implementation.

My work includes:

- document control, IDs, versions, review states and ownership
- Software Requirements Specification (SRS)
- requirement traceability from requirements to epics, user stories and sprint tasks
- project proposal and project plan
- product backlog documentation
- UI/UX design specification support
- meeting minutes and decision records
- sprint and task documentation
- test documentation and recorded findings
- maintaining the team's Notion project portal
- keeping documentation synchronized when customer feedback or implementation behaviour changes

## Documentation approach

The project uses a controlled Notion workspace as the main working project record. Requirements, user stories, tasks, sprint planning, decisions, meetings and controlled documents are kept connected so the team can trace a customer need from requirement through implementation and testing.

A key part of my role is preserving project history while keeping active specifications current. For example, when the implemented appointment flow changed from an earlier approval-based concept to direct embedded scheduling, the active requirement and SRS were updated while the original meeting record was kept as historical evidence.

## Final deliverables

All eleven documents were issued in their final versions on 9 October 2026 and combined into a 202-page system document package with contents and bookmarks.

| No. | Document | ID | Version | Pages |
|---|---|---|---|---|
| 01 | A1 Project Proposal | SE-PRO-001 | 1.1 | 6 |
| 02 | A2 Software Requirements Specification | SE-SRS-001 | 1.0 | 30 |
| 03 | A3 Software Design Specification | SE-SDS-002 | 2.0 | 57 |
| 04 | A4 Sprint 1 Demo and Presentation | SE-PRE-002 | 1.0 | 6 |
| 05 | A5 Sprint 2 Demo and Presentation | SE-PRE-003 | 1.0 | 8 |
| 06 | A6 System Document Package | A6 | 1.0 | 202 |
| 07 | System Document | SE-DSN-003 | 2.0 | 32 |
| 08 | Testing Document | SE-TST-002 | 2.0 | 12 |
| 09 | Application Manual | SE-DOC-002 | 2.0 | 28 |
| 10 | Meeting Minutes | SE-MIN-001 to 009 | 1.0 | 11 |
| 11 | Sprint 2 Report | SE-RPT-001 | 1.0 | 10 |

## Product highlights

- About and research profile for the lab
- research projects grouped by area, with funding details
- publications, team and member pages, and events
- embedded Calendly appointment scheduling
- single-administrator content management with an emailed second sign-in step

## Engineering context

The team built a single Next.js 15 application (React 19, TypeScript) organised as feature modules, each with the same four layers: route handler, input schema, service and repository. Data lives in PostgreSQL on Supabase through Prisma, with a Neon standby every six hours. Sign-in uses Better Auth with database-backed sessions, a mandatory emailed second step and backup codes. Cloudflare provides DNS, TLS, a WAF rule, Turnstile and R2 photo storage; Resend sends email. Testing uses Vitest, Testing Library and Playwright. Staging runs Node.js 22 in Docker on a VPS behind Caddy and is released automatically on every merge; production runs on Vercel. See the team repository for the implementation.

## What I learned

This project strengthened my ability to treat documentation as part of the engineering process rather than as a final report. I gained practical experience with requirements management, traceability, change control, Scrum documentation, meeting records, test documentation and keeping project documentation consistent with a continuously changing implementation.

---

This is a team project. The source repository is maintained by the Culprit! development team; this page documents my individual contribution as Documentation Lead.
