# AGAPE App — Complete Claude Prompt

Copy everything below and paste it into Claude together with the style images from this folder.

---

You are an expert mobile app developer and UX designer. You are building a cross-platform (Android + iOS) Bible and prayer application called AGAPE.

AGAPE is a sacred, tradition-aware Bible and prayer app designed specifically for three Christian traditions:
1. Eastern Orthodox
2. Oriental Orthodox
3. Catholic

The app adapts its content (Bible books, prayers, saints, calendars, reading plans, councils) based on the tradition the user selects during onboarding.

==================================================
IMPORTANT: GITHUB REPOSITORIES
==================================================
There are two existing repositories:

1. AGAPE app code:
   https://github.com/gabriel360110l/AGAPE-Android2.0

2. Reference & guidelines:
   https://github.com/gabriel360110l/EOC-church

You may look at both repositories.

You are allowed to delete, replace, or completely restructure anything that is outdated, incomplete, or no longer matches the final design described below.
The goal is that the final code and documentation fully follow the structure, navigation, onboarding, and features defined in this prompt.

==================================================
CORE PRINCIPLES
==================================================
- Default language on first launch: English
- User can switch to Dutch at any time
- Three visual styles, each with Light mode and Dark mode
- Offline-first: as much content as possible must work offline after initial download
- Clean, calm, readable, and professional (must not look like a generic AI-generated app)
- Account required for streaks, progress sync, quizzes, and reading plans
- No intro video handling needed (developer will handle the very first intro separately)

==================================================
ONBOARDING FLOW (FIRST LAUNCH)
==================================================
1. (Developer handles) Intro / opening experience
2. Welcome to AGAPE screen with short explanation of the app
3. Terms & Conditions screen — user must accept
4. Choose Church / Tradition:
   - Eastern Orthodox
   - Catholic
   - Oriental Orthodox
5. Choose Visual Style (user picks one of the three styles below; each style has Light + Dark)
6. Login / Sign Up screen (must look beautiful and match the chosen style)
7. After successful login: Guided tour
   - User is taken through the main areas
   - On each tab/section they tap, a clear explanation appears of what that area does
8. When the user reaches the Prayer tab for the first time:
   - Extra explanation about the prayers / hours of prayer
   - Strong prompt to enable notifications
   - Notifications are used for:
     a) Prayer times / hours
     b) Reminder if the user has not opened the app for a while

==================================================
VISUAL STYLES (3 STYLES, EACH WITH LIGHT + DARK)
==================================================
Style 1 — Modern Navy + Cream
- Soft cream / warm off-white background
- Deep navy blue for text and accents
- Subtle gold details
- Clean, contemporary, elegant

Style 2 — Classic Sacred
- Parchment / ivory background
- Bordeaux / deep red + gold accents
- Traditional, reverent, Byzantine-inspired feel

Style 3 — Warm Terracotta
- Soft warm beige / cream background
- Terracotta and soft gold accents
- Inviting, calm, approachable

==================================================
IMPORTANT — ABOUT THE REFERENCE IMAGES
==================================================
I am uploading multiple screenshots.

Do NOT copy these screens exactly.

These images are only meant as STYLE and COLOR references for the 3 visual styles of the app.

What you should take from the images:
- Color palettes
- Overall mood and atmosphere
- Typography feeling (serif vs clean)
- Level of decoration and elegance
- Light vs dark versions

What you should NOT copy:
- The exact layout of the screens
- The bottom navigation (it is often wrong in the images)
- The exact placement of cards and buttons
- Any specific icons or illustrations

The correct app structure is defined below:
- Exactly 4 bottom tabs: Home → Bible → Prayer → Me
- The features and flows described in this prompt

Use the images only to understand the visual direction of the 3 styles.
Create clean, professional screens that follow the real app structure, while matching the color and style feeling of the uploaded images.

==================================================
MAIN NAVIGATION (BOTTOM TAB BAR — EXACTLY 4 TABS)
==================================================

