# 🐦 Chirp English

*A fictional social media feed for casual English reading practice.*

## About This Project

Chirp English is a small, personal English-learning experiment inspired by social media timelines.

Read short English posts, follow fictional characters' everyday lives, and enjoy their conversations and ongoing stories at your own pace. The goal is to make English reading feel less like studying and more like checking a friendly social feed.

**Chirp English is a fictional world.** All characters, accounts, cities, businesses, organizations, posts, conversations, news stories, incidents, weather forecasts, and events are invented for entertainment and language-learning purposes. There are no real users or live social media connections.

## Features

- Short, casual English posts and reply threads
- **Easy** and **Normal** reading levels
- Japanese translations shown on demand
- Fictional characters with profiles, conversations, and stories
- Prewritten interactive choices, player posts, and simulated replies
- Bookmarks and reading-progress tracking
- A **Stories** view for story progress and chapter archives
- Fictional news, weather, local events, and seasonal or time-of-day posts
- A customizable player name, avatar icon, and avatar background color
- Local save-data export and import
- Main post body text size options (Standard, +2px, +4px)
- DM unread badge and short everyday mood posts
- New content can be added through JSON files over time
- Fictional Eastmere city and its neighborhoods introduced in Ver.4.4

## Version History

## Ver.4.5 — Flower Themes, Eastmere Journey & More English 🌼🚆

- Added **Flower Themes**, with **Olive as the default**, plus Rose, Marigold, Mimosa, Nemophila, Lavender, and Cotton. Theme settings are stored in the existing local save object; restoring an older save defaults safely to Olive.
- Flower colors are used for the floating **＋ Post** button, saved 🔖 state, primary action buttons, progress bar, and selected navigation state. Light/dark display mode remains separate.
- Standardized the six bottom navigation icons using **self-contained inline line-art SVG** (in a Lucide-inspired style), without an external runtime icon/CDN dependency. These icons are authored within this project rather than fetched verbatim from a third-party icon distribution. Bottom-right Stats is now **Settings**. In-post translation and reply emoji remain unchanged; the save emoji stays 🔖 in both states.
- A floating **＋ Post** button appears on Feed, remains available while scrolling, and hides in other tabs and the composition screen. On creating a post, the feed scrolls to your new post so its delayed replies can be seen.
- Added a Japanese in-app **guide.html**, accessible from Settings → Help & About. It provides spoiler-free city descriptions and privacy/fiction disclaimers.
- Added **100 new Normal posts** and **100 new Easy posts**, across everyday topics and music, with translations and authored short replies. Normal grows from 216 to **316** posts; Easy grows from 100 to **200** posts.
- Added a **10-part Mika Eastmere trip** story arc (story days 12–21): departure from Bellport, airport, downtown Neonbridge, Willow Lane, Cloverfield, Harmony Street instrument shops, Clara's Brookside concert, riverside conversation, and homecoming. The trip follows the existing Rosie/jazz story progression so the stories don't place Mika on tour and at a Bellport gig at once. Easy text variants and delayed character replies are included. No missed-day skips.
- Existing saved progress, bookmarks, selected avatar, reading history, events and prior story chapters retain their IDs and existing localStorage key. Back up your saved data before upgrading.

### How to update

Upload **all 11 files** from the new ZIP into the same GitHub Pages folder, including the new `guide.html`. Do not rename or remove the JSON files. Existing installed home-screen shortcuts should continue to work. A site refresh may be needed for caching.

### Ver.4.4 — Reading Comfort & Eastmere Introduction 🏙️

- Saved the Feed reading location when switching between bottom tabs, including DMs, Stories, People, and Stats.
- Improved translation/replies click behavior to preserve the current post's place on the screen.
- Restored consistent padding and touch-target sizes for Translate, replies, and Save buttons.
- Made Japanese translation text smaller and less visually prominent than the English post body.
- Prevented the same story/local post from appearing twice as both a fresh post and a newly replied-to post in the same feed section.
- Changed the Stories tab icon from a globe to an open book.
- Introduced **Eastmere**, a fictional train-oriented city inspired by Tokyo, with Neonbridge, Willow Lane, Cloverfield (including Harmony Street instrument shops), and Brookside Concert Hall.
- Added four fictional accounts: Chloe Spark, Daily Wellness, Clara Strings, and Lily Pop, with short Easy variants and new everyday posts.
- The full Eastmere travel story is planned for a later update; no travel storyline is included here.
- Kept the same local save-data key and existing post IDs, so previously saved progress should be retained. Back up before updating.



### Ver.4.3 — More Natural Conversations & Reading

- Fixed a specific rendering bug: array callback indexes were interpreted as a reply flag, causing some full-width posts to lose their normal card layout.
- Renamed **World** to **Stories**, with clearer story progress and chapter access.
- Revised Rosie's opening story: Rosie posts about preparations first, followed by a fictional news article and the restaurant opening.
- Restaurant announcements are hidden until Rosie's Kitchen has opened in the story.
- Added a DM unread indicator in the bottom navigation. A DM is marked read when its conversation is opened.
- Added post body text sizing: Standard, +2px, +4px. This changes main post text only.
- Added a selection of everyday mood posts, with prewritten replies that vary by character and sometimes time of day.
- Added shorter Easy-mode variants for story-event prompts, choices, and responses.
- Added a limited "New replies" resurfacing of earlier story/local posts, for natural rereading practice.

*The application is still an offline-authored fictional social feed, not a real messaging or real-time news service. Some earlier posts remain ordered by archive position rather than exact timestamps.*


### Ver.4.2 — Profile & Layout Improvements

- Added player avatar customization: choose an emoji icon and background color.
- Saved avatar settings with other local progress, including backup/export data.
- Improved horizontal spacing and text layout across feed posts, events, replies, and story views.

### Ver.4.1 — Reading Comfort & Timeline Fixes

- Improved side padding on smaller screens.
- Improved restoration of reading position after post and conversation events.
- Adjusted timeline ordering so newer world activity appears above older posts.
- Corrected a baritone saxophone joke to refer to a giant saxophone, not a tuba.

*Note: Some original posts have no timestamp, so their ordering is approximate rather than a fully accurate chronological timeline.*

### Ver.4.0 — Living World 🌍

- Introduced fictional news, weather, transit, event, animal shelter, and restaurant accounts.
- Added Rosie Pan and **Rosie's Kitchen**, including an opening storyline.
- Added prewritten story arcs, the World view, and story archives.
- Added delayed, simulated replies to make conversations feel more natural.
- Added fictional time-of-day and seasonal posts.
- Added clearer fictional-world notices.

### Ver.3.1 — Reading Progress Improvements

- Improved when posts are marked as read while scrolling.
- Added an option to reset reading history separately by reading level.

## Fictional Content & Important Notices

- **Not real news:** News reports, accidents, announcements, businesses, and public-service updates are fictional and should not be treated as factual reporting.
- **Not real weather:** Forecasts, temperatures, and seasonal events are part of the fictional setting. Do not use them for real-world decisions.
- **Not a live social network:** All character posts, messages, replies, and reactions are prewritten or locally simulated. No real person is responding on the other end.
- **Not an official account or service:** Labels used for in-world news, weather, transport, or businesses refer only to fictional organizations; they do not indicate real-world verification or authority.
- **Not unlimited generated content:** Stories and posts do not continue creating themselves. Additional content must be written and added in future updates.

## Privacy & Saved Data

Chirp English does not require user registration and does not include an app-specific system for collecting personal profiles or messages on a server.

Bookmarks, reading progress, preferences, and story choices are stored locally in your browser or installed web app. They may be lost if browser or site data is cleared, or if you switch browsers, devices, or storage contexts.

Use **Settings → Export save data** to back up your progress before major updates. You can import saved data to restore it.

The website is hosted through GitHub Pages; normal hosting or platform access logs may be handled by its provider. Local browser storage is separate from those hosting logs.

## Updates & Installation

Chirp English is a static website hosted on GitHub Pages. To update it, replace the existing site files with the files from the new version, including any new JSON files. A home-screen shortcut normally continues to open the same website and does not need to be added again.

An updated page may take a little time to appear because of publishing delays or browser caching. Back up saved data before updating as a precaution.

## Disclaimer

This is an independent personal hobby project, not an official social media service, news organization, or weather service. Any resemblance to real people, places, organizations, or events is coincidental.

## 🤖 AI-Assisted Project

Chirp English is a personal English-learning project created with the assistance of ChatGPT (OpenAI).

The concept, features, and creative direction are guided by a human, while AI is used to help develop the application and write fictional content.

All characters, posts, and conversations are fictional. They do not represent real people or actual social media activity.

This project is independent and is not affiliated with, endorsed by, or an official product of OpenAI or any social media platform.


## v4.5.1 — UI polish (2026-10-22)

- Replaced the Settings gear with a centered symmetric SVG shape.
- Mimosa and Cotton use dark gray text for active translation and reply controls, improving contrast.
- Removed the redundant “Choose another post” button; use the floating **＋ Post** button.
- Your own posts now have two independent controls: **Collapse / Expand** for the whole post and **Hide replies / Show replies** for the reply thread. These states persist in local storage and are included in exported saves. New posts initially appear expanded.
- Existing progress, bookmarks, theme choices, reading history and story progress remain compatible with v4.5.
