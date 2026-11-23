# GMI × Acclime Referral Partnership deck

This repo holds one slide deck for **General Magick Industries (GMI)**, made with Claude as a claude.ai **Slides** artifact. The deck offers **Acclime** a referral partnership. Acclime sets up and runs companies in Thailand: company setup, accounting, payroll and compliance. The main message is GMI's **AI workflow automation as a business solution**, with AI setup and training, ERP and data work, websites, apps and customer portals around it.

- **Deck:** "GMI × Acclime Referral Partnership", 12 slides
- **Link:** https://claude.ai/artifact/Qa719oAxraohZoRE9rH7vy
- **Local copy:** `project/`

## First message of a session

When someone opens a session here (for example "hello", "hi", "what is this?"), start with a short, plain-English briefing:

1. What the deck is, with the link.
2. What was done so far (the history below, as 5 to 8 short points).
3. How to change it: ask you to edit a slide, or edit it directly in the browser.
4. What still has to be filled in: the [bracket] gaps listed under Rules.

Then ask what they want to change. Keep it short.

## Slides

| # | Slide id | What it shows |
|---|---|---|
| 1 | `cover` | GMI × Acclime title on the Earth-at-night photo: "One referral, two services" |
| 2 | `problem` | The admin problem, then the AI solution: Read · Sort · Draft · Check · Report |
| 3 | `how` | Map → Build → Approve, plus why it matters to Acclime |
| 4 | `automations` | Five AI automations: document intake, customer messages, HR & payroll, reporting, compliance reminders |
| 5 | `offer` | "Workflow automation at the core": six services Acclime can refer |
| 6 | `ai-teams` | Claude setup for every team member, plus AI automation training |
| 7 | `training-demo` | Mock one-screen sales pipeline dashboard (all made-up data) |
| 8 | `build-run` | ERP & data (Connect, Clean, Show, Ask) plus websites, apps, customer portals |
| 9 | `why-gmi` | Claude Partner Network, NVIDIA Inception, 2 hubs, 8 products, office addresses |
| 10 | `products` | Six GMI products: Magick Robotics, GabiGo, Magick Learn, Matji & Co, Magick Tailor, OrgAI |
| 11 | `partnership` | What each side brings, plus 4 referral steps (the blue cards) |
| 12 | `close` | "Let's build it together" and contact line |

## History: what was done

- **Theme.** The look comes from generalmagickindustries.com: dark navy, Anton titles, Instrument Sans text, blue accent. Notes are in `theme.md` and the images are in `brand/`.
- **Origin.** The deck started as a 20-slide pitch deck (kept separately, not in this repo). It was cut to 12 slides with nothing dropped, then copied and rewritten as this referral partnership deck with AI workflow automation first.
- **Training slides.** "AI automation training" was added: hands-on Claude coaching so a client's own staff build dashboards, trackers and reports without code. Slide 7 is a mock dashboard based on a sales pipeline screenshot. Every name and number on it is made up and the slide says "mock data".
- **No IT support.** "Everyday IT" was removed everywhere because GMI does not offer it. Slide 8 has a "Customer portals" card in its place.
- **Card styling.** The blue "active" ring around highlighted cards was removed. Only the 4 "How referrals work" cards on slide 11 are blue (class `blue`).
- **Last slide.** The next-step cards were removed. The next steps are now only in its speaker notes.
- **Product pictures.** Magick Tailor and OrgAI had no usable images, so they have simple made-up SVG drawings.
- **Browser edits.** The owner edited some text directly in the browser, for example the contact email on the last slide and the law-firm version of the dashboard example.

## Rules

- **No IT support.** Never list "everyday IT" or IT support as a GMI service.
- **Keep the GMI look.** Use the classes in `project/deck.css`, with no new colors or fonts. Don't add blue rings or borders to cards.
- **Nothing invented.** Never invent statistics, clients or quotes. Mock data must stay labeled "mock data".
- **Open terms stay in [brackets]** until the owner gives real values:
  - referral fee `[__%]`
  - payment timing
  - client contact owner
  - workflow review `[free / fee]`
  - reply time `[__] days`
- **Wording.** Use the typographic apostrophe `’` in slide text.

## How to edit the deck

The deck is a claude.ai Artifact of type "Slides". Its files are:

- `project/deck.json`: title, slide order and sections
- `project/deck.css`: the shared style for every slide
- `project/slides/<id>.html`: one `<section id="<id>">` per slide, with speaker notes in the last `<aside>`

Steps:

1. **Read the live deck first.** Someone may have edited it in the browser. Use the Artifact tool with action `read`, the deck link and `paths` for the files you will change, then make the same changes in `project/` so git stays current.
2. **Edit** the files in `project/`.
3. **Publish only the changed files.** Use Artifact `publish` with `url` = https://claude.ai/artifact/Qa719oAxraohZoRE9rH7vy, `root` = this repo's folder, `file_path` = one changed file, and `files` = the other changed files (keys like `project/slides/offer.html`). Send `project/deck.json` only when the title, the slide order or the sections change.
4. **Commit** the change to git with a clear message.

### Edit access

The deck belongs to the owner's claude.ai account. To publish to the same link, the owner has to share the deck with **edit** access (Share menu on the deck). If a publish is refused for lack of access:

1. Make a copy under your own account: run Artifact `quickstart` with intent `slides` and create a new deck from the Slides type it gives.
2. Upload the images from `brand/` (see `images.md`).
3. Replace the old `/_blob/<id>` links in the slides with the new ones.
4. Publish all files to the new deck and tell the user the new link.

## Images

Slides show images as `/_blob/<id>` links, and those only work inside this deck. `images.md` lists which local file in `brand/` each id is.
