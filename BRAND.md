# Accrue brand

Version 2.0, 30 October 2026. This is the complete text of the brand book (`accrue-brand-book.html`), page by page, for people and AI assistants. The same rules as structured data are in `brand.json`; colors, type and motion values in `tokens.json`; every file is explained in `assets/index.html`. Where the book shows something visually (the logo, colors, motion, sound), the files in `assets/` are the source.

## Brand at a glance

Open-source billing for Phoenix apps, kept in your own database. Nothing shows as paid until Stripe or Braintree says it is.

### Color

**Ledger Paper** #F3EEDF **Ledger Green** #17392D **Folio** #FBF8F0 **Line Green** #3F8A68 **Column Line** #D8D0BC **Mint Line** #8FCBAA, the double line on dark backgrounds

Paid Pending Failed No update

### Type

Besley for the name and headlines, Public Sans for reading, IBM Plex Mono for code and figures.

### Voice

A careful bookkeeper explaining what happened, in order, with receipts.

### Three rules

1. The name is never shown without its double line.
2. Green means paid, brass means pending, always with the status word.
3. Say what it does, not how good it is.

## Positioning and values

**Open-source billing for Phoenix apps, kept in your own database. Nothing shows as paid until Stripe or Braintree says it is.**

### Elixir and phoenix developers

When I add billing to my Phoenix app, I want subscriptions and payments in my own database, so my app always knows which customers have paid.

Billing that fits a normal Phoenix app, setup in a few Mix commands, and a way to test the whole flow without real payments.

### Evaluators on hex and hexdocs

When I compare billing libraries, I want one that’s easy to start with and safe to depend on for years, so I can commit to it with confidence.

Easy setup, a realistic demo, flexibility for how they bill, and signs of a healthy open-source project.

### Support and billing staff

When a customer asks about a charge, I want to see what happened to it, so I can answer without asking an engineer.

One place in Accrue Admin to look up a customer, see their plan and what they owe, and fix the problem.

### The host app’s customers

When I go to pay my invoice, I want it to look like the company I signed up with, so I know it’s genuine.

The company’s own brand on every email, invoice and billing page, with no mention of Accrue.

**Measured**

Say what Accrue does (“verifies every webhook signature”), not how great it is (“bank-grade”).

**Exact**

Use the real names: the actual module, the actual version, `Accrue.Billing.subscribe/3` rather than “the API”.

**Native**

Speak Elixir: Ecto schemas, contexts, plugs and Mix tasks, used the way Phoenix developers use them.

**Honest**

Pending is not paid. When Accrue doesn’t know, it says so instead of guessing.

**Durable**

Words and design that still hold up in five years: no trends, no dated slang.

## Messaging

### Elevator pitch

**Accrue is an open-source billing library for Elixir and Phoenix. It handles subscriptions, invoices, payments and webhooks inside your app, and comes with a ready-made admin dashboard.**

### Key messages

**In your own database**

Every verified webhook from Stripe or Braintree becomes a record in your own database.

**Never “paid” before it’s paid**

A charge sent to Stripe isn’t a payment yet. Accrue shows Pending until Stripe confirms it, and only then Paid.

**Try it in minutes**

Create a subscription with the test payment processor, send a signed webhook, see it in Accrue Admin, then run `mix verify`.

### Tagline

Paid means paid.

“Paid means paid.” leads where a reader is already on the page (the README, a talk, the website). Where a string is search-indexed or seen out of context (the GitHub description, Hex.pm, the social card), the descriptor leads and the tagline follows. It is never attached to the logo.

### About accrue: approved descriptions

Descriptor (search and social)

The Elixir billing library for Phoenix apps.

Short (about 20 words)

Accrue is an open-source billing library for Elixir and Phoenix: subscriptions, invoices, payments, recovery and webhooks, kept in your own database.

Medium (about 45 words)

Accrue is an open-source billing library for Elixir and Phoenix. Your app keeps its own billing module, routes and auth; Accrue handles the rest: subscriptions, invoices and payments as Ecto schemas, signature-verified webhooks, a full event history, a ready-made admin dashboard and a white-labeled customer portal.

Long (about 85 words)

Accrue is an open-source billing library for Elixir and Phoenix. It keeps subscriptions, invoices, payments, refunds and each customer’s feature access (their entitlements) in your app’s own database, matching what Stripe or Braintree says. Your app keeps its own billing module (`MyApp.Billing`), routes, auth and config. Every webhook is signature-verified and stored, so you never lose a billing event and can always see how an invoice got to where it is. Your team gets a ready-made billing dashboard, and your customers get a billing portal white-labeled with your brand. MIT licensed.

## The idea

**Why a double line under the name**

On invoices, statements and spreadsheets, a double line under a number means it is the final total. Nothing below it changes.

Accrue’s job is to know which charges, refunds and invoices are final. A refund you requested is not final; a refund Stripe has confirmed is. So the logo puts that double line under the name. In the docs, in Accrue Admin and on invoices, the same line marks what is final. No other billing or payments brand uses it.

## Where the brand shows

**Accrue lives inside the apps that use it. The brand knows when to be quiet.**

### Full brand

**Accrue’s own surfaces**

The README and the GitHub repository, HexDocs, Hex.pm, the social card, release posts, talks, stickers and the tee.

**What shows.** The lockup on light and dark, Besley headlines (the brand’s serif), the double line under titles and totals, the logo sound after a click.

### In the background

**Accrue Admin, in the host app**

Support and billing staff, and engineers, investigating billing inside the host app, at a path the host app chooses.

**What shows.** Accrue’s own look by default: the Accrue lockup in the header, its type, background and status colors, Ledger Green for actions. A host app that white-labels it puts its own name or logo in the header instead and sets its own accent color (`:admin_branding`). No sound.

### Host brand only

**Portal, emails and invoices**

The host app’s own customers, who are subscribing, paying and reading invoices.

**What shows.** Accrue designs the templates; the host app’s own name, logo, accent color and font fill them, from its branding settings (`config :accrue, :branding`). The Accrue name and logo never appear.

The host app’s customers have a relationship with the host app, not with a library. Showing them Accrue’s name or logo would be noise at best and a support question at worst.

## Logo: on Ledger Paper

**One color.** Ledger Green on Ledger Paper. In one-color versions, the word and the line use the same color. They are separate pieces that never touch, so the line never has to break around a letter.

**Symbol.** The a with its own double line under it: avatars, the Accrue Admin sidebar, stickers.

**Drawn per size.** 64, 32 and 16 px, each its own drawing.

**Ledger Paper is the default background.** HexDocs, the README and documents show the lockup (word and line) on it. The word and the line are one logo. The line is never shown alone as the logo, and the word is never shown without it.

## Logo: on Ledger Green

**One color.** Ledger Paper on Ledger Green. In one-color versions, the word and the line use the same color. They are separate pieces that never touch, so the line never has to break around a letter.

**Symbol.** The a with its own double line under it: avatars, the Accrue Admin sidebar, stickers.

**Drawn per size.** 64, 32 and 16 px, each its own drawing.

**For dark backgrounds.** On Ledger Green the line turns Mint Line, so it stands out against the background; the word is Ledger Paper.

## Logo: construction

**Wordmark.** accrue, lowercase, in Besley SemiBold (weight 600) with no extra letter spacing, converted to outlines (drawn shapes, not live text). It is a drawing: never typed in the font.

**Double line.** The double line is drawn from the letters: each bar is 100 font units thick (the font’s em is 2,000), the weight of Besley’s thinnest horizontal stroke (the top of the a’s bowl), so it reads as part of the type and not as an underline. The bars are 68 units apart and the first sits 120 units under the baseline; “accrue” has no descenders, so the line can sit close. It runs exactly from the a’s left edge to the e’s right edge.

**Symbol, here at 64 px on its pixel grid.** The symbol is the a alone, with its own double line under it, as wide as the a. It is drawn for each size rather than scaled: at 16, 24, 32, 48 and 64 px the x-height, the baseline, the a’s stem and both lines sit on whole pixels, the a gets a little heavier as it gets smaller (weight 640 at 64 px, 700 at 16), and each line is the a’s thin stroke at that size, rounded to whole pixels.

## Symbol and app tile

The app tile is the symbol on Ledger Green: a Ledger Paper “a” over a double line in Mint Line. Each size has its own drawing, so even the 16 px favicon keeps two distinct 1-pixel lines: they blur only when a large drawing is scaled down, so we never scale one down.

We supply square files. GitHub, Hex and social sites crop avatars to circles and rounded squares themselves; the symbol is centered with room for their crop. Never draw the symbol inside a circle yourself.

## Clear space and minimum size

Keep one x-height (the height of a lowercase x in the wordmark) of clear space on every side of the lockup: no text, page edges or other logos inside it. The line counts as part of the logo.

### Minimum size

|   | Screen | Print |
| --- | --- | --- |
| **Lockup** | 96 px wide | 25 mm wide |
| **Symbol, drawn for its size** | 16 px | 5 mm |

Below 96 px wide each line would be thinner than 1.4 pixels and the two would start to merge; use the symbol instead. Below 64 px always use the symbol file drawn for that size. Print sizes assume offset or good digital printing; check engraving and embroidery with the supplier.

## Logo: misuse

Don’t use the word without the line.

Don’t make the line a single line or blue: it reads as a link.

Don’t change the line’s length.

Don’t put the line through or above the word.

Don’t stretch, slant or outline it.

Don’t lock a tagline to it.

Don’t put it in a box or badge.

Don’t set it on Line Green or coral.

## Logo: on photographs and in others’ hands

### On photographs and screenshots

- On photographs and screenshots, place the lockup on a calm area: a wall, a table top, empty paper.
- Use the light lockup over light areas and the dark lockup over dark ones, with the clear space free of detail.
- If no calm area exists, move the logo off the image onto Ledger Paper or Ledger Green beside it.

- No boxes, badges or blurred panels behind the logo.
- Never over code, tables or figures, where the line reads as an underline.

### When others use our marks

- Hex packages, blogs, newsletters and conference sites may use the lockup and symbol unaltered, from these files, at no less than the minimum sizes.
- In your own writing, write the name as plain text, “Accrue”; never imitate the wordmark.
- Packages that extend Accrue use their own names and marks, and may say “for Accrue”, as in “Tax rates for Accrue”. They don’t use the double line.
- Host apps never put the Accrue logo on their customers’ invoices, emails or Portal, and no “Powered by Accrue” line is needed.
- Don’t use the marks to suggest an endorsement, audit or partnership that doesn’t exist.

## Color: light, the default

**Ledger Paper**

#F3EEDFRGB 243 238 22360% of a surface

The background: warm, never white. Pages, docs, the README banner.

**Ledger Green**

#17392DRGB 23 57 4522% of a surface

The wordmark, all text, buttons and code. A deep bottle green, never black.

**Folio**

#FBF8F0RGB 251 248 24010% of a surface

Raised surfaces: cards, code blocks, Accrue Admin’s panels.

**Line Green**

#3F8A68RGB 63 138 1044% of a surface

The double line and graphics only. At 3.6:1 contrast, never small text.

**Column Line**

#D8D0BCRGB 216 208 1884% of a surface

Hairlines and table lines: the lines of a ledger.

### In use: logo

### Button

Get started

### Link

First hour guide

### Secondary text

Last webhook 2 minutes ago

Pencil #5B6A60

## Color: dark

**Ledger Green**

#17392DRGB 23 57 4562% of a surface

The background in dark mode, on the cover, talks and the social card.

**Ledger Paper**

#F3EEDFRGB 243 238 22322% of a surface

The wordmark and all text: 10.9:1.

**Felt**

#1F4538RGB 31 69 5610% of a surface

Raised surfaces: cards, code blocks, the docs sidebar.

**Mint Line**

#8FCBAARGB 143 203 1706% of a surface

The double line, links and buttons on dark: 6.8:1.

