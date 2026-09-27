# USMLE Prep Pro Tools

### Personal study analytics for high-volume USMLE Q-bank preparation

*Browser-integrated study analytics · data visualization · AI-assisted software development*

> **Portfolio case study. Source code and implementation details are intentionally private.**

USMLE Prep Pro Tools is a personal study-analytics toolkit I developed during my own USMLE Q-bank preparation to make question progress, focused study sessions, break patterns, review activity, session history, and circadian study patterns clearly visible.

What began as a reliable daily question counter evolved through sustained daily use and dozens of revisions into a broader system designed to structure concentration, understand study timing, and support long-term performance.

<p align="center">
  <img src="media/screenshots/03_qbank-pro-assist_live-dashboard.png" width="100%" alt="USMLE Prep Pro Tools live dashboard">
</p>

*Live Q-bank session view combining question progress, break tracking, focused study blocks, session analytics, coaching, and circadian context.*

> Screenshots throughout this page reflect my own real study use rather than demonstration data. Some retain earlier internal interface labels from the project's development.

---

## At a Glance

- **Question progress** — tracks completed Q-bank questions and long-term volume
- **Separate solving and review workflows** — active question-solving and later review are measured independently
- **Focus and break analysis** — makes uninterrupted study periods, interruptions, and break behavior visible
- **Session analytics** — turns study and break segments into timelines and activity waveforms
- **Longitudinal and circadian views** — compares sessions across days and against time of day
- **Personal motivational layer** — integrates selected quotations and coaching elements into the study environment

---

## The Toolkit

The project developed into three connected components:

| Component | Purpose |
| --- | --- |
| **QBank Pro Assist** | Central session interface for question progress, study and break behavior, timelines, coaching, history, and circadian visualization |
| **Test Timer** | Tracks questions actively solved and converts question volume into daily, hourly, and long-term analytics |
| **Review Timer** | Separately tracks questions reviewed so that solving and reviewing remain distinct study activities |

The separation became important because answering new questions and reviewing completed questions are different study activities with different goals.

---

# QBank Pro Assist

## From a Clean Start to a Live Session

Before a session begins, the interface establishes the question blocks, break budget, study/break panels, session timeline, and circadian map.

<p align="center">
  <img src="media/screenshots/01_qbank-pro-assist_clean-start.png" width="90%" alt="QBank Pro Assist clean session start">
</p>

*Ready state before the first question — session targets, question blocks, break budget, study/break panels, and circadian context are already visible.*

### Coaching and motivation

<p align="center">
  <img src="media/screenshots/02_qbank-pro-assist_coaching-pre-session.png" width="70%" alt="QBank Pro Assist coaching and motivational layer">
</p>

*Selected quotations and Topper Counsel formed a personal motivational layer around the study session.*

Once active, the interface becomes a live representation of the session: question progress, focused study blocks, breaks, elapsed time, and behavioral patterns develop together.

---

## Study and Break Activity

Raw totals were not enough. I wanted to see the *shape* of a study session.

<p align="center">
  <img src="media/screenshots/04_qbank-pro-assist_activity-waveforms.png" width="100%" alt="Study and break activity waveforms">
</p>

Study and break segments are represented separately, making longer uninterrupted blocks, brief interruptions, and extended breaks visible rather than hiding them inside a single duration total.

---

## A Shared 18-Hour Session Canvas

Individual sessions become far more useful when they can be compared on the same scale.

<p align="center">
  <img src="media/screenshots/05_qbank-pro-assist_18hour-history-canvas.png" width="100%" alt="18-hour session history comparison canvas">
</p>

Historical sessions are plotted against the same **18-hour canvas**, with a consistent reference plan above them. Differences in start time, session length, test time, break time, and question volume can therefore be compared directly.

---

## Circadian Study Patterns

<p align="center">
  <img src="media/screenshots/06_qbank-pro-assist_multiday-circadian-history.png" width="100%" alt="Multi-day circadian session history">
</p>

Adding time-of-day context made it possible to look beyond individual sessions and quickly see when studying tended to begin, when longer focused periods occurred, and how those patterns shifted across days.

---

# Question Solving vs. Question Review

One of the most important design decisions was **not combining everything into one counter**.

Solving a new question and reviewing an already-completed question are different study activities, so I maintained independent analytics for both.

<table>
<tr>
<td width="50%" valign="top">
<b>Test Timer — Questions Solved</b><br><br>
<img src="media/screenshots/07_test-timer_alltime-summary.png" width="100%" alt="Test Timer all-time summary">
</td>
<td width="50%" valign="top">
<b>Review Timer — Questions Reviewed</b><br><br>
<img src="media/screenshots/11_review-timer_alltime-summary.png" width="100%" alt="Review Timer all-time summary">
</td>
</tr>
</table>

