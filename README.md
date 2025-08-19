# GPT5

There will be many apps in the repo.

## Blog Posting Area

This repository contains a **single–page application** called **Blog Posting Area**.  The app is delivered as one HTML file (`admin.html`) with embedded JavaScript and CSS.  It provides a UX‑focused space where you can draft, edit and preview blog posts with rich formatting support.

### Features

The application satisfies the above prompt by implementing the following functionality:

* **Large typing area with spell‑check** – The main `textarea` is spacious and uses the browser’s built‑in spelling and grammar checking.
* **Markdown support with live preview** – As you type Markdown in the editor, the content is converted on the fly to HTML using the [marked](https://github.com/markedjs/marked) library and sanitized with [DOMPurify](https://github.com/cure53/DOMPurify).  The preview pane displays headers, lists, code blocks, links and other Markdown elements.
* **Random paragraph generator** – A button inserts a random, neutral paragraph from a predefined set.  This simulates an AI paragraph generator without requiring external services.
* **Countdown animation** – Press “Start Countdown” to see a simple countdown timer animate from 5 seconds down to zero.
* **Snapshot history and chart** – You can save snapshots of your current word count, which are persisted to `localStorage`.  A line chart (powered by [Chart.js](https://www.chartjs.org/)) visualizes how the word count has changed over time.
* **Accessibility and design** – The interface uses a high‑contrast colour scheme, a white background and responsive layout.  Content is keyboard‑accessible and the preview area uses polite `aria-live` updates.


### Original prompt

> Create a single-page app in a single HTML file with the following requirements:
>
> - Name: Blog Posting Area
> - Goal: UX-first Text and media area for blog posting; spelling-checks, markdown, code block, links, post-preview. Best practice solution.
> - Features: Random paragraph AI-generator, error highlighting, live-preview, countdown animation, history chart.
> - The UI should be clean, with high-contrast text and a large typing area. White background.

The `admin.html` file can be opened directly in a browser.  No build step or server is required; all libraries are loaded from public CDNs.
