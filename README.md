# 🐦 Chirp English

**English** | [日本語](README-ja.md)

*A fictional social feed for relaxed English reading practice.*

## About

Chirp English is a free-to-use, personal English-learning web app. Read short posts, replies, fictional local news, and continuing stories from imaginary residents. It is a simulation, **not a real social network**: all accounts, conversations, places, businesses, weather, and events are fictional. Replies are prewritten or simulated locally, not generated in real time by an AI. There are no real users messaging you.

## Features

- Easy and Normal reading modes, with Japanese translations on demand.
- Resident profiles, prewritten reply threads, DMs, story chapters, fictional news, weather, events, and time-of-day posts.
- Your own selectable posts with simulated replies, including an additional reply around one hour after newly created eligible posts.
- Reading history, Continue reading, bookmarks, and saved reading progress.
- My Posts accordion, initially closed, showing three posts at a time.
- Little English Lab: a searchable glossary of expressions appearing in Chirp English ([Open the lab](lab.html)).
- Custom player name, emoji avatar, avatar background, seven Flower Themes, and text-size settings.
- Feed batch-size setting (3–7, default 4) and optional Japanese translations in selectable-post menus.
- Local save export/import; posts, story content, and other authored data are delivered in JSON files.

## Using and updating

Chirp English is a static website intended for GitHub Pages or another static host; a Node.js server is not required to run it. Upload **all 14 files** from the Ver.4.7.2 ZIP together, preserving filenames and relative paths. [Japanese guide](guide.html) is available in the app, with a one-time guide prompt for new users.

Before replacing files, use **Settings → Export save data** to back up your progress. If necessary, restore it with **Import save data**. Reading history, selected posts, profile choices, and other preferences are stored in the browser's localStorage using the existing key `chirp-english-v3`. Clearing site data or changing browsers/devices can lose locally stored progress. Existing exported saves and post/reply IDs are designed to remain compatible. Browser caching or GitHub Pages publishing delays may mean that changes do not appear immediately.

## Version history

### Ver.4.7.2 — My Posts and profile usability (2026-10-29)

- My Posts starts **closed** on launch and sorts by **original post time, newest first**. New replies do not reorder posts.
- Your posts and replies show approximate elapsed-time labels (for example, `just now`, `2h ago`, or `1d ago`) when actual timestamps are available; exact clock times are not shown.
- Tap either a resident's name **or avatar** to view the resident's profile. Your own avatar opens profile settings.
- Corrected two Wise Owl posts about performing/reeds to match the character's role as a music listener.
- The existing save-data key and post/reply IDs are preserved.

### Ver.4.7.1 — Maintenance and reading comfort

- My Posts initially displays **three** entries, with three more per load. Unread-reply indicators are saved after the relevant visible replies have been viewed for approximately 1.4 seconds.
- Feed batch limits now include returning reply threads, stories, and local-life items; already visible posts are not removed when the batch setting changes.
- Added Japanese meanings to all selectable post options and a separate Settings toggle for showing or hiding those meanings (default: shown).
- Newly created eligible selectable posts receive one additional simulated reply around one hour later, including on a later visit; there are no push notifications. Older saved posts do not gain these extra replies.
- Replaced six new avatar choices with 🐿️ 🧁 🍮 🎀 💎 🎵 while preserving previously chosen icons.
- Fixed a new-story badge incorrectly labeled “LOCAL LIFE”; incorporated corrected Normal, Easy, and story reply data.
- Added basic JSON data validation, including schema/ID/length checks. This does not guarantee protection against every attack.
- Kept the existing save-data key and IDs; backing up before upgrading remains recommended.

### Ver.4.7 — Living world and English Lab

- Expanded authored archive posts to **600 Normal** and **400 Easy**.
- Added Gemma Stone (Frosthill) and Sunny Bloom (Sunvale), the Missing Bell mystery, and Gemma's mineral-collecting story.
- Expanded selectable activity/feeling posts and avatar options.
- Introduced the separate searchable [Little English Lab](lab.html) (using `lab.html` and `lab.json`).
- Improved repeat prevention for local-life posts and added fictional city time-zone metadata; Bellwindport follows Japan time.
- Introduced the Japanese README, first-visit guide prompt, translation sizing improvements, and timestamped save-export filenames.

### Ver.4.6 series — Reading progress, Stories, and town events

- Introduced My Posts, Reading history, Continue reading, staged replies, and more consistent unread/new-reply indicators.
- Added Bellwindport Harbor Festival, story progress tools, and standalone Little English Lab lessons within the feed.
- Refined Feed batches, navigation, translation sizing, and reply visibility; changed Bellport to Bellwindport and Cloverfield to Cloverstonemill.
- Improved DM timing, character voices, and restored archival post data where necessary.

### Ver.4.5 and earlier — World building and customization

- Added Flower Themes, avatar customization, the floating Post button, the Japanese guide, and Eastmere's neighborhoods.
- Expanded the fictional world with Rosie's Kitchen, the Eastmere journey, music scenes, news, events, and resident accounts.
- Earlier updates improved layouts, bookmarks, reading, story navigation, and locally saved choices.

## Privacy and safety

Chirp English does not require an account or operate its own server-side user-profile database. Your progress and selected posts are stored locally in your browser. The app is not a live messaging service and does not send real-world push notifications. GitHub Pages or another hosting provider may handle ordinary website access logs. Back up your save before upgrading; local data can disappear if browser or website data is erased. Fictional news, weather, transport information, and locations must **not** be used as real-world information. Basic data validation does not mean the app has undergone a comprehensive security audit.

## Creator and usage

**Created by:** Komugi Midorino (緑野こむぎ)  
**Development assistance:** ChatGPT (OpenAI)

© 2026 Komugi Midorino

Chirp English is free to use for personal English learning, and sharing its website URL is welcome. **No open-source license is granted.** Unauthorized republication or redistribution of source code or authored content, and publication of modified copies, are generally not permitted, except where allowed by applicable law or GitHub's terms. Third-party rights belong to their respective owners. This notice does not claim exclusive copyright in every AI-generated element.

Any resemblance to real people, places, or organizations does not imply affiliation. Chirp English is not affiliated with, endorsed by, or an official product of OpenAI or any real social media platform.