The resulting histories reflect sustained real-world use rather than a small demonstration dataset.

---

## Daily Progress

The daily question graph was where the entire project began.

Without a visual record, progress felt vague. Once question volume became visible day by day, productive and unproductive periods were much easier to recognize.

<table>
<tr>
<td width="50%" valign="top">
<b>Daily solving history</b><br><br>
<img src="media/screenshots/08_test-timer_daily-history.png" width="100%" alt="Daily question solving history">
</td>
<td width="50%" valign="top">
<b>Daily review history</b><br><br>
<img src="media/screenshots/12_review-timer_daily-history-aug.png" width="100%" alt="Daily question review history">
</td>
</tr>
</table>

---

## Time-of-Day Patterns

I also wanted to know *when* productive bursts were occurring rather than looking only at daily totals.

<table>
<tr>
<td width="50%" valign="top">
<b>Question-solving activity by hour</b><br><br>
<img src="media/screenshots/09_test-timer_hourly-activity.png" width="100%" alt="Hourly question solving activity">
</td>
<td width="50%" valign="top">
<b>Question-review activity by hour</b><br><br>
<img src="media/screenshots/10_review-timer_hourly-activity.png" width="100%" alt="Hourly question review activity">
</td>
</tr>
</table>

---

# Why I Built This

The project started with a simple need: I wanted a reliable daily graph of how many Q-bank questions I was actually completing.

Without that visual record, progress felt vague. Some days felt productive and others did not, but it was difficult to see the difference clearly over time. Once question volume became graphical, the feedback itself became motivating and made study patterns easier to recognize.

I was also deliberately creating a low-distraction study environment. I was already using time-management and distraction-blocking tools, but I wanted something tied directly to the Q-bank workflow — a system that made my own study behavior visible rather than merely recording screen time.

As I used the first question counter, its limitations became obvious. Different Q-bank and assessment workflows behaved differently, counts could be duplicated or missed, and solving questions was not the same activity as reviewing them. Each limitation led to another round of testing, correction, and refinement.

What began as one graph gradually became a broader personal study-analytics system.

---

<details>
<summary><strong>How It Evolved</strong></summary>

<br>

**1. Question progress**  
Reliable question counting and daily visualization made progress measurable.

**2. Solving and review separated**  
Active question-solving and later review became independent workflows with their own analytics.

**3. Focus and break patterns**  
Question totals alone could not explain why some sessions worked better than others, so study and break behavior became part of the system.

**4. Session history**  
Repeated sessions were stored and compared so that patterns across days became visible.

**5. Circadian context**  
Study sessions were placed within time-of-day context to make recurring timing patterns easier to recognize.

Each stage came from a limitation exposed through everyday use rather than from a fixed product specification.

</details>

---

# Built Through Iteration

This project was developed through an **AI-assisted software development workflow**.

I defined the problems, workflows, features, constraints, and desired behavior; used **OpenAI Codex, Gemini, and Claude** to generate and revise implementations; and repeatedly tested the resulting software during real study sessions.

My role centered on:

**problem identification → specification → AI-assisted implementation → testing → failure detection → debugging direction → validation → refinement**

The tools went through dozens of revisions because real Q-bank use continually exposed edge cases that were difficult to anticipate in advance: missed or duplicate counts, differences between workflows, navigation changes, session transitions, timing behavior, and interactions between components.

I do not present this project as software written manually line by line. The work I am showcasing is the combination of **problem definition, system design, AI-assisted development, sustained testing, debugging, and iterative refinement** that turned an initial idea into a tool I could rely on during daily study.

At a high level, the tools are browser-based JavaScript applications combining client-side analytics, visualization, and persistent session tracking.

---

# Personalization

Because this was built for my own study environment rather than as a generic product, I also incorporated selected motivational content and optional elements reflecting my Christian faith.

I have kept that aspect visible because it was part of the authentic system I actually used, rather than something added later for presentation.

---

# Author

**Pranav Krishna Buddhapuram, MS Orthopaedics**  
Orthopaedic surgeon · AI-assisted software development and study analytics  
GitHub: [@doctorpranavb](https://github.com/doctorpranavb)

---

# Project Status & Intellectual Property

This repository is a **portfolio and demonstration case study**.

The working source code and detailed implementation are intentionally kept private. The screenshots and descriptions show the purpose, behavior, and evolution of the system without publishing the implementation required to reproduce it.

No license is granted for reuse, redistribution, derivative implementation, or commercial use.

This is an independent personal project created for my own study workflow. It is not affiliated with, sponsored by, or endorsed by any examination organization or Q-bank provider.

---

**© 2026 Pranav Krishna Buddhapuram. All rights reserved.**