### In use: logo

### Button

Get started

### Link

First hour guide

### Secondary text

Last webhook 2 minutes ago

Sage #A7BCAE

## Color: what it means

**Green means paid. Brass means pending.**

**Paid**

#2E6B4E on light #8FCBAA on dark

Done, in Stripe’s or Braintree’s own words: paid, refunded, active. Shown with the Paid mark, a small double line, beside the word. Paid Ink on light, Mint Line on dark.

**Pending**

#7D5A1F on light #D1A24E on dark

A charge or refund sent to Stripe or Braintree that they haven’t confirmed yet, or a webhook received and not yet applied. Brass Ink on light, Brass on dark.

**Failed**

#A33A2C on light #F0937F on dark

Refused or failed, by Stripe, Braintree or Accrue. Red Ink on light, a lighter red on dark. Bookkeepers’ red, used sparingly.

**No update**

#5B6A60 on light #A7BCAE on dark

Stripe hasn’t sent anything yet, or its last update is old. Pencil on light, Sage on dark, never green or red, because Accrue doesn’t guess.

Every status shows its word. Color and the Paid mark only add to it, so color is never the only signal.

## Color: combinations

**Ledger Green** on **Ledger Paper**: 10.91 : 1

Any text

**Pencil** on **Ledger Paper**: 4.93 : 1

Any text

**Ledger Paper** on **Ledger Green**: 10.91 : 1

Any text

**Ledger Green** on **Folio**: 11.92 : 1

Any text

**Paid Ink** on **Ledger Paper**: 5.44 : 1

Any text

**Brass Ink** on **Ledger Paper**: 5.40 : 1

Any text

**Red Ink** on **Ledger Paper**: 5.66 : 1

Any text

**Line Green** on **Ledger Paper**: 3.59 : 1

Large text (24 px+, or 19 px bold) and graphics only

**Ledger Paper** on **Line Green**: 3.59 : 1

Never for text: see the note

**Sage** on **Ledger Green**: 6.30 : 1

Any text

**Mint Line** on **Ledger Green**: 6.80 : 1

Any text

**Ledger Green** on **Mint Line**: 6.80 : 1

Any text

**Ledger Paper** on **Felt**: 9.21 : 1

Any text

**Brass** on **Ledger Green**: 5.42 : 1

Any text

**Red Ink Light** on **Ledger Green**: 5.53 : 1

Any text

**Mint Line** on **Felt**: 5.74 : 1

Any text

Ratios are WCAG 2.2 contrast ratios computed from these exact values. Line Green is a line color. Ledger Paper text on it reaches only 3.6:1; buttons on light are Ledger Green. These pairs cover the brand’s own surfaces; they don’t certify a host application as accessible.

## Type

### Serif

**Besley**

600 for the name, headlines and titles; 400 italic for quotes and the voice line.

An 1845 Clarendon, the slab serif of ledgers and receipts. No billing library or Elixir project uses it.

### Sans

Public Sans

400 for reading, 500 for leads, 600 for emphasis and labels.

The U.S. Web Design System’s open typeface: easy to read, with no voice of its own.

### Mono

IBM Plex Mono

400 for code, IDs and figures; 500 for a total.

Its figures line up in columns, as a ledger’s should.

### In the product and license

Accrue Admin uses all three. Customer emails and invoices use the host app’s own fonts. All three are free under the SIL Open Font License 1.1, in assets/fonts. Fallbacks: Georgia, the system UI font, ui-monospace.

## Type: the hierarchy

- Display: Besley 600, 72/72 px, tracking −1.5%. Covers, talk titles, the website hero. Sample: “Paid means paid.”
- Headline: Besley 600, 44/48 px, tracking −1%. Guide and section titles. Sample: “Webhooks, verified.”
- Title: Besley 600, 26/33 px, tracking 0. Module names in guides, card titles. Sample: “Payment recovery”
- Quote: Besley Italic 400, 24/32 px, tracking 0. Pull quotes, the voice line. Sample: “Refund requested. Stripe hasn’t confirmed it yet.”
- Lead: Public Sans 500, 21/30 px, tracking 0. The first line under a headline. Sample: “Your app owns `MyApp.Billing`; Accrue does the rest.”
- Text: Public Sans 400, 17/27 px, tracking 0. Guides, READMEs, release notes. Sample: “Every webhook is signature-verified before it touches your database.”
- Emphasis: Public Sans 600, 17/27 px, tracking 0. The phrase that matters most. Sample: “Sending a charge to Stripe is not the same as getting paid.”
- Label: Public Sans 600, 13/16 px, tracking +8%, capitals. Table headers, section labels. Sample: “LAST WEBHOOK”
- Code: IBM Plex Mono 400, 15/23 px, tracking 0. Code, commands, module names. Sample: “mix accrue.install”
- Figures: IBM Plex Mono 400, 15/23 px, tracking 0. Amounts and IDs, right-aligned. Sample: “USD 1,248.00”
- Caption: Public Sans 400, 14/20 px, tracking 0. Figure notes, in Pencil or Sage. Sample: “Shown with the test payment processor and sample data.”

Sizes are for screens at 1×; scale the set together. The wordmark is a drawing and is never typed.

## Layout

**Lines, not boxes.**

For what Accrue designs itself: the README, release posts, social images and slides. On HexDocs, ExDoc sets the page layout; Accrue adds the logo, the colors and code colors, and writes the guides. Accrue Admin follows the “In the product” pages; templates for host apps follow the host app’s brand.

1. **Words left, figures right.** As in a ledger: text aligns to one left edge, and amounts align right in IBM Plex Mono, so figures line up from top to bottom.
2. **Lines divide; boxes don’t.** Sections and rows are separated by Column Line hairlines and space. Cards are for things you can act on, not for every paragraph.
3. **One closing line per surface.** The double line goes under the one thing that is final: the page title, the total, the slide headline. Never two on a surface.

Not set by this book: a website grid or spacing scale (a website build guide is its own document), component states and form specifications (they live in Accrue Admin’s code), and a print grid. Logo placement, clear space and minimum sizes are on the logo pages.

