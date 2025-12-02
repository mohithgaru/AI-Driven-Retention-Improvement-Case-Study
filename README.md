# AI-Driven-Retention-Improvement-Case-Study
# AI-Driven Retention Strategy for a Music + Video Streaming App  
### A Product Management Case Study by Mohith Pulavarthi

![Cover](assets/cover-banner.png)

<p align="center">
  <img src="https://img.shields.io/badge/domain-music_+_video_streaming-blueviolet" />
  <img src="https://img.shields.io/badge/focus-retention_&_activation-brightgreen" />
  <img src="https://img.shields.io/badge/role-product_/_apm-important" />
  <img src="https://img.shields.io/badge/type-self_initiated_case_study-informational" />
</p>

<p align="center">
  <a href="#-project-overview">Overview</a> •
  <a href="#-problem--context">Problem</a> •
  <a href="#-funnel--metrics">Funnel</a> •
  <a href="#-solution-architecture">Solutions</a> •
  <a href="#-visuals--wireframes">Visuals</a> •
  <a href="#-execution--roadmap">Execution</a> •
  <a href="#-how-to-read-this-as-a-hiring-manager">For Hiring Managers</a>
</p>

---

## 🔖 Project Snapshot

> **Goal:** Redesign the **first-week experience** of a **music + video streaming app** to improve **Week-1 retention** using better onboarding, faster personalization, and habit-focused design.  

**Type:** Self-initiated Product Case Study (assumption-driven)  
**Domain:** Consumer App • Music & Video Streaming • Retention & Activation  
**Role:** Student targeting Product / APM roles  
**Timeline:** ~4–6 weeks (part-time)  
**Artifacts:** Case study (PDF), journey diagrams, wireframes, funnel model, experiment plan, 12-week roadmap

---

## 🎯 Project Overview

Most streaming apps (music or video) lose the majority of new users **within the first week**, often during the **first session** itself. New users typically:

- see a generic homepage with random mixes/playlists/rows  
- sample 1–2 tracks or videos, then churn  
- never like / save / follow anything  
- rarely return on Day-1  

This case study explores:

1. **Where new users drop off** in the first week  
2. **Which behaviors predict retention** (especially activation events)  
3. **What product changes can realistically improve Week-1 retention** for a junior PM scope  

The work is **assumption-driven** (no internal company data), but follows realistic funnels and PM decision patterns. :contentReference[oaicite:1]{index=1}  

---

## 🧠 Problem & Context

> “How can we redesign the first-week experience so that more new users actually come back and become retained users?”

I modeled a generic streaming product that supports:

- **Music:** songs, audio tracks, playlists  
- **Video:** episodes, clips, short-form or long-form content  

### Baseline assumptions (for a new-user cohort of 100):

- **Day-1 retention:** ~22%  
- **Week-1 retention:** ~18%  
- **Activation rate:** ~25%  
  - Any meaningful action: like / save / follow / add to playlist / add to watchlist  
- **First-play or first-watch completion:** ~28–30%  
- **Homepage → first-click:** ~45%  

Key observation:  
Most users churn **before the product learns anything about their tastes**, so personalization never becomes powerful.

---

## 📊 Funnel & Metrics

### New-User Funnel (Assumed)

| Stage                                         | Users Remaining | Notes                                                |
|-----------------------------------------------|-----------------|------------------------------------------------------|
| Install → Signup                              | 100             | Starting cohort                                     |
| Signup → Homepage load                        | ~70             | 30% lost to friction / low intent                   |
| Homepage → First content click (play/watch)   | ~45             | Generic homepage, decision overload                 |
| First click → First play/watch completion     | ~28             | Irrelevant first item → skips → exits               |
| Completion → Activation event (engagement)    | ~25             | Like / save / follow / playlist or watchlist add    |
| Activated → Day-1 return                      | ~22             | Weak or no return trigger                           |
| Day-1 → Week-1 retained                       | ~18             | Habit never forms                                   :contentReference[oaicite:2]{index=2}  

**Key drop-offs:**

- **Signup → Homepage**: cold-start + UX friction  
- **Homepage → First completion**: low relevance on first content  
- **Completion → Activation**: users consume but do not invest (no like/save/follow)

---

## 💡 Key Insights

From user behavior patterns and the funnel, I derived several insights: :contentReference[oaicite:3]{index=3}  

