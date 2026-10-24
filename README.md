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

### Ver.4.6.3 — Reading polish, translation, place names (2026-10-24)
- Changed fictional Bellport → Bellwindport and Cloverfield → Cloverstonemill in displayed data, world descriptions, resident profiles and stories. Existing post IDs and saved progress remain unchanged.
- A post not yet read is labeled **Unread post**, even when it already has replies; separate **Unread replies** / **New replies** markers apply after the original is read.
- Stabilized the returning-replies feed, avoided duplicate cards, and prevented repeatedly showing the same time-of-day item when no new suitable item is available.
- Standard Japanese translation text is **13px for both posts and replies**, adjusted together with the existing Standard / +2 / +4px text-size setting.
- Corrected identified instrument-specific Japanese translations and the generic-you melody example, without changing the authored story or English post text.
- Updated Japanese help text and browser title. Verified original Normal/Easy post sets are preserved.


### v4.6.2.1 — reply-card visibility hotfix
- Fixed a Feed bug where a resurfaced post disappeared immediately after opening its unread replies. The card remains in the current Feed view until the reader presses “Got it ✓” or leaves the Feed.
- Fixed the same issue within the “Unread replies” reading-history filter: opening replies no longer removes a card while it is being read.
- No changes to user save-data format or story progress.


### Ver.4.6.1 — Conversation & Feed polish (2026-10-22)

- Corrected tab navigation so switching from DMs/People/Stories/Settings to Feed no longer accidentally reapplies scroll coordinates from a different screen. Feed position remains recoverable.
- Reassigned **25 Normal + 25 Easy** second replies to different, context-appropriate speakers (with several duplicate lines rewritten). Original post IDs and existing reading progress are preserved.
- Added **58 authored replies** to story episodes. Stories have roughly **3–5 replies** per episode, arriving in stages. Existing replies remain instantly readable; new arrivals briefly show **Typing…** when their reply thread is open.
- Stories are no longer permanently displayed as full-size pinned Feed cards. A compact **Stories · Day N** shortcut remains available. An active story appears within the normal stream and can reappear when new replies arrive; every chapter remains available in Stories.
- Seasonal and time-of-day posts appear interspersed in the normal Feed, not in a permanent top block; posts for the wrong daypart are excluded. The time-of-day selection refreshes when the feed refreshes.
- Ollie's profile icon is now **💡**, distinct from Wise Owl. Added **Good afternoon**, **Good evening** and **I'm home** to the selectable English posts; common greetings appear in time order and carry emoji + Japanese hints **only in the selection list**, never in published English text.
- Previously exported saves remain importable. The user's saved posts, bookmarks, DM choices, and themes are retained. New optional tracking fields do not erase the old storage key.
- Ver.4.7 ideas (more mood phrases, additional avatar icons, residents of Sunvale and Frosthill, and broader choice-based conversations) are *not* part of this minor release.

### Ver.4.6 — A Better Everyday Feed & Harbor Festival ⚓