### Readme or guide page

### Conference talk slide

## Voice: the tone dial

**A careful bookkeeper explaining what happened, in order, with receipts.**

- Talks and social posts: 3 of 4 toward lively. “Webhooks arrive out of order. Your invoices shouldn’t.”
- README and the website: 2 of 4 toward lively. “Paid means paid.”
- Release notes: 2 of 4 toward lively. “Webhook replay is safer: two concurrent replays can no longer dispatch the same delivery.”
- Guides on HexDocs: 2 of 4 toward lively. “Send one signed webhook with the test payment processor, then inspect it in Accrue Admin.”
- API reference: 1 of 4 toward lively. “Returns `{:error, :checkout_context_mismatch}` when the fetched session does not match.”
- Accrue Admin: 1 of 4 toward lively. “Retry scheduled. Waiting for Stripe.”
- Errors and warnings: 0 of 4 toward lively. “Refund not sent. The invoice is still a draft.”

The voice never changes; the tone shifts with where the words appear. The closer a message is to money moving, the plainer its language.

## Voice: this, not that

- Say: “Every webhook is signature-verified before it touches your database.” Not: “Bank-grade security.”
- Say: “Refund requested. Stripe hasn’t confirmed it yet.” Not: “Refund processed!”
- Say: “Pull requests are merge-blocked until `mix verify.full` passes.” Not: “Extensively tested.”
- Say: “Retry scheduled. Waiting for Stripe.” Not: “Payment fixed!”
- Say: “Your app owns `MyApp.Billing`; Accrue handles the billing behind it.” Not: “Accrue handles everything for you.”
- Say: “Pay and Laravel Cashier showed the way. Accrue brings it to Phoenix.” Not: “The modern alternative to Pay.”
- Say: “Elixir 1.19+, Phoenix 1.8+.” Not: “Works with the latest Elixir.”

### Writing for support staff, customers and translators

- **Write for support staff who don’t read code.** Name the customer, the invoice or plan, and the next step; keep the module name and the ID for the engineer.
- **Never blame the paying customer.** “The card was declined”, never “You failed to pay”.
- **Say who acted.** Stripe, Braintree, Accrue or your app: each is a different actor, and the sentence names the right one.
- **Give amounts their currency and period.** In Accrue Admin and the docs, “USD 588.00 per month”, never a bare 588. Customer-facing templates (Portal, invoices, emails) format money in the host app’s own locale and style, such as “$588.00/month”.
- **Leave out “just”, “simply” and “easy”.** Integration has real steps; name them.
- **Use “they”** for a person you don’t know.

## How to write our name

**Accrue**

Accrue in running text, with a capital A. In code, packages and commands: `accrue`, `accrue_admin`, `accrue_portal`. The logo is lowercase; the name in a sentence is not.

### Not like this

- ~~ACCRUE~~: except as a label in capitals
- ~~accrue~~: in running text
- ~~Accrue.io, AccrueJS~~: not our names
- ~~the Accrue library’s~~: say Accrue’s
- ~~Accrue Billing~~: there is no such product

### Accrue admin and accrue portal

Accrue ships two interfaces of its own: Accrue Admin, for the host app’s team, and Accrue Portal, where the host app’s customers manage their billing. Customers never see these names. Neither has a logo of its own: Accrue Admin’s header shows the Accrue lockup alone, or the host app’s brand when it white-labels Admin. Possessive: Accrue’s.

## Key terms

**The words Accrue depends on.**

- subscriptions, invoices, payments: The billing records Accrue keeps in your app’s database. Instead of: billing state, billing data, stuff. Name the thing itself: “the invoice failed”, not “billing state changed”.
- payment processor: The service that moves the money: Stripe or Braintree. Instead of: payment provider, gateway. The industry’s term. When you mean a specific one, name it: “Stripe sent a webhook”, not “the payment processor sent a webhook”.
- pending / paid (refunded, active): Pending: Accrue has sent a charge or refund and is waiting for the payment processor to confirm it. Paid, refunded or active: the processor has confirmed it. Instead of: observed, confirmed, processing. These are the status words Stripe and Braintree use, so Accrue’s screens match what people see in those dashboards.
- webhook delivery: One message from Stripe or Braintree to your app about something that happened. Instead of: callback, ping. It’s what Accrue’s code and Accrue Admin call these messages.
- test payment processor: Accrue’s built-in stand-in for Stripe, for tests and demos; no money actually moves. `Accrue.Processor.Fake` in code. Instead of: mock, sandbox, Fake processor. The name says what it’s for: “the test payment processor”, not “the Fake”.
- your billing module: `MyApp.Billing`, the module Accrue generates in your app; your code calls it. Instead of: wrapper, SDK, facade (outside architecture guides). “Facade” is fine in architecture guides.
- host app: The Phoenix app that uses Accrue. Instead of: parent app, consumer, client. Accrue lives inside it.

These are only the terms the brand depends on; Accrue’s docs own the full glossary. Never write seamless, robust, powerful, bank-grade, production-grade, batteries-included, best-in-class or modern alternative. Say what Accrue does instead.

## Motion

**A word, then two strokes. Then still.**

1. **0.00 s** The word fades in, without moving. Sound: silence.
2. **0.24 s** The first line is drawn from the a’s left edge, slow at first, quickest in the middle, slowing into the e. Sound: one pen stroke, loudest where the pen is fastest.
3. **0.66 s** A beat, then the second line, shorter in time and a touch quicker, as a hand’s second pass would be. Sound: a second stroke, shorter and quieter.
4. **0.96 s** Rest: exactly the static logo. Sound: silence.

### Never

The line never wipes away, bounces, loops, overshoots the e or draws right to left; the word never moves. Amounts never count up or down. Pending states never pulse or spin. Reduced motion: the finished logo fades in, and the Paid mark appears without drawing.

### Craft

