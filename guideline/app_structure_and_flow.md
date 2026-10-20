# AGAPE App — Structure, Flow & Features

**Last updated:** 2026-10-21

This document describes the full structure of the AGAPE Bible & Prayer app for Eastern Orthodox, Oriental Orthodox and Catholic users.

## Core Concept
- One app that adapts based on the chosen church tradition.
- Default language: **English**. User can switch to **Dutch**.
- Three visual styles, each with light + dark mode.
- Offline-first where possible.

## Onboarding Flow (first launch)
1. Intro video/screen (handled separately by developer)
2. Welcome to AGAPE + short explanation
3. Accept terms & conditions
4. Choose church:
   - Eastern Orthodox
   - Catholic
   - Oriental Orthodox
5. Choose visual style (3 styles, each with light/dark)
6. Login / Sign up
7. Post-signup guided tour (user taps each main area and receives explanation)
8. On Prayer screen: extra explanation + prompt to enable notifications for prayer times and inactivity reminders

## Main Navigation (Bottom Bar — 4 tabs)

### 1. Home
- Verse / text of the day (tradition-specific)
- Continue reading (last position)
- Reading plan status (start new or continue existing)
- Quick access to Bible, Prayer, Bookmarks
- Optional: Saint of the day

### 2. Bible
- Book list adapted to chosen tradition (including deuterocanonical books where applicable)
- Old Testament / New Testament filter
- Church section: history, councils, fathers, explanations
- Verse view:
  - Commentary / explanation
  - Cross-references
  - Links to saints/fathers who spoke about the passage
  - Bookmark, highlight, share
- Quiz at end of chapter or reading-plan day (must pass to continue in plans)

### 3. Prayer (center tab)
- Current hour of prayer (Agpeya / Horologion / Liturgy of the Hours depending on tradition)
- Tap to start praying that hour
- Full list of prayer hours and additional prayers
- First-time explanation of the prayers
- Notification permission prompt (prayer times + inactivity)
- Favorites and reminders

### 4. Me / Profile
- Streaks (consecutive days)
- Medals / achievements
- Activity history (readings, highlights, prayers)
- Saved items (verses, notes, plans)
- Settings (language, style, church, notifications)
- Help, feedback, donation
- Sign out

## Key Features
- Reading plans (including beginner-friendly and redemptive-historical plans)
- Council reading plans (Bible passages + council context, canons summary, why the council happened, outcome)
- Quizzes after chapters or plan days
- Saint of the day
- Per-verse commentary and cross-references
- Offline support
- Notifications for prayer times and inactivity

## Council Reading Plans
Special reading plans that connect Scripture with the Ecumenical Councils (up to 1054 and beyond depending on tradition).

Example structure per council (e.g. Nicaea 325, Constantinople 381, Ephesus 431, Chalcedon 451):
- Relevant Bible passages
- Short historical reason the council was called
- Key canons (summary)
- Outcome for the Church
- Optional quiz

Plans can be filtered by tradition (Eastern Orthodox / Catholic / Oriental Orthodox) because recognized councils differ.

## Languages
- Default: English
- Available: Dutch

## Visual Styles
Three styles, each with light and dark mode:
1. Modern navy + cream
2. Classic sacred (parchment + burgundy/gold)
3. Warm terracotta + beige

---

This document is the single source of truth for app structure and user flow.