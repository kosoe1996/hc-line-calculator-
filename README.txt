HC / Line Completion Dashboard — Checker and Remaining Time Fix

Changes:
- Removed the separate Complete Pick Line manual field and moved the input inside the Complete Pick card.
- Current Status uses the sum of Order Line values in Block Overview as its total.
- Checker Status = Block Overview Total Order Line - Complete Pick - MOD Balance Pick.
- Example: total 2,000, complete 1,000, balance 200 => checker 800 (40%).
- If Complete Pick is blank, it defaults to Total Order Line minus MOD Balance.
- Fixed Remaining Time Calculator JavaScript error: the removed summary Shift Status element was still being updated, which stopped the script.
- Current Time and Stop Time now need to be selected before results are shown; time changes recalculate.
- Break remaining is in minutes; e.g. 150 minutes = 2 hours 30 minutes.
- Stop tomorrow checkbox adds 24 hours; without it, a stop time earlier than current time means zero remaining time.
- Dashboard cards and Block Overview colors remain consistent.

Update:
1. Extract ZIP in iPhone Files.
2. Upload index.html to GitHub repository root, replacing old index.html.
3. Commit changes, wait for Pages deployment, then reload site.