- Feed reads in smaller groups: **4 posts** at launch and per "More" action. Automatically marks an original post as seen after **1.4 seconds** at 60% visibility, or immediately when its translation/replies/bookmark action is used on Feed. People profiles never auto-mark posts.
- Introduced **Reading history**, including earlier seen posts where available, and a **Continue reading** shortcut to the last feed position. These are separate from bookmark records.
- Player posts now live in a collapsed **My Posts** section with new-reply indicators; they no longer take up the top of the daily feed as separate cards. New messages show a brief typing indicator; existing replies open immediately.
- New DMs are spaced **12 hours** apart rather than 20; DM threads are ordered by latest activity. Replies to selected DM choices still appear after approximately three seconds.
- Updated Marigold (#E07820, white text), Nemophila (#579DD7, white text), Lavender (#9979C7, white text), while keeping Olive as the default and the seven original themes. Bright themes retain readable action text.
- **Story Progress** in Settings allows manual day rescue, preserving reading history and bookmarks but not reconstructing lost DM choices or posts.
- Added five-part **Bellwindport Harbor Festival** after Mika's Eastmere return (Days 23–27), and introduced **Little English Lab** with eight English-only mini-lessons per reading level, with Japanese shown only on demand.
- Original localStorage key and story/post IDs are preserved. As always, export your save before updating. No live data or genuine real-time AI replies.


## Ver.4.5 — Flower Themes, Eastmere Journey & More English 🌼🚆

- Added **Flower Themes**, with **Olive as the default**, plus Rose, Marigold, Mimosa, Nemophila, Lavender, and Cotton. Theme settings are stored in the existing local save object; restoring an older save defaults safely to Olive.
- Flower colors are used for the floating **＋ Post** button, saved 🔖 state, primary action buttons, progress bar, and selected navigation state. Light/dark display mode remains separate.
- Standardized the six bottom navigation icons using **self-contained inline line-art SVG** (in a Lucide-inspired style), without an external runtime icon/CDN dependency. These icons are authored within this project rather than fetched verbatim from a third-party icon distribution. Bottom-right Stats is now **Settings**. In-post translation and reply emoji remain unchanged; the save emoji stays 🔖 in both states.
- A floating **＋ Post** button appears on Feed, remains available while scrolling, and hides in other tabs and the composition screen. On creating a post, the feed scrolls to your new post so its delayed replies can be seen.
- Added a Japanese in-app **guide.html**, accessible from Settings → Help & About. It provides spoiler-free city descriptions and privacy/fiction disclaimers.
- Added **100 new Normal posts** and **100 new Easy posts**, across everyday topics and music, with translations and authored short replies. Normal grows from 216 to **316** posts; Easy grows from 100 to **200** posts.
- Added a **10-part Mika Eastmere trip** story arc (story days 12–21): departure from Bellwindport, airport, downtown Neonbridge, Willow Lane, Cloverstonemill, Harmony Street instrument shops, Clara's Brookside concert, riverside conversation, and homecoming. The trip follows the existing Rosie/jazz story progression so the stories don't place Mika on tour and at a Bellwindport gig at once. Easy text variants and delayed character replies are included. No missed-day skips.
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
- Introduced **Eastmere**, a fictional train-oriented city inspired by Tokyo, with Neonbridge, Willow Lane, Cloverstonemill (including Harmony Street instrument shops), and Brookside Concert Hall.
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


### Ver.4.5.2 — Contextual conversations fix

- Rewrote replies for all 100 new Normal and 100 new Easy archive posts to respond to the actual post content, not repeating four generic templates.
- Replies now use 30+ individual fictional character voices, including relevant interests and topics, with Japanese translations.
- Original pre-v4.5 archive posts, character conversations, stories, interactions, and all localStorage keys are unchanged. The mood-post reply pools in moods.json have also been rewritten to match each specific mood.
- Note: Older self-posts saved in the browser retain the replies originally saved with them; newly selected self-posts will use the improved moods.json replies.


## Ver.4.5.4 – World & conversations consistency

- Fixed instruments being played by unrelated characters in both Easy and Normal posts; prevented self-congratulatory replies from being attributed to the post author.
- Added 46 contextual second replies per reading level. These may arrive after the post is first shown; earlier posts can appear again when a reply arrives without duplication or changing read IDs.
- Added Ollie, a curious fictional Bellwindport resident, without making their identity a mystery gimmick. Added 12 Ollie posts and 10 grounded Daily Wellness posts in both levels.
- Added five optional DMs, including returning characters. Unread indicators continue to use existing save keys.
- New-post screen is always called “Create a post”; welcome posts are available only before the first player post.
- Preserves localStorage key `chirp-english-v3` and original post IDs. Back up progress before upgrading.


### Ver.4.5.4 (DM pacing and feed variety)
- New eligible DMs arrive one at a time, spaced approximately 20 hours apart. Previously read/completed messages remain accessible. No live background push notifications; messages appear when using the app.
- After replying to a DM, the character's reply appears after about 3 seconds with a temporary "Typing…" indication.
- Redistributed new Ollie and Daily Wellness posts among existing posts so no single account dominates the newest feed batch.
- Preserves all earlier IDs and browser reading/bookmark/story progress.


## Ver.4.6 — A Better Everyday Feed (2026-10-22)

### Comfortable reading
- The initial archive feed batch and subsequent Load more batches contain **4 archive posts** each instead of 7. Story and ambient items are displayed separately.
- A post is automatically marked seen after 60% remains in the feed viewport for **1.4 continuous seconds**. Using Translate, Replies, or Save on a Feed post also marks it seen. Visiting People does not mark it seen.
- **Reading history** stores posts shown in each level (Easy/Normal) for revisiting, without requiring every post to be understood immediately. Existing seen IDs seed the history when upgrading. Use **Continue reading** to return to the last visible archive post. Reading history and seen statistics are distinct.
- Personal posts are collected in **My Posts** at the top of Feed, initially closed. New timed replies earn a red dot and are marked read explicitly with **Mark new replies read**. Existing individual fold controls are retained.

### Conversations & world
- Newly eligible DMs are staggered at approximately **12-hour** intervals, including rescheduling future undelivered queue entries from the v4.5.4 schedule. DM conversations sort by most recent known activity, with unread dots. The existing approx. 3-second DM reply Typing… remains.
- **Only genuinely arriving delayed post replies** get a temporary approx. 3-second Typing… indicator before display. Existing replies and archive rereads open instantly.
- **Bellwindport Harbor Festival** introduces five carefully ordered story episodes starting Story Day **23**, after the Eastmere journey (Days 12–21). The festival includes food stalls, jazz, local games, and visitors from outside Bellwindport. Both levels use English-only post content with Japanese translations available on demand.
- **Little English Lab** is a fictional Bellwindport English school, appearing in 8 dispersed posts per level. The account explains one English word or expression at a time with examples; Japanese appears only in hidden translation text. This is a modest introduction, not a new quiz or required study step.

### Settings & compatibility
- **Story Progress** lets readers manually change their story day (up to Day 90 or the current day, whichever is greater) as an emergency recovery aid. It controls story availability without forging reading history or DM choices. It is **not** a complete save-file restore; export backups as before.
- Revised flower colors: Marigold `#E07820` (white label), Nemophila `#579DD7` (white label), Lavender `#9979C7` (white label). The default remains Olive `#667C3E`. Marigold and Nemophila have less contrast with small white lettering; check legibility on your own screen.
- Existing storage key `chirp-english-v3`, IDs, bookmarks, chosen replies, profile, and theme preferences are retained. Newly introduced storage fields are added without clearing existing data.
- Fictional people, places, institutes, news/weather, promotions and events remain fictional; general wellness and language tips are intended to be grounded and qualified.


## v4.6.2 — reading and reply updates

- Replies have their own unread count independent of post read status. `Unread replies` means never opened; `New replies` means more replies since last opening. Opening the reply button records the currently visible count.
- Previously acknowledged basic-post reply resurfacing is suppressed until genuinely later replies arrive.
- Settings offers a 3–7 post batch size, default 4; it applies to Feed and My Posts.
- My Posts is now a single accordion showing up to one batch of complete posts and replies, with a Load more button. Existing post data is retained.
- Greetings can be posted repeatedly; several character-specific responses are rotated with variety in reply counts.
- Translation correction: `p45-021` retains the library location. Other translations retain a natural Japanese style; a full editorial audit is still recommended.
- The existing `chirp-english-v3` localStorage key is unchanged. Before updating, export your save in Settings.

## Credits and usage / 制作・利用について

**Creator / 制作者:** GitHubリポジトリの所有者（公開名を明記する場合は、この行を編集してください）  
**Development assistance / 制作支援:** ChatGPT (OpenAI)

Chirp Englishは、無料で利用できる架空SNS型の英語学習Webアプリです。アプリのURLの共有や、個人での学習利用を歓迎します。ソースコード、登場人物、文章、ストーリー等の無断転載、再配布、および改変版の公開は原則として許可していません。ただし、法律上認められる利用や、GitHubのサービス利用規約に基づく操作は除きます。オープンソースライセンスは付与していません。第三者の権利が含まれる場合は各権利者の権利を尊重します。

© 2026 Project creator (replace with your public handle if desired).  
All places, people, and organizations in this fictional world are imaginary. Similarity to real-world names does not imply affiliation.
