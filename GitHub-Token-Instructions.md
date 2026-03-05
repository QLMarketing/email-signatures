# How to Renew the GitHub Token for the Email Signature Generator

The email signature generator uses a GitHub Personal Access Token (PAT) to upload headshot photos. This token expires every **90 days** and needs to be renewed. Follow the steps below.

---

## GitHub Account Credentials

| Field    | Value |
|----------|-------|
| Username | `QLMarketing` | OR | 'marketing@qualitylogic.com
| Password | `2f0TbCUh2dl5st5^` |
| Token    | `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^` | (AS OF March 4, 2026)

> **Note:** Keep this document secure. Do not share these credentials outside the team.

---

## How to Tell the Token Has Expired

When the token expires, clicking **"Upload to GitHub"** in the signature generator will show an error like:

> **Upload failed (401)** — Your GitHub token may be expired or invalid.

When you see this, follow the steps below to create a new token.

---

## Step 1: Log In to GitHub

1. Go to [github.com](https://github.com) and sign in using the credentials above.

---

## Step 2: Create a New Token

1. Click your **profile icon** (top-right corner) and select **Settings**.
2. Scroll down the left sidebar and click **Developer settings** (at the very bottom).
3. In the left sidebar, click **Personal access tokens** then **Tokens (classic)**.
   - Direct link: [github.com/settings/tokens](https://github.com/settings/tokens)
4. Click the **Generate new token** dropdown and select **Generate new token (classic)**.
5. Fill in the form:
   - **Note:** `QL Email Signatures`
   - **Expiration:** Select **90 days**
   - **Scopes:** Check the **repo** checkbox (first option in the list — this checks all sub-items automatically)
6. Scroll to the bottom and click **Generate token**.
7. **Copy the token immediately** — it starts with `ghp_` and will only be shown once. If you lose it, you'll need to create a new one.

---

## Step 3: Update the Token in the Signature Generator

1. Open the email signature generator (`signature-generator.html`).
2. In the **Image Hosting** section, find the **GitHub Token** field.
3. Paste the new token into the field.
4. Click **Save**.
5. The token is now stored in your browser and will persist until you clear browser data or it expires again in 90 days.

---

## Troubleshooting

| Problem | Solution |
|---------|----------|
| Upload fails with **401** error | Token is expired or invalid — create a new one (Steps 1-3 above) |
| Upload fails with **404** error | The GitHub repository may have been moved or deleted — contact IT |
| "No GitHub token found" message | Paste your token into the GitHub Token field and click Save |
| Token field is not visible | Make sure **GitHub Repository** is selected in the Image Hosting dropdown |
| Token doesn't persist between sessions | Your browser may be clearing site data on close — re-enter the token each session, or adjust browser privacy settings |

---

## Optional: Delete Old Tokens

After creating a new token, you can delete the expired one:

1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. Find the old token (it will show as **Expired**)
3. Click **Delete** and confirm

This keeps the account tidy but is not required.