- **Slow in, slow out.** Each line starts slowly, is quickest in the middle and slows into its end, like a pen pulled along a ruler.
- **Follow-through.** The second line is shorter in time than the first: the hand already knows the length.
- **Timing.** A 40 ms beat between the lines, so they read as two strokes, not one thick one.
- **One focus at a time.** The word is readable before the pen moves, and never moves itself.

### In the docs and accrue admin

- **Confirm.** In the docs and in Accrue Admin, the Paid mark draws in beside the word in 200 ms when a value becomes paid, refunded or active: for example, after someone clicks Retry payment and Stripe’s webhook turns the invoice from Pending to Paid. Pending has no mark that moves; nothing pulses while waiting.
- **Reveal.** Panels and rows appear with an opacity fade of 150 ms or less. Nothing slides in from the side.

**For developers:** `logo.close 960ms` to rest, `logo.pen-ease cubic-bezier(0.5, 0, 0.2, 1)` for each line and `confirm 200ms`, the only motion values in tokens.json. They describe the brand’s motion, not a UI spec; every keyframe is in brand.json, and the animation is in assets/motion as video.

## Sonic identity

**Pen and paper.**

When the double line is drawn, you hear it: a pen pulled along a ruler, then nothing. Quiet, short, and only where Accrue speaks for itself.

**Close**two pen strokes drawing the double line, the second shorter and quieter, loudest where the pen is fastest. Nothing at the end: the logo is simply there. **Confirm**one short stroke as a value becomes paid, for videos and talk demos.

Each sound is two files in the assets folder. The MP3 (`assets/sound/listening/`) is the listening master, tuned for laptop speakers and headphones (loudness: Close −24 LUFS, Confirm −27 LUFS); this page and the logo video play it. The WAV (`assets/sound/`) is the raw synthesis (48 kHz, mono, Close −20 LUFS, Confirm −23 LUFS) for a sound designer, who can re-record it with a real pen and ruler without changing the idea.

### Where sound plays

- **Video, talks and the website:** Close plays with the logo animation, and on the website only after a click.
- **Confirm** plays in videos and live talk demos when a value becomes paid.
- **Accrue Admin and Portal:** always silent. The Paid mark still draws, with no sound. Support teams work in shared offices and on calls, inside the host app.
- **Never** for errors, never on page load, never in emails.

### Character

Pen and paper. A pen pulled along a ruler across good paper, dry and close, rising with the pen’s speed and gone the moment it lifts; then a second, shorter pass. No chime, no tap, no success sound: the line itself is the confirmation. Short and quiet, so it never startles anyone while they’re working.

### In sync

Sound and picture share one timeline. Each stroke sits on its line: it starts as the line starts, is loudest where the line draws fastest and stops where the line ends. The sound is scheduled first and the animation starts when it is heard, so speaker and Bluetooth delay never pull them apart; a stroke may land a touch late, never early.

## Imagery: code and the product

**Show the product: real code and Accrue Admin.**

- Show real code that works with the current release (`{:accrue, "~> 1.7.0"}`), never pseudo-code.
- Take every Accrue Admin screenshot from the demo app with the test payment processor, so each release can retake the same pictures.
- Invented customers with plain, obviously fictional names (Acme Bakery, Riverside Dental) and invented amounts. Never a real customer, card or email address.
- Light and dark versions of each, at 2× resolution, never upscaled.

### Don’t

- No growth dashboards or tilted, glowing screens.
- No mock-ups of features that don’t exist, and no claim that Braintree works exactly like Stripe unless it has been tested.
- No tilted devices, glowing code or terminal art.
- No dashboards of revenue going up: Accrue shows what happened to each payment, not growth.

Admin pictures in this book are simplified renderings of Accrue Admin with sample data from the Taskly demo app.

## Imagery: code colors

**Quiet code colors that never look like a status.**

- No status colors in code blocks: no brass, no red and not the Paid green, so nothing in code looks pending, failed or paid.
- In code blocks, keywords and module names stand out by weight (600), not by another color.
- Syntax colors are for code blocks only. Inline code in a sentence is always plain IBM Plex Mono on a Folio chip, in every medium.
- Use these colors where Accrue styles code blocks: HexDocs, slides, blog posts and screenshots. GitHub highlights the README’s code itself; leave that alone.
- Show real code that works with the current release, never pseudo-code.

| Role | On Folio (light) | On Felt (dark) |
| --- | --- | --- |
| **Text**Names, operators and punctuation. Keywords and module names are the same color in weight 600. | Aa #17392D | Aa #F3EEDF |
| **Comment**Comments, in Pencil and Sage. | Aa #5B6A60 | Aa #A7BCAE |
| **String**Strings and string interpolation, in a muted plum: away from green, brass and red. | Aa #74476A | Aa #D9B4CC |
| **Atom**Atoms, keyword keys and numbers: in a cool slate. | Aa #3D5876 | Aa #AFC4DC |

Every code color has at least 4.5:1 contrast on its code background. For HexDocs, add `assets/code/accrue-exdoc.css` through ExDoc’s `before_closing_head_tag`; it covers light and dark mode.

## Imagery: photography

**Paper, hands and daylight.**

Photographs are rare: talk slides, blog posts and a future website. They set a scene of careful work; they are not pictures of billing.

### Photography: use

- Daylight and real surfaces: paper, desks, notebooks. Hands rather than faces.
- Calm frames with room for a headline beside them.
- Muted, natural color, so Ledger Green stays the strongest color on the page.

- Use: Checked by hand. Work checked line by line, by hand. Brief: A hand with a pen marking a printed sheet; hand only. Photo: Glenn Carstens-Peters, Unsplash License.
- Use: Where the work happens. A quiet place where billing code gets written. Brief: An ordinary desk with a laptop, nothing legible on screen; no people, no logos. Photo: Kari Shea, Unsplash License.
- Use: Kept in order. Every record in its place, so it can be trusted later. Brief: Ordered paper: cards, notebooks or a binder; not sepia nostalgia. Photo: Maksym Kaharlytskyi, Unsplash License.

The use examples are free-licensed stock, matched to these briefs until the project’s own photographs replace them. The subjects to avoid are free-licensed photographs too; card brands that appear in them are incidental.

### Photography: subjects to avoid

- Avoid: Coin jars and piggy banks: the savings-app world, and another company named Accrue.
- Avoid: Glowing credit cards: payments marketing, not a library.
- Avoid: Market charts and trading screens: growth, which Accrue doesn’t promise.
- Coins, piggy banks, wallets and savings jars: the consumer-finance world.
- Credit cards, phones with payment apps, tap-to-pay.
- Growth charts, rising arrows, stairs and dollar signs.
- Staged stock smiles and handshakes.

## Imagery: photo treatment

**One quiet grade for every photograph.**

- **White balance:** neutral to a touch warm, so whites sit near Ledger Paper, never blue.
- **Contrast:** gentle. Bright areas stay soft and dark areas never go fully black, so no detail is lost.
- **Saturation:** well below the camera’s, so Ledger Green stays the strongest color on the page.
- **Shadows:** a faint green tint toward Ledger Green; bright areas stay neutral.

### Photography: treatments to avoid

- Avoid: Teal and orange: the film-poster grade.
- Avoid: Heavy vignette and grain: a filter, not daylight.
- Avoid: Sepia: nostalgia, not careful work today.

No heavy filters, vignettes, fake grain or sepia, and never a teal-and-orange grade. The set should look like it was shot on one quiet afternoon. These three are the same photograph as the pair on the left, with the wrong grade.

### The grade as a file

A LUT (color lookup table) is a small file that applies one color grade to any photograph. Apply `accrue-ledger-daylight.cube` in Lightroom or Photoshop (Color Lookup), Resolve, Final Cut, Premiere or ffmpeg (`lut3d`), at 100% on a correctly exposed photograph; lower the opacity if a photo was already muted. The file is in `assets/imagery`, with the example photographs and their licenses.

## Imagery: illustration

**Illustrate with diagrams and the line.**

### Illustration: use

- Accrue has no illustration style beyond two things: the double line itself, and diagrams.
- Diagrams: boxes and arrows in Ledger Green and Column Line on Ledger Paper, with Line Green on the one path that matters. Labels are in Public Sans, module names in IBM Plex Mono.
- Status in diagrams uses the status colors and their words.
- Icons: the host app’s or the platform’s own set in Accrue Admin; none on Accrue’s own pages.

A diagram in the brand’s style, with Line Green on the one path that matters.

The double line, under the one final thing on a surface.

### Illustration: avoid

- Avoid: Isometric servers, coins flowing through pipes, glowing data streams: generic infrastructure art.
- Avoid: The Elixir drop or the Phoenix bird recolored as Accrue’s: they belong to those projects.
- Avoid: A mascot or a character holding money: the consumer-app world.

Drawn for this book, so no real project’s mark is reproduced.

## Graphic device: the closing line

**The closing line.**

The brand’s graphic device is the double line itself, taken from the logo: under a page title, under a total, under the headline of a talk slide. It says “this is final” in the convention every ledger has used.

Use it once per surface, as wide as what it sits under, in Line Green on light or Mint Line on dark. In the product, a small double line beside the word marks Paid; the full line goes under totals only.

Not through or above words, not as a section divider, not in blue, not on a pending or failed value, and animated only as one left-to-right draw.

## Graphic elements

**A small set of graphic elements, each with one job.**

**The closing line**

The double line under the one final thing on a surface: a title, a total, a slide headline.

Once per surface, as wide as what it sits under.

**Column figures**

Amounts and IDs in IBM Plex Mono, right-aligned, with the currency code, so figures line up from top to bottom.

Real figures, or ones clearly marked as samples.

**The lined table**

Rows divided by Column Line hairlines, labels in spaced capitals. No zebra stripes, no boxes.

Use it for data to compare, never for page layout.

**The voice line**

One sentence in Besley italic, the way a careful person would say it.

Once per surface, on Accrue’s own pages.

Not among the graphic elements: coins, piggy banks, wallets, credit cards, stairs and rising arrows, padlocks and shields, dollar signs as decoration, gradients, lined-paper patterns and repeated lines as texture.

## In the product

**In the product: Accrue Admin stays in the background.**

Accrue Admin runs inside the host app. By default it shows Accrue’s own look; a host app can white-label it with its own name, logo and accent. These are starting points for Accrue Admin’s theme, not component specs.

**Status with its word**

Paid in green with its double-line mark, Pending in brass, Failed in red ink. Always show the word: color is never the only signal.

Never green for a charge that has only been sent. Pending is not paid.

**Action color**

Buttons and the selected nav item use Ledger Green (Mint Line on dark), or the host app’s accent if set (`:admin_branding`). Other greens stay on status and the line.

One primary action per view.

**Amounts in columns**

IBM Plex Mono, right-aligned, currency code first, with the double line under the total.

Never animate amounts.

**IDs you can copy**

Stripe and Braintree IDs and webhook event IDs in IBM Plex Mono, on Folio, selectable.

Never truncate an ID without a way to copy it whole.

Shape: small, soft corners (a 6 px radius), flat surfaces and hairlines instead of shadows. These are Accrue’s own values for radius and elevation; a host app can override them in Accrue Admin’s theme. The header shows one name, never two: Accrue with “Admin”, or the host app’s own once white-labeled.

## In the product: type and neutrals

### Type in accrue admin

- Page title: Besley 600, 28/34 px. Sample: “Riverside Dental”
- Section title: Public Sans 600, 15/20 px. Sample: “Invoices”
- Text and controls: Public Sans 400, 14/20 px. Sample: “Team plan, 12 seats”
- Label: Public Sans 600, 11/12 px, capitals, +8%. Sample: “LAST WEBHOOK”
- Amounts and IDs: IBM Plex Mono 400, 14/20 px, tabular, right-aligned. Sample: “USD 588.00”

### Neutrals and actions

