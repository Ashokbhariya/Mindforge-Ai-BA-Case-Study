# MindForge AI — Business Analysis Case Study

**Role**: Business Analyst · **Type:** AI-powered personalized learning platform · **Duration:** 12–13 day training-cum-hackathon program (Brudite Pvt. Ltd.)

[Live Project →](https://mind-forge-ai-three.vercel.app)

------------------------------------------------------------------------------------------------------------------------------------------------


## Overview

| | |
|---|---|
| **Problem** | Standardized e-learning platforms give every learner the same content and pace, leading to low engagement and poor retention. |
| **Solution** | An AI-driven platform that assesses learner knowledge, generates a personalized roadmap, and tracks retention over time. |
| **My Contribution** | Authored the full requirements chain end-to-end — BRD → FRD → User Stories — with complete traceability, prioritization, and a documented risk register. |

------------------------------------------------------------------------------------------------------------------------------------------------

## Documents

| Document | Contents | Link |
|---|---|---|
| Business Requirements (BRD) | 10 prioritized BRs, stakeholder matrix, risk register, scope | [View PDF](BRD_MindForgeAI.pdf) |
| Functional Requirements (FRD) | 9 FRs mapped to BRs, business rules, validation logic | [View PDF](FRD_MindForgeAI.pdf) |
| User Stories & Acceptance Criteria | 10 stories, 7 epics, Given–When–Then format, story points | [View PDF](User_Stories_&_Acceptance_Criteria_MindforgeAi.pdf) |

------------------------------------------------------------------------------------------------------------------------------------------------

## Requirement Traceability

| BR | Business Requirement | FR | Functional Requirement | User Story |
|---|---|---|---|---|
| BR-001 | User registration & authentication | FR-001 | Registration & Authentication | US-001, US-002 |
| BR-002 | Assess knowledge via SkillScan AI | FR-002 | SkillScan AI | US-003 |
| BR-003 | Generate personalized roadmap | FR-003 | Roadmap Generator | US-004 |
| BR-005 | Generate & evaluate quizzes | FR-004 | Learn & Quiz | US-005, US-006 |
| BR-007 | Track retention, recommend revision | FR-006 | Knowledge Decay Tracker | US-008 |
| BR-009 | Interactive progress dashboard | FR-008 | Progress Dashboard | US-009 |

*Full traceability for all 10 BRs is in BRD, Section 7.*

------------------------------------------------------------------------------------------------------------------------------------------------

## Key BA Decisions

**1. Scoped out mobile, live tutoring, multi-language, and LMS integrations**
Prioritized a complete, working web MVP over a partial multi-platform build within the fixed timeline.

**2. Made SkillScan a hard prerequisite for roadmap generation (BRL-001)**
Roadmap quality depends entirely on assessment accuracy — sequencing this correctly upfront avoided rework later.

**3. Split "Concept Confusion Detection" from "Knowledge Decay Tracking" (FR-006 vs FR-007)**
Both drive revision recommendations, but trigger on different signals — retention decay vs. repeated quiz errors — so each needed its own business rule rather than being merged into one feature.

------------------------------------------------------------------------------------------------------------------------------------------------

## Wireframes

Low-fidelity wireframes for the four core flows (Auth, SkillScan, Roadmap, Dashboard) are included alongside the relevant FR/User Story sections in the documents above.

------------------------------------------------------------------------------------------------------------------------------------------------

## Tech Context (for reference)

FastAPI · PostgreSQL · Qdrant (vector search) · LLM-based content generation