1. HOME
   - Verse / Text of the Day (tradition-specific)
   - “Continue Reading” card (shows last place the user left off)
   - Reading Plan card (start a new plan or continue an active one)
   - Quick access buttons (Bible, Prayer, Bookmarks, etc.)
   - Optional: Saint of the Day card

2. BIBLE
   - Book list that changes based on the chosen tradition (includes deuterocanonical books where applicable)
   - Clear filters: Old Testament / New Testament
   - Separate “Church” section containing:
     - Church history
     - Councils and canons
     - Church Fathers
     - Tradition-specific explanations
   - Bible Reader:
     - Clean, highly readable text
     - Tap a verse to see:
       - Commentary / explanation
       - Cross-references
       - Links to saints or Church Fathers who spoke about that passage
     - Bookmark, highlight, share
   - Quizzes:
     - After finishing a chapter or a day of a reading plan
     - User must pass the quiz to continue in locked reading plans

3. PRAYER (CENTER TAB)
   - Shows the current hour of prayer prominently
   - User can tap the current hour and immediately start praying
   - Full list of prayer hours and additional prayers (Agpeya for Oriental Orthodox, Horologion for Eastern Orthodox, Liturgy of the Hours for Catholic — adapted to the chosen tradition)
   - First-time explanation of the prayers
   - Notification permission prompt (prayer times + inactivity reminders)
   - Favorites and personal reminders

4. ME / PROFILE
   - Streaks (consecutive days of activity)
   - Medals / Achievements
   - Activity history (readings, highlights, prayers, etc.)
   - Saved items (verses, notes, bookmarks, reading plans)
   - Settings:
     - Language (English default + Dutch)
     - Visual style + Light/Dark mode
     - Church / Tradition
     - Notifications
     - Font size
   - Help & Support
   - Feedback
   - Donation link
   - Sign out

==================================================
KEY FEATURES
==================================================
- Reading Plans
  - Beginner-friendly plans that build step by step
  - Redemptive-historical plans that link Old Testament and New Testament
  - Full Bible plans (1 year, 2 year, chronological)
  - Council Reading Plans (special plans that connect Bible passages with Ecumenical Councils)
- Quizzes after chapters or plan days (progression lock)
- Saint of the Day
- Per-verse commentary, cross-references, and Church Father links
- Offline support
- Notifications for prayer hours and inactivity
- Account system for progress, streaks, and sync

==================================================
COUNCIL READING PLANS
==================================================
Special reading plans that combine Scripture with the great Councils.

For each council (examples: Nicaea 325, Constantinople 381, Ephesus 431, Chalcedon 451, and others up to 1054 depending on tradition):
- Relevant Bible passages
- Short historical reason why the council was called
- Summary of the most important canons
- Outcome for the Church
- Optional quiz at the end

Plans can be filtered by tradition because the list of recognized councils differs between Eastern Orthodox, Catholic, and Oriental Orthodox.

==================================================
LANGUAGES
==================================================
- Default: English
- Additional: Dutch

==================================================
TECHNICAL & UX REQUIREMENTS
==================================================
- Cross-platform: Android + iOS
- Smooth, professional, non-generic design
- Excellent readability
- Clear navigation at all times
- Deep linking to specific verses or prayers
- Offline caching strategy
- Accessibility support (font size, contrast)
- Store-ready (privacy policy, terms, etc.)

==================================================
SUMMARY OF USER FLOW
==================================================
First open → Welcome → Terms → Choose Church → Choose Style → Login/Sign up → Guided Tour → Main App (Home / Bible / Prayer / Me)

==================================================
INSTRUCTION
==================================================
You may examine the existing code in AGAPE-Android2.0 and the documentation in EOC-church.
You are allowed to delete, replace, or restructure anything that does not match this final specification.
Build and document the app so that it fully follows the structure, navigation, onboarding, styles, and features described above.

Confirm you understand the full structure of AGAPE and the freedom to clean up the existing repositories before generating any output.
