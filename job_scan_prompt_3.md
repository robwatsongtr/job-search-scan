# Weekly finance job scan
Find open senior finance and accounting roles at the companies in `companies_sources.md`. Deliver a Gmail draft to chris@ccsconsulting.org with five sections: Senior roles, Other finance roles, Team-page watch, Not covered this week, and Summary (details at the end).

## Before you start: last week's email
Search Gmail for the most recent "Weekly finance job scan" email. You'll use it to mark postings NEW or SEEN and to compare team pages. If none exists, treat everything as NEW and team pages as a baseline.

## Step 1: Read company job boards directly
- For every company under "Readable with web fetch," fetch its URL and follow its Notes.
- If a page shows placeholder text ("Text", "City", "Loading...", a sample job card), treat it as not loaded and report nothing from it.

## Step 2: Search for postings
- For every company, search the web for its open finance roles. Aggregators (Indeed, LinkedIn, ZipRecruiter, Built In, Glassdoor, dejobs.org, etc.) may be used to find postings.
- Skip staffing-agency listings that don't name one of our companies as the employer.
- If a browser tool is available, also open the URLs of companies under "Needs browser or scraper" and read their lists, following their Notes.

## Step 3: Verify every posting from Step 2
Open the employer's own posting page:
- Shows the job: VERIFIED. Report the employer's URL.
- Redirects to a search page, 404s, or says "no longer accepting applications" or "position filled": CLOSED. Drop it, but count it.
- Won't load or shows no job content: UNVERIFIED. Report it with the aggregator URL.
Never build, shorten, or guess a URL; copy it exactly from a page you opened. Merge duplicates (match by requisition ID, else title + location).

## Role match
Match any of these keywords in the job title or the opening of the description:
SOX, Audit, Auditor, Internal Audit, Tax, Finance, Financial, Financial Analyst, FP&A, Controller, Assistant Controller, Treasury, Treasurer, Accounting, Accountant, Senior Accountant, Accounting Manager, Technical Accounting, SEC, CFO, Corporate Development, Strategic Finance, Bookkeeper, Compliance, Revenue, ASC 606.

Whole words, case-insensitive, except "SEC," which must be uppercase. Exclude roles where the keyword is incidental (e.g., "Financial advisor sales rep," "Tax attorney," "Audit nurse"); the goal is corporate finance/accounting/audit roles. When unsure, include it and mark "Check."

## Seniority
- SENIOR: Director, Senior Director, Head of, VP, SVP, EVP, Chief (CFO, CAO, etc.), Treasurer, Controller, Corporate Controller, or any "Interim" leadership role.
- OTHER: everything else.
If unsure, tag SENIOR and mark "Check."

## Location
Include if fully remote (US), or in the Oregon or Vancouver, WA metro (including hybrid out of an office there).
- "Oregon" means the state; exclude places like "Oregon, IL."
- "Remote-XX" roles limited to one state count only if that state is Oregon.
- If a listing shows "+ N other locations," open the posting to check before excluding it.

## New vs. seen
NEW if the posting's URL (or same title + company) wasn't in last week's email; otherwise SEEN. Don't use posted dates; sites often refresh them on reposts.

## Team-page watch
For companies whose Notes say "watch the team section," list the finance staff (CFO, Controller, VP Finance, and similar) by name and title. Mark any added, removed, or changed entry vs. last week as CHANGE.

## Output: the Gmail draft
Subject: Weekly finance job scan — {today's date}

1. **Senior roles**: table with columns Status (VERIFIED / UNVERIFIED) | New/Seen | Company | Title | Location | Link | Notes. NEW first.
2. **Other finance roles**: one line each: Status, New/Seen, Company, Title, Location, Link.
3. **Team-page watch**: current finance names and titles per watched company; CHANGE items first, or "No change."
4. **Not covered this week**: companies with no board read and no search results, with the reason.
5. **Summary**: one line, e.g., "36 companies; 4 senior (2 new), 7 other; 3 closed listings dropped."

Write "not listed" for any missing field. Never guess.
