# Spendyy

Private, offline-first personal finance and loan manager.

## Architecture
- Vercel hosts the static app only.
- Financial records are stored in IndexedDB on the user's device.
- No backend, Supabase, Firebase, login, cloud database or external API.
- JSON export/import backup is included.

## Features
- Actual cash balance, outstanding loan reserve and spendable balance.
- Separate EMI and one-time loan creation flows.
- EMI amount, installment count, first EMI date and monthly due day.
- One-time repayment amount, duration and exact due date.
- Record loan repayments, partial payments and payment history.
- Track salary, freelance income and personal expenses.
- Monthly summary and reports.
- ₹5,000 default essential-spending budget, editable in Settings.
- Responsive layout and offline app-shell caching.

## Deploy
Import this repository into Vercel as a static project. No build command or environment variables are needed; the app entry point is index.html and output is the repository root.

## Local use
Open with a local static server (not file://), or deploy to Vercel. For iPhone, open the HTTPS URL in Safari and choose Share → Add to Home Screen.

## Important limitations
- Local browser storage is not a cloud backup. Export backups regularly to Files/iCloud Drive.
- Records do not automatically sync to another phone or browser.
- iOS may evict website storage in some circumstances.
- This backend-free version has in-app due visibility but no guaranteed background push reminders.
- EMI reserve is remaining installments × EMI. One-time reserve is entered repayment amount minus recorded payments. Verify lender figures before relying on them.
- This is a record-keeping tool, not a lender or credit-score provider.