| Role | Light | Dark |
| --- | --- | --- |
| Background | Ledger Paper | Ledger Green |
| Panels and code | Folio | Felt |
| Hairlines | Column Line | Ledger Paper at 16% |
| Text | Ledger Green | Ledger Paper |
| Secondary text | Pencil | Sage |
| Actions | Ledger Green, or the host app’s accent if one is set | Mint Line, or the host app’s accent if one is set |
| Focus | a 2 px Ledger Green outline, 2 px off the element | a 2 px Mint Line outline |

Accrue Admin follows the host app’s theme setting (system, light or dark, from its admin branding settings, `:admin_branding`). Both modes use these roles; the hex values are on the color pages and in tokens.json.

## In the product: status and messages

**Say what is known, what is pending and what to do.**

| What Accrue knows | Status | Example |
| --- | --- | --- |
| A charge or refund was sent; Stripe hasn’t answered | Sent to Stripe | Refund re_1Pz2… for USD 64.67 |
| A webhook was received and verified; Accrue is updating its record | Received, updating | invoice.paid, evt_1QA9… |
| A retry or job is queued | Retry scheduled | Attempt 3 of 4 on Nov 3 |
| Stripe or Braintree confirmed it, in its response or a verified webhook | Paid Refunded Active | Invoice in_1Q2c… paid |
| Stripe, Braintree or a check refused it | Declined Failed | Card declined by the issuer |
| Nothing from Stripe yet, or the last update is old | No update | No webhook for 24 hours |

- Use the support team’s words: customer, subscription, invoice, payment, refund. Module names and other technical terms belong in the details, for engineers.
- Name the action for its result: “Cancel at period end”, “Cancel now”, “Retry payment”, never “Submit” or “OK”. A button or link on its own has no final period.
- Before a destructive action, say what it affects and what happens, and offer the safer option beside it.
- Say what the system does in the present tense (“updates when the webhook arrives”, not “will update”). No exclamation marks, no “Success”, and no middle dots as separators: use a comma or a new line.

### Every message, in order

1. What happened, in the past tense, naming the object.
2. What is pending, and who acts next: Stripe, Braintree, Accrue, the host app or the person reading.
3. What they can do, as a link or button named for its outcome.

### This, not that

- Say: “Refund requested. Stripe hasn’t confirmed it yet. The status updates when the webhook arrives.” Not: “Refund successful!”
- Say: “Payment declined by the card issuer. Recovery retries on Nov 3. Retry now or email the customer.” Not: “Error: card_declined.”
- Say: “No update: no webhook has arrived for this charge in 24 hours. Check it in the Stripe dashboard.” Not: “Charge failed.”
- Say: “Cancel Riverside Dental’s Team plan now? Access ends today. No refund is issued.” Not: “Are you sure?”
- Say: “No invoices match these filters. Clear filters” Not: “Clear or adjust the filters above to inspect matching billing records.”

## Applications: HexDocs

HexDocs is where an Elixir developer decides whether to trust a library. ExDoc takes a custom logo and stylesheet: the lockup on Felt, Besley titles with the double line under them, IBM Plex Mono for code.

The same guide on a phone.

## Applications: GitHub and sharing

The README: the lockup on Ledger Paper, the tagline first because the reader is already here, then the descriptor.

Social preview, 1280 × 640 (shown at half size). Search-indexed, so the descriptor leads and the tagline follows.

The avatar is a square file; GitHub and Hex crop it themselves, so the symbol is centered with room for their crop. The browser tab shows the 16 px drawing.

## Applications: inside the host app

Accrue Admin as it ships, in a host app that has set no branding: Accrue’s lockup in the header, and Ledger Green for the one action.

White-labeled by Taskly, a sample host app: its name replaces Accrue’s in the header and its blue replaces the action color. A small “Accrue v1.7.0” stays in the footer.

The invoice template, in the host app’s brand: its own name, font and way of writing money (“$588.00”, where Accrue Admin writes “USD 588.00”). Accrue’s only trace is the double line under the total, drawn in the host app’s text color.

## Applications: talks, stickers and a tee

A talk title slide: the headline on the left with the double line under it, the lockup small at the foot.

Stickers on a light laptop lid and a dark one: the die-cut lockup in both colorways, the die-cut symbol, the tile, the tagline and the Mix dependency. Cut to shape; never on a white backing.

The tee: the lockup in Ledger Paper and Mint Line on Ledger Green, 25% of the chest width.

## Considered and not needed

**Mascot**

Considered, not proposed. A billing library is trusted for being exact; a character would pull it toward the consumer-app world it must stay out of.

**A pattern or watermark**

A repeated double line reads as lined paper or a strikethrough. The double line appears once per surface.

**Packaging, signage and stationery**

Accrue is a Hex package with no shop, office or stationery. HexDocs and the README are where people find it and where it speaks.

**Co-branding with hosts**

Host apps never show Accrue to their customers, so there is no co-brand lockup. For conference or sponsor pairings, put the partner’s logo to the right with a 1 px Column Line divider, at a matching x-height.

## Brand assets: which file to use

