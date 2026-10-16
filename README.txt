HC / Line Completion — Block Overview + Remaining Time Fix

This build removes the manual For Checking Line field.
Complete Pick is automatic: Overall Order Line minus MOD Balance Pick Line.
It removes obsolete JavaScript event listeners and references to removed fields that could stop startup rendering.

Block Overview:
- The four default rows (Picking - E/F/G/H) should render on load.
- Total Order Line and Request HC are recalculated from those rows.

Remaining Time:
- Current Time remains a manual time picker; it is intentionally not auto-filled.
- Select Current Time and Stop Time to calculate remaining time.
- Enter remaining break minutes, available HC, and weighted lines per HC per hour.
- For an overnight shift, enable “Stop time is tomorrow”.
- If time is not selected, the calculator shows SET TIME rather than a misleading zero.

Update steps on iPhone:
1. Extract this ZIP in Files.
2. In the GitHub repository, upload index.html to the repository root and replace the old file.
3. Commit changes and wait for GitHub Pages deployment.
4. Refresh the website. If the old version still appears, close the tab and reopen the Pages URL.

The calculator remains manual-time based, as requested.
