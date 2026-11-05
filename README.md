# RTO Sales Dashboard

Static site (GitHub Pages). Upload the daily RTO `reportTable` .xlsx files → dashboard updates in the browser.

- Current month till date + previous month (RTO-wise and manufacturer-wise, daily-average change)
- Line graph of top makers (Jan → current month)
- **Download report (.xlsx)** – summary, month MTD, previous month, YTD, monthly by maker, monthly by RTO

## Deploy
1. Create a GitHub repo and push all files in this folder to `main`.
2. Settings → Pages → Source: *Deploy from a branch* → `main` / `(root)`.
3. Open `https://<user>.github.io/<repo>/`.

## How data is stored
GitHub Pages has no server, so files are parsed in the browser and kept in that browser (localStorage).
A newer upload for an RTO replaces its older data (reports are year-to-date).
To make everyone see the same data: click **data.json** on the site and commit it to `data/data.json`.