| You need | Use (in assets/) |
| --- | --- |
| HexDocs, the README, documents and slides on a light background | `logo/accrue-lockup-light.svg` |
| The same on Ledger Green or another dark background | `logo/accrue-lockup-dark.svg` |
| One-color printing, engraving, embroidery | `logo/accrue-lockup-mono-ledger-green.svg` `logo/accrue-lockup-mono-paper.svg` |
| The symbol alone: avatars, the Accrue Admin sidebar, stickers | `logo/accrue-symbol-light.svg` `logo/accrue-symbol-dark.svg` `logo/accrue-symbol-mono-ledger-green.svg` |
| 64 px and below: the symbol drawn for each size (use the file for the size) | `logo/accrue-symbol-{16,24,32,48,64}-{light,dark}.svg` |
| The closing line as a graphic (titles, totals, slides) | `logo/accrue-closing-line-light.svg` `logo/accrue-closing-line-dark.svg` |
| App tile: Hex, Livebook, GitHub, avatars | `icon/accrue-tile.svg` `icon/accrue-tile-1024.png` `icon/accrue-tile-512.png` `icon/accrue-tile-64.png` |
| Browser tab, HexDocs favicon and home screen | `icon/favicon.svg` `icon/favicon-32.png` `icon/favicon-16.png` `icon/accrue.ico` `icon/apple-touch-icon-180.png` |
| GitHub social preview and avatars | `social/accrue-social-preview-1280x640.png` `social/accrue-avatar-1024.png` |
| Sounds: raw WAVs for sound designers; MP3s mastered for speakers, for the web and videos | `sound/` `sound/listening/` |
| The logo animation with its sound, for videos and talks | `motion/accrue-logo-animation.mp4` `motion/accrue-logo-animation.webm` |
| The photo grade (a LUT) and the example photos, with licenses | `imagery/accrue-ledger-daylight.cube` `imagery/README.md` |
| Fonts for design apps (install) and the web | `fonts/variable/` `fonts/static/` `fonts/web/` |
| Colors (code colors included), type and motion values for Accrue Admin’s theme and HexDocs | `../tokens.json` `code/accrue-exdoc.css` |
| The whole brand as data, or as text for an AI assistant | `../brand.json` `../BRAND.md` |
| This book to print or send, a one-page summary, and a visual guide to every file | `../accrue-brand-book.pdf` `../accrue-one-page.pdf` `index.html` |

### Retired with version 2.0

- **The four-step stair mark, its favicons and the subtitle lockup.** Replace with the lockup, symbol and icon files in this folder.
- **The name set in Geist Regular as a logo.** Use the lockup files. In running text the name is plain text in the surrounding font.
- **Cobalt #5D79F6 as the brand accent.** Ledger Green carries buttons and links; Mint Line on dark backgrounds.
- **Moss as both the brand color and the “paid” status.** Status colors mean status only: Paid, Pending, Failed.
- **brandbook/tokens (tokens.css, tokens.json, June 2026).** Use tokens.json from this folder; Accrue Admin’s theme takes its values from it.

## Contact, approval and legal

**Who to ask, and what’s ours.**

### Contact and approval

- Questions about the brand and requests to use it: the Accrue maintainers, through the project’s GitHub issues (github.com/szTheory/accrue).
- Approval: changes to the logo, colors, type or sounds need a maintainer’s approval and a new version of this book. Everyday applications that follow these rules need none.
- This book is versioned: touch-ups raise the decimal (2.1), a new identity raises the whole number (3.0). The revision history is below.

### Legal

- Accrue is not a registered trademark. Use ™ (not ®) only to claim the name as a trademark, once, on the first prominent use in marketing; never on the logo itself.
- Not to be confused with the consumer savings app, also named Accrue, at byaccrue.com: it is a different company. Accrue the library never uses wallet, savings or rewards language, coral or red as a brand color, or growth imagery.
- The code is MIT-licensed. This book asks that the name and logo identify the official project only (see above).
- Credit Pay (Ruby) and Laravel Cashier as prior art; never compare Accrue against them.
- Fonts: SIL Open Font License 1.1 (see assets/fonts). Trademark clearance has not been done (see To review).

### Revision history

**Version 2.0**, 30 October 2026. A new identity: the lowercase Besley wordmark with a bookkeeper’s double line under it, the ledger palette with its paid and pending colors, Besley, Public Sans and IBM Plex Mono, voice, motion, sound, imagery, the brand’s place inside host applications and the files to use it all.

## To review

**Choices made in this edition that are easy to change**

1. **Shade values.** Ledger Green #17392D, Line Green #3F8A68, Mint Line #8FCBAA, Brass #D1A24E and Brass Ink #7D5A1F, as presented.
2. **Red Ink for failed outcomes.** Added in the book: #A33A2C on light, #F0937F on dark, always with the word; Paid Ink #2E6B4E for Paid on light.
3. **A fourth status, No update.** Pencil or Sage, for when Stripe hasn’t sent anything yet or its last update is old: Accrue’s own rule that no news is neither success nor failure.
4. **A heavier double line.** Each bar is now 100 units, the weight of the top of the a’s bowl, 68 apart and 120 under the baseline (the presentation drew 64, 44 and 110). The thinner line read as an underline.
5. **The symbol drawn per size.** Separate pixel-fitted drawings at 16, 24, 32, 48 and 64 px, each keeping both lines. The presentation scaled one drawing down.
6. **Besley italic for quotes.** Added for the voice line and pull quotes; the presentation used it once.
7. **Admin and Portal are silent.** Sound only on Accrue’s own surfaces, and only after a click.
8. **No Accrue name on host surfaces.** No logo or “Powered by” on invoices, emails or Portal. The branding config’s `business_name` default is “Accrue”; the product may want to require it.
9. **Accrue Admin’s default brand.** Accrue’s own brand by default (the lockup alone in the header, Ledger Green actions). The host app’s name, logo and accent replace it only when white-labeled, never both. Nothing is set beside the logo: “Admin” would add nothing. The product has to build the default and the switch.
10. **The tagline and the voice principles.** “Paid means paid.” replaces June 2026’s “Billing state, modeled clearly.”; the voice principles (measured, exact, native, durable) carry over.
11. **Light as the default background.** Ledger Paper for docs, the README and Accrue Admin; Ledger Green for the cover, talks, the social card and dark mode.
12. **Motion values.** A one-second close: the word in 180 ms, the lines drawn 240 to 620 and 660 to 960 ms; a 200 ms Paid mark.
13. **Example photographs.** Free-licensed stock, graded with the brand LUT, until the project’s own replace them.
14. **No website grid in the book.** A website build guide sets its own grid within the layout principles.

**Not checked:** Trademark clearance (another company named Accrue, a consumer savings app, exists; on 30 October 2026 its site (coral on white) and those of Pay, Laravel Cashier and Bling showed none with a serif wordmark or bottle green), print color (proof against a physical swatch; no CMYK or Pantone values are given), the sounds on a range of real speakers, a HexDocs stylesheet and Accrue Admin’s theme built from these values, and the icons as Hex, Livebook and GitHub crop them.
