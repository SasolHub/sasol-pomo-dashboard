Sasol Rewards  Promotions Dashboard

A single-file, self-contained HTML dashboard for tracking Sasol Rewards conditional pricing / EDLP promotions — brand filters, a live calendar heatmap, sortable data table, and click-through detail popups, all in Sasol navy/blue/gold branding.

Live demo: add your GitHub Pages link here once published, e.g.
https://<your-username>.github.io/<repo-name>/


✨ Features


KPI count cards — total promotions, active now, upcoming, expired, unique brands, total basket value
Live filters — brand, year, period, status, and free-text product search, all updating instantly
Promotion calendar — monthly heatmap showing how many promotions are active on each day; click a day to filter the table to it
Sortable table — click any column header to sort; each row shows a real brand logo (fetched live via the Clearbit Logo API), falling back to a generated colour tile if no logo is found
Click-to-view popup — click any product image to open a detail card (price, qty, period, dates, status, days remaining)
Load your own Excel file — swap in a new .xlsx/.csv export at any time via the "Load Excel File" button (parsed client-side with SheetJS, no server needed)
Live clock — current date/time in Africa/Johannesburg (SAST)
Animated mascot — a small waving, blinking helper with rotating tips


Everything runs client-side. There is no backend, build step, or server — it's one HTML file.


📂 Files

FilePurposesasol-promo-dashboard.htmlThe dashboard itself — open it directly in a browserpomo-beif-clean.xlsxExample/source promotions workbook (optional to include in the repo)

📊 Expected Excel format

The dashboard expects a sheet (any name containing "promo", or the first sheet) with these columns:

ColumnTypeExampleConditionalPricingIdtext/number21565Periodnumber1Yearnumber2026BrandtextCCBSAProducttextMonster 500mlQtynumber1Price (R)number23.0Start Datedate2026-01-22End Datedate2026-03-31CommenttextEDLP

Loading a new file via the Load Excel File button replaces the dataset entirely and refreshes all cards, filters, the calendar, and the table.


🚀 Deploying on GitHub Pages


Create (or reuse) a repo and add sasol-promo-dashboard.html to it.
In the repo, go to Settings → Pages.
Under Build and deployment, set Source to Deploy from a branch, pick your branch (e.g. main) and root folder.
Save. GitHub will publish at:
