\# Invoice & Quote Generator

A single-file, no-dependency invoicing tool built for freelancers and small businesses who need something faster and cheaper than QuickBooks, but more capable than a blank template.

\#\# Why This Exists

Most free invoice tools are either too basic (no recurring billing, no client memory) or locked behind a subscription for basic features like discounts and payment status tracking. This was built to solve a real need — generating and tracking retainer-based invoices for an active freelance IT/web development client — without paying for or setting up a SaaS platform for a single-user workflow.

\#\# Features

\- \*\*Invoice & Quote modes\*\* — toggle between document types; labels (e.g. "Due Date" vs "Valid Until") adjust automatically  
\- \*\*Line-item billing\*\* — add/remove rows, auto-calculated totals  
\- \*\*Discounts\*\* — flat dollar or percentage, applied before tax  
\- \*\*Tax calculation\*\* — configurable rate, applied after discount  
\- \*\*Recurring retainers\*\* — mark an invoice as recurring (e.g. every 6 weeks), then generate the next invoice in one click with the date auto-advanced and invoice number auto-incremented  
\- \*\*Client directory\*\* — save client details once, autocomplete on future invoices  
\- \*\*Status tracking\*\* — Draft / Sent / Paid / Overdue, color-coded, visible in the saved list at a glance  
\- \*\*Stripe Payment Link integration\*\* — paste a payment link, get a working "Pay Online" button on the document  
\- \*\*PDF export\*\* — browser-native print-to-PDF with a dedicated print stylesheet (no library dependency)  
\- \*\*Local persistence\*\* — invoices and clients saved via localStorage; no backend, no account, no server required

\#\# Tech Stack

\- Vanilla HTML/CSS/JS — no framework, no build step  
\- Google Fonts (Space Grotesk, IBM Plex Mono) — only external dependency  
\- Browser localStorage for persistence  
\- Native \`window.print()\` with print-specific CSS for PDF export

\#\# Design Decisions

\- \*\*Single file, zero dependencies\*\*: works offline, easy to host anywhere (static hosting, or just opened directly from disk), no npm install or build pipeline required  
\- \*\*No backend\*\*: keeps the tool free to run and deploy; all data stays local to the browser it's used in  
\- \*\*Print-based PDF export over a PDF library\*\*: avoids adding a dependency for something the browser already does natively and reliably

\#\# Possible Future Additions

\- Multi-currency support  
\- Partial payment tracking  
\- Business logo upload  
\- CSV export of saved invoices

\#\# Usage

Open \`invoice-generator.html\` in any modern browser. No installation required.  
