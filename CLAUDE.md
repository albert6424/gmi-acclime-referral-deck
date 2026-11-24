# General Magick · AI Workflow Automation deck

This repo holds a slide deck for **General Magick Industries (GMI)**, made with Claude as a claude.ai **Slides** artifact. It's a general company deck with one main message: **AI workflow automation as a business solution**. GMI takes the repeat work off teams in companies of every size, then builds what sits around it: AI setup and training, ERP and data, customer message assistants, websites, apps and portals.

| | Deck | Link |
|---|---|---|
| **Current** | "General Magick · AI Workflow Automation", 10 slides. Its files are in `project/`. | https://claude.ai/artifact/4AG7B6ug9bKzNnXzDFsgv9 |
| Backup (v1) | "GMI × Acclime Referral Partnership", 12 slides. Git tag `v1-backup`. | https://claude.ai/artifact/Qa719oAxraohZoRE9rH7vy |

Work only on the **current** deck. The backup deck is kept so the team can always go back to the start. Don't change it unless the user asks.

## First message of a session

When someone opens a session here (for example "hello", "hi", "what is this?"), start with a short, plain-English briefing:

1. What the deck is, with the current link and the backup link.
2. What was done so far (the history below, as 5 to 8 short points).
3. How to change it: ask you to edit a slide, or edit it directly in the browser.
4. What still has to be filled in: the [bracket] gaps listed under Rules.

Then ask what they want to change. Keep it short.

## Slides (current deck)

| # | Slide id | What it shows |
|---|---|---|
| 1 | `cover` | "General Magick Industries" on the Earth-at-night photo, with a general one-line promise |
| 2 | `need` | The need: what we see, what it costs ("far too many hours", highlighted), what we do, plus a 5-step tracker (all circles the same blue): Read → Sort → Draft → Check → Report |
| 3 | `deliver` | What we deliver: six services in ruled columns |
| 4 | `automations` | Five AI automations: document intake, customer messages, HR & payroll, reporting, compliance reminders |
| 5 | `why-gmi` | Claude Partner Network, NVIDIA Inception, 2 hubs, 8 products, office addresses |
| 6 | `products` | Six GMI products: Magick Robotics, GabiGo, Magick Learn, Matji & Co, Magick Tailor, OrgAI |
| 7 | `ai-teams` | Claude setup for every team member, plus AI automation training |
| 8 | `training-demo` | Mock one-screen client pipeline dashboard (all made-up data) |
| 9 | `build-run` | ERP & data (Connect, Clean, Show, Ask) plus websites, apps, customer portals |
| 10 | `close` | "Let's build it together", a general line, and the contact line |

## History: what was done

- **Theme.** The look comes from generalmagickindustries.com: dark navy, Anton titles, Instrument Sans text, blue accent. Notes are in `theme.md` and the images are in `brand/`.
- **v1 decks.**
  - The first version was a GMI × Acclime pitch deck (20 slides, then cut to 12).
  - It was then rewritten as a referral partnership deck for Acclime, which is now the backup (v1).
  - Along the way:
    - "AI automation training" and a mock dashboard slide were added.
    - "Everyday IT" was removed because GMI doesn't offer it, with "Customer portals" in its place.
    - The blue ring around highlighted cards was removed.
    - Simple SVG pictures were drawn for Magick Tailor and OrgAI.
- **v2, the current deck:**
  - It is general, with no Acclime anywhere and "× Acclime" removed from every footer.
  - The cover lost its small "General Magick Industries" header and got general text.
  - The old problem and how-it-works slides were merged into the new **Need** slide.
  - The old services slide was replaced by **What we deliver**.
  - The partnership slide was removed.
  - The closing slide was kept at the end, with its Acclime line made general.
  - New order: cover, need, deliver, automations, why GMI, products, AI setup and training, dashboard, data and build, close.
- **Browser edits.** The owner edited some text directly in the browser, for example the cover title and the law-firm version of the dashboard example.

## Rules

- **No IT support.** Never list "everyday IT" or IT support as a GMI service.
- **General audience.** This deck is general, so don't name Acclime or any other partner unless the user asks.
- **Every company size.** Write for companies of every size and type. Don't say "new and growing companies" or anything that limits the audience.
- **Keep the GMI look.** Use the classes in `project/deck.css`, with no new colors or fonts. Don't add blue rings or borders to cards.
- **Nothing invented.** Never invent statistics, clients or quotes. Mock data must stay labeled "mock data".
- **Missing figures.** If a slide needs a number you don't have, put a [bracket] placeholder in its place and tell the user. Don't make one up.
- **Wording.** Use the typographic apostrophe `’` in slide text.

## How to edit the deck

The deck is a claude.ai Artifact of type "Slides". Its files are:

- `project/deck.json`: title, slide order and sections
- `project/deck.css`: the shared style for every slide
- `project/slides/<id>.html`: one `<section id="<id>">` per slide, with speaker notes in the last `<aside>`

Steps:

1. **Read the live deck first.** Someone may have edited it in the browser. Use the Artifact tool with action `read`, the current deck link and `paths` for the files you will change, then make the same changes in `project/` so git stays current.
2. **Edit** the files in `project/`.
3. **Publish only the changed files.** Use Artifact `publish` with `url` = https://claude.ai/artifact/4AG7B6ug9bKzNnXzDFsgv9, `root` = this repo's folder, `file_path` = one changed file, and `files` = the other changed files (keys like `project/slides/need.html`). Send `project/deck.json` only when the title, the slide order or the sections change.
4. **Commit** the change to git with a clear message.

### Making another safe version

Before a big rework, keep the current deck as a backup and do the work on a new copy:

1. Tag the repo with `git tag -a vN-backup`.
2. Create a new deck from the Slides type: run Artifact `quickstart` with intent `slides`.
3. Copy the images from the current deck to the new one: Artifact `publish` with `asset: true`, `from_url` and `asset_ids`.
4. Swap the `/_blob/<id>` links, publish all files, then update this file and `images.md`.

### Edit access

The decks belong to the owner's claude.ai account. To publish to the same link, the owner has to share the deck with **edit** access (Share menu on the deck). If a publish is refused for lack of access, make a copy under your own account the same way as above, uploading the images from `brand/` instead of copying them, and tell the user the new link.

## Images

Slides show images as `/_blob/<id>` links, and those only work inside their own deck. `images.md` lists which local file in `brand/` each id is.
