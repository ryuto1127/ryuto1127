<p align="center">
  <strong>English</strong>
  &nbsp;·&nbsp;
  <a href="README.ja.md">日本語</a>
</p>

### Hi, I'm Ryuto 👋

I build AI-native products that start from frictions I've personally run into.

Most of my development happens in conversation with Claude Code — not as delegation, but as a division of labor. Now that implementation speed is no longer the bottleneck, I spend my time on defining the problem correctly, articulating design principles, verifying behavior, and deciding what *not* to build. What ultimately determines a product's quality is not the amount of code written, but the quality of the judgment behind it.

#### What I've built

I write about *why it's designed this way*, not just what it does.

🗑️ **[wayste](https://github.com/ryuto1127/wayste)** — An AI waste-sorting kiosk that tells you the right bin the moment you walk up with your trash.

Japan has no national waste-sorting standard: rules differ across roughly 1,700 municipalities. Overseas competitors that hard-code sorting rules can't scale against this fragmentation. wayste separates image recognition (a custom 15-class YOLO dataset, mAP50 ≈ 0.92) from the structured representation of local rules, making "deployable in any town" the center of the design — classification runs 100% on-device in the browser, and no frame is ever sent to a cloud AI. Built in about 2 weeks. Currently seeking pilot sites and partners in Japan. [Homepage](https://wayste.vercel.app/)

📚 **[steadii](https://github.com/ryuto1127/steadii)** — An AI secretary for university students: it connects to Gmail, Calendar, Notion and more, and proactively supports academic life, from email to course information.

The core design principle is *"a secretary, not a tutor."* Instead of a passive AI that answers when asked, it anticipates and delivers what you need — but never acts without your consent. I keep this boundary between initiative and overreach written down as explicit design rules, and when an exception surfaces I edit the rulebook itself rather than bolting on another exception, because a spec that grows by accretion confuses both the AI and the human. Built in about a week; now running as an auth-gated alpha. [Homepage](https://mysteadii.com/)

📝 **[es-canvas](https://github.com/ryuto1127/es-canvas)** — An editor that makes a student's ES (Japan's make-or-break job-hunting essay) stronger while keeping it in their own words.

Hand your writing to generative AI and you get prose that is polished but belongs to no one. es-canvas answers this by *drawing out* instead of rewriting: it researches your target company, asks follow-up questions to surface strengths you never wrote down, and proposes edits that you accept or reject one at a time. The AI offers options; the human makes the final call — a principle carried down to the unit of UI interaction. Built in about a week. Public demo available (bring your own OpenAI key). [Homepage](https://es-canvas.vercel.app/)

🚨 **[Sonae](https://github.com/WhiteStoneTak/Sonae)** — An offline disaster-response platform that assigns every citizen a personal AI agent. Built in about a week for the AMD Hackathon 2026 (Track 3: Vision & Multimodal AI).

Instead of broadcasting the same warning to 100,000 people, it returns an action plan tailored to each person's location, physical condition, and family — with 8,000 agents reasoning in parallel on a single AMD MI300X, showing that "personal disaster response" is computationally realistic. [Live demo](https://sonae-visitor-lp.vercel.app/)

📖 **[CEFR Reading Assistant](https://github.com/ryuto1127/smart-vocab-reader)** — A Chrome extension: select any English text while reading, and it shows meaning cards right on the page — only for words at or above your CEFR level.

Born from my own frustration of losing reading focus every time I opened another tab for a dictionary. Live on the Chrome Web Store (v4.0.1). [Install](https://chromewebstore.google.com/detail/cefr-reading-assistant-%E2%80%93/eplnkcihpoimjahabgdikemnfknlpcof)

#### What I'm learning from building with AI

- **The faster implementation gets, the more a sloppy problem definition shows.** AI will happily build "something plausible" from a vague instruction, so unless you articulate up front what success looks like and how it could fail, you just move faster in the wrong direction. That is why I spend the most time, before implementation, putting user flows, expected behavior, and failure patterns into words.
- **Improve instructions to AI by editing, not appending.** Pile on exceptions and your instructions will eventually contradict themselves. Operating steadii taught me that rewriting the rulebook itself when something breaks is what actually works.
- **Where you draw the autonomy boundary becomes the product's personality.** On the same foundation models, the differentiator is the line between what the AI does on its own and where it hands judgment back to the human. es-canvas's "approve each suggestion one by one" and steadii's "anticipate but never overstep" are both experiments in drawing that line.

#### Background

From Chiba, Japan. Spent the first year of high school at **Chiba Prefectural Chiba High School** (a top public high school in Japan), then moved to Vancouver, Canada, and graduated from high school there. Joining the **University of Toronto** in September 2026 to study **Computer Science**. Outside of tech, I'm into vintage clothing and streetwear.

#### Reach me

📫 ryuto.2007.11.27@gmail.com