- **The first 10–20 minutes decide retention**, for both music and video.  
- **Personalization must start before the homepage**, not “after a few plays.”  
- **Activation (like / save / follow / watchlist)** is the strongest predictor of retention.  
- **Day-1 return** is the key habit moment; if users don’t come back next day, they almost never return later.  
- Most churn happens **before users even feel what the product can do** (they bounce at generic, overwhelming entry points).

These insights shaped the solution architecture.

---

## 🧩 Solution Architecture

Rather than proposing many scattered ideas, I focused on **three product bets** that work together across music and video:

1. **Fast Personalization Layer (Onboarding Taste Picker)**  
2. **Smart First Play/Watch Pathway (Activation-Focused)**  
3. **Day-1 Habit Starter (Personalized Return Trigger)** :contentReference[oaicite:4]{index=4}  

---

### 6.1 Fast Personalization Layer  
**(Taste Picker + Smart First Feed)**

**Problem:**  
New users land on a generic home screen full of categories like “Top Hits”, “Trending Now”, “Popular Shows”, or random carousels. It causes:

- choice overload  
- low relevance  
- poor first clicks  
- quick churn  

**Idea:**  
A lightweight **Taste Picker** immediately after signup, before homepage:

- Languages (for music + content audio)  
- Genres (music genres, show categories, video types)  
- Optional moods / activities  
- 1–2 favorite artists or creators (musicians, channels, or shows)  

**Why it helps:**

- Warmer first homepage (both music and video rows feel personalized)  
- Higher first-click probability  
- Better chance of a relevant first play or watch  
- Stronger trust in recommendations  

**Scope:**  
Rules-based personalization (tags + metadata), no complex ML required — realistic for junior PM teams.

---

### 6.2 Smart First Play/Watch Pathway  
**(Activation-Focused Microflow)**

**Problem:**  
Even if users click something, they often:

- skip within 10–15 seconds (song or video)  
- watch one item and leave  
- never like / save / follow / add to watchlist  

Without activation:

- personalization can’t improve  
- library / watchlist stays empty  
- notifications remain generic  
- there’s no reason to return  

**Idea:**  
After a user **fully completes** their **first track or video**, show a **one-time, low-friction prompt**:

1. “Did you like this?” ❤️  
2. If *Yes* → “Add to Library / Watchlist?”  
3. Then → “Follow this artist / channel / show?”  

**Why it helps:**

- Increases meaningful actions early  
- Feeds personalization for both music and video  
- Builds emotional connection (“this is my stuff”)  
- Enables more relevant future recommendations & notifications  

**Student realism:**  
This is a UX / flow-layer change with clear metrics and minimal engineering lift — perfect for an APM-level project.

---

### 6.3 Day-1 Habit Starter  
**(Personalized Return Trigger)**

**Problem:**  
Day-0 → Day-1 drop-off is huge.  
If users don’t open the app the next day, they rarely come back later.

**Idea:**  
Create a simple but powerful **Day-1 return system** that works across music and video:

- **Notification examples:**
  - “Your mix based on yesterday’s listening is ready.”  
  - “Continue watching *[Show Name]* from where you left off.”  
  - “New episodes and tracks based on what you liked yesterday.”  

- **In-app Day-1 surface:**
  - “Continue where you left off” strip (music + video)  
  - “Your Day-1 Mix” row: tracks, videos, or episodes generated from Day-0 behavior + Taste Picker.

**Why it helps:**

- Closes the loop between Day-0 and Day-1  
- Reinforces a habit loop: trigger → action → reward  
- Makes the app feel responsive and alive  
- Directly pushes Week-1 retention upwards  

---

## 🎨 Visuals & Wireframes

Suggested `assets/` folder structure:

```text
assets/
  ├── cover-banner.png            # Hero graphic for the repo
  ├── journey-current.png         # Diagram 1 – Current first-session journey (music+video)
  ├── journey-improved.png        # Diagram 2 – Improved first-session journey
  ├── activation-flow.png         # Diagram 3 – First play/watch activation microflow
  ├── retention-loop.png          # Diagram 4 – First-week retention loop
  ├── wf-taste-picker.png         # Wireframe – Taste Picker onboarding
  ├── wf-first-play.png           # Wireframe – Player screen + prompt (music & video)
  └── wf-day1-return.png          # Wireframe – Day-1 home with "Continue" + mix rows

Contact

If you’d like to discuss the project or collaborate:
LinkedIn: (add your link)
Email: mohithpulavarthi@gmail.com


Time line of this project: 6 weeks
<img width="794" height="731" alt="image" src="https://github.com/user-attachments/assets/041acb27-dc5f-4d4d-be5a-fabb257e7269" />
