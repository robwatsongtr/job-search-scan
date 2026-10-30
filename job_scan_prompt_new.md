# Weekly finance job scan
Find open senior finance and accounting roles at the companies in `companies_sources.md`. Produce a report with five sections: Senior roles, Other finance roles, Team-page watch, Not covered this week, and Summary (details at the end).

Always show the full report in the chat when you finish. If the Gmail connector is available, also save it as a Gmail draft addressed to chris@ccsconsulting.org. If not, use last week's report if the user pastes it; otherwise mark everything NEW.

## Step 1: Read company job boards directly
- For every company under "Readable with web fetch" in `companies_sources.md`, fetch its URL and follow that company's Notes (pagination, filters, which section to read).
- If a page shows placeholder text (e.g., "Text", "City", "Store DBA", "Loading...", or a sample job card), treat it as not loaded. Do not report jobs from it.

## Step 2: Search for the rest
- For every company (including the readable ones, to catch anything missed), run web searches for its open finance and accounting roles, for example: `"[Company]" controller OR "VP finance" OR CFO OR accounting OR FP&A job`.
- Aggregator listings (Indeed, LinkedIn, ZipRecruiter, Built In, Glassdoor, dejobs.org, and similar) are allowed as a way to FIND postings.
- Skip staffing-agency listings that don't name one of our companies as the employer.
- If a browser tool is available, you may also open the URLs of companies under "Needs browser or scraper" and read their lists, following their Notes.

## Step 3: Verify every posting
For each posting found in Step 2, open the employer's own posting page (follow the aggregator's apply link, or find it on the company's board):
- Page shows the job: VERIFIED. Report the employer's URL.
- Redirects to a search page, 404s, or says "no longer accepting applications" / "position filled": CLOSED. Drop it, but count it.
- Page won't load or shows no job content: UNVERIFIED. Report it with the aggregator URL.

Never build, shorten, or guess a URL. Copy URLs exactly from pages you opened.

Merge duplicates: the same job on several sites is one posting (match by requisition ID if shown, otherwise title + location).

## Role match
Match any of these keywords in the job title or the opening of the description:
SOX, Audit, Auditor, Internal Audit, Tax, Finance, Financial, Financial Analyst, FP&A, Controller, Assistant Controller, Treasury, Treasurer, Accounting, Accountant, Senior Accountant, Accounting Manager, Technical Accounting, SEC, CFO, Corporate Development, Strategic Finance, Bookkeeper, Compliance, Revenue, ASC 606.

Match keywords as whole words, case-insensitive, except "SEC", which must be uppercase.
Exclude roles where the keyword is incidental (e.g. "Financial advisor sales rep," "Tax attorney," "Audit nurse"). Use judgment — the goal is corporate finance/accounting/audit roles.
When unsure, include it and mark it "Check" in Notes.

## Seniority
Tag each posting:
- SENIOR: Director, Senior Director, Head of, VP, SVP, EVP, Chief (CFO, CAO, etc.), Treasurer, Controller, Corporate Controller, or any "Interim" leadership role.
- OTHER: everything else.
If unsure, tag SENIOR and mark "Check".

## Location
Include a posting if any of these is true:
- Fully remote, US-based
- In Oregon or the Vancouver, WA metro (Portland, Salem, Eugene, Bend, Medford, Tigard, Beaverton, Hillsboro, Lake Oswego, Tualatin, Wilsonville, Sherwood, and so on)
- Hybrid, based out of an Oregon or Vancouver, WA office
"Oregon" must mean the state; exclude places like "Oregon, IL". "Remote-XX" roles limited to one state count only if that state is Oregon.
If a listing shows "+ N other locations", open the posting to check before excluding it.

## New vs. seen
- Search Gmail for the most recent "Weekly finance job scan" email.
- Mark a posting NEW if its URL (or same title + company) was not in that email; otherwise SEEN.
- Don't use posted dates to decide what's new; sites often refresh dates on reposts.

## Team-page watch
- For companies whose Notes say "watch the team section," fetch the URL and list the finance staff (CFO, Controller, VP Finance, and similar) by name and title.
- Compare with the "Team-page watch" section of the last scan email and mark any added, removed, or changed entry as CHANGE. If no previous email exists, report the list as a baseline.

## Output: the Gmail draft
Subject: Weekly finance job scan — {today's date}

1. **Senior roles**: table with columns Status (VERIFIED / UNVERIFIED) | New/Seen | Company | Title | Location | Link | Notes. NEW first.
2. **Other finance roles**: one line per posting: Status, New/Seen, Company, Title, Location, Link.
3. **Team-page watch**: per watched company, current finance names and titles; CHANGE items first, or "No change".
4. **Not covered this week**: companies whose board couldn't be read AND that no search turned up, with the reason (e.g., "needs browser", "blocked").
5. **Summary**: one line, e.g., "36 companies; 4 senior (2 new), 7 other; 3 stale aggregator listings dropped."

Write "not listed" for any missing field. Never guess.
