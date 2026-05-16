# personal-fintrack-ph[README.md](https://github.com/user-attachments/files/27843477/README.md)
# 💰 FinTrack PH — Personal Finance Tracker 2025

A fully client-side personal finance web app built from the Google Apps Script finance tracker. No server required — runs entirely in the browser and stores data in `localStorage`.

## ✨ Features

| Module | Description |
|---|---|
| 📊 Dashboard | KPI cards, monthly summary, bar chart, budget snapshot |
| 📅 Transaction Log | Add / delete / filter income & expense records |
| 📆 Monthly Budget | Set budgets per category, see actual vs budget with progress bars |
| 💰 Savings Goals | Track goals with progress bars, status, months remaining |
| 💳 Debt Tracker | Monitor balances, payoff progress, estimated months left |
| 📈 Net Worth | Assets vs Liabilities, monthly history table |
| 🚫 No-Spend Days | Click-to-toggle calendar for every month |
| 📉 Annual Charts | Visual bar & line charts, category breakdown, annual table |

## 🚀 Deploy to GitHub Pages (free hosting)

1. **Create a new repository** on GitHub (name it anything, e.g. `fintrack-ph`)
2. **Upload** `index.html` to the root of the repository
3. Go to **Settings → Pages**
4. Under *Source*, select **Deploy from a branch → main → / (root)**
5. Click **Save** — your app will be live at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```

That's it! No build step, no npm, no frameworks.

## 🔐 Login Credentials

| Username | Password |
|---|---|
| `admin` | `finance2025` |
| `user` | `myfinance25` |

> To change credentials: open `index.html`, find the `USERS` object near the top of the `<script>` tag, and update the key-value pairs.

```js
const USERS = {
  'admin': 'finance2025',
  'yourname': 'yournewpassword',
};
```

## 💾 Data Storage

All data is saved in the browser's `localStorage` — **no data ever leaves your device**. Each user account has its own separate data namespace.

> ⚠️ Clearing browser data/cache will erase your finance records. Consider exporting data periodically (future feature).

## 📋 Currency

All amounts are in **Philippine Peso (₱)**. The app is pre-seeded with sample data so you can explore immediately after logging in.

## 🛠️ Customisation

- **Categories**: Edit the `CATEGORIES` array in the `<script>` tag
- **Accounts**: Edit the `ACCOUNTS` array
- **Year**: Change `2025` references as needed
- **Colors**: All colors use CSS variables at the top of the `<style>` tag — tweak `--teal`, `--gold`, `--navy`, etc.

## 📁 File Structure

```
index.html    ← The entire app (single file, no dependencies)
README.md     ← This file
```

All fonts load from Google Fonts (requires internet connection).
