# Engine LinkedIn Posts

A mobile-first app for managing your LinkedIn post queue. No code required after setup — just update a Google Sheet and the app updates with it.

---

## Setup (5 minutes)

### Step 1 — Copy the Google Sheet template

Make a copy of the [post template sheet](#) *(link to be added)* into your own Google Drive.

Your sheet needs these column headers in row 1 — exact spelling, lowercase:

| publishDate | contentType | status | hook | text | hashtags |
|---|---|---|---|---|---|
| 2026-05-07 | tactical | scheduled | Your hook here | Full post text... | #Tag1 #Tag2 |

**Column values:**
- `contentType` — `tactical`, `journey`, or `commentary`
- `status` — `idea`, `draft`, `scheduled`, or `published`
- `publishDate` — YYYY-MM-DD format
- `text` — your full post body (can be multi-line in the cell)
- `hashtags` — all your hashtags as a single string

### Step 2 — Publish your sheet to the web

1. In Google Sheets: **File → Share → Publish to web**
2. Select your sheet, change the format to **CSV**
3. Click **Publish** and confirm
4. Copy the URL it gives you (or just copy the regular sheet URL — both work)

### Step 3 — Deploy the app

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/ENGINE_ORG/engine-linkedin-posts)

Click the button above. Follow the prompts. Done.

### Step 4 — Connect your sheet

Open the deployed app. You'll see a setup screen asking for your name and your Google Sheet URL. Paste it in, hit **Get Started**.

That's it. The app is now connected to your sheet.

---

## Daily workflow

**Adding a post:** Add a new row to your Google Sheet. Set `status` to `scheduled` when it's ready. Refresh the app — it appears automatically.

**Posting:** Open the app on your phone → tap **Copy Post** (or **Share Post** on mobile) → paste into LinkedIn.

**After posting:** Tap **Posted** in the app → it opens your sheet — change that row's status to `published`. Refresh the app and it moves to the Published section.

**Editing a post:** Update the cell in your sheet. Refresh the app.

---

## Buffer system

The three dots in the header show how many posts you have scheduled and ready:

- 🟢 **3+ scheduled** — healthy buffer
- 🟡 **2 scheduled** — getting thin
- 🔴 **0–1 scheduled** — time to write

---

## Changing your sheet later

Tap the ⚙ gear icon in the top right to update your name or sheet URL.

---

## Content strategy

See the [content strategy guide](https://github.com/SarahMort/vex-posts#content-strategy) in the vex-posts repo for guidance on content types, voice principles, and cadence. Same principles apply here.
