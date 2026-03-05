# QualityLogic Email Signature Generator — User Guide

Use this tool to create a branded email signature for Outlook. No software installation required — just open the HTML file in your browser.

---

## Getting Started

1. Open **signature-generator.html** in any web browser (Chrome, Edge, Firefox, Safari).
2. The page has two columns:
   - **Left side** — Your information, image hosting settings, and photo editor
   - **Right side** — Live signature preview, copy buttons, and setup instructions

---

## Step 1: Enter Your Information

Fill in the fields in the **"Your Information"** panel:

| Field | Required? | Notes |
|-------|-----------|-------|
| **Full Name** | Yes | First and last name (e.g., "Jane Smith") |
| **Job Title** | Yes | Your official title |
| **Office Phone** | Yes | Main office number (e.g., "208-424-1905") |
| **Ext** | Optional | Your phone extension |
| **Cell Phone** | Optional | Personal or work cell |
| **LinkedIn URL** | Optional | Full URL (e.g., "https://linkedin.com/in/janesmith") |

The signature preview on the right updates automatically as you type.

---

## Step 2: Choose a Signature Style

At the top of the preview panel, click one of the two tabs:

- **With Photo** — Includes your circular headshot next to your info
- **Without Photo** — Text-only with a teal accent line on top

---

## Step 3: Add a Headshot (if using "With Photo")

### Upload Your Photo
1. In the **"Headshot Photo"** panel, click the drop zone or drag-and-drop an image.
2. The photo editor opens, showing your image in a circular crop with a teal border.

### Position and Zoom
- **Drag** the image to reposition it within the circle.
- **Scroll** your mouse wheel (or use the **Zoom slider**) to zoom in/out.
- The circle preview is exactly what will appear in your signature.

### Publish the Photo to GitHub
Your headshot needs to be hosted online so it shows up in emails. The easiest method:

1. Make sure your **GitHub Token** is saved (see below).
2. Click **"Upload to GitHub"**.
3. The photo is uploaded automatically and the URL is filled in for you.
4. You'll see a confirmation: *"Photo uploaded to GitHub!"*

> **Alternative:** Click **"Download"** to save the processed photo to your computer, then manually upload it to any web host. Update the **Hosted Image URL** field with the public URL.

### Remove a Photo
Click **"Remove"** to clear the photo and start over.

---

## Step 4: Image Hosting Settings

The **"Image Hosting"** panel controls where your signature images are stored:

- **GitHub Repository (default)** — Images are hosted at `raw.githubusercontent.com/QLMarketing/email-signatures/main/assets/img/`. This is the recommended option.
- **Custom URL** — Enter any base URL where images are hosted. The image filename will be appended automatically.

### GitHub Token (Required for Auto-Upload)

To use the **"Upload to GitHub"** button, you need a GitHub Personal Access Token saved:

1. If you already have a token, paste it into the **GitHub Token** field and click **Save**.
2. If you need a new token, see the separate document: **GitHub-Token-Instructions.md**.

The token is saved in your browser and persists between sessions. You only need to enter it once per browser/computer.

---

## Step 5: Copy Your Signature

Once everything looks good in the preview:

1. Click **"Copy Signature"** — this copies the formatted signature to your clipboard.
2. Open **Outlook** (desktop or web).
3. Go to **Settings** → **Mail** → **Compose and reply**.
4. Click in the **Email signature** editor box.
5. Press **Ctrl+V** (Windows) or **Cmd+V** (Mac) to paste.
6. Click **Save**.

> **"Copy HTML Source"** copies the raw HTML code instead. Use this only if you need to paste the source into a system that requires HTML input.

---

## How the Photo Filename Works

The generator automatically names your headshot file based on your name:

- "Jane Smith" → `Smith,-Jane.png`
- "Gary James" → `James,-Gary.png`

This keeps all headshots organized in the GitHub repository with a consistent naming convention.

---

## Multiple Computers / Browsers

- The **signature generator** is a standalone HTML file — it works on any computer with a web browser. No internet connection needed to fill in fields and preview.
- The **GitHub Token** is stored per browser. If you use a different browser or computer, paste the token again on first use.
- **Uploading to GitHub** and loading the live signature preview images both require an internet connection.

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Signature has gray/blue background in Outlook | Make sure you're using the latest version of the generator (v1.1+). Re-copy and re-paste the signature. |
| Photo doesn't appear in emails | Check that the **Hosted Image URL** points to a publicly accessible image. Try opening the URL in a browser to verify. |
| "Upload to GitHub" fails with 401 | Your token is expired or invalid. Create a new one — see **GitHub-Token-Instructions.md**. |
| "Enter a name first" when uploading | Type your full name in the form before uploading so the file is named correctly. |
| "Set a GitHub token" message | Paste a valid token into the GitHub Token field and click Save. |
| Preview looks different from Outlook | The browser preview is approximate. Outlook may render fonts slightly differently, but the layout and links will work correctly. |
| LinkedIn link not clickable in Outlook | Make sure you used **"Copy Signature"** (not "Copy HTML Source") and pasted with Ctrl+V / Cmd+V. |
