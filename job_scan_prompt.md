# Weekly finance job scan
Run a weekly scan for open finance and accounting roles at the companies in `companies_sources.md` (36 companies). Deliver the results as a Gmail draft addressed to chris@ccsconsulting.org.

## Sources: careers pages only
- Use only each company's own careers page or job board, as listed in `companies_sources.md`. Follow that company's Notes (filters, sorting, which board to use).
- Never use LinkedIn, Indeed, Glassdoor, ZipRecruiter, or other job aggregators, and never use web-search snippets as evidence that a job exists.
- If a listed URL fails, shows no jobs, or doesn't load its listings, try the "Careers" link on the company's main site once. If that also fails, put the company under "Couldn't check" with the reason. Do not substitute another source.
- If a company's Notes start with "NEEDS SCRAPER", do not fetch it. List it under "Couldn't check" as "Not yet automated".

## Team-page watch
- Some companies have no job board. If a company's Notes in `companies_sources.md` say "watch the team section," fetch its URL and find the finance staff (CFO, Controller, VP Finance, Accounting Manager, and similar titles) listed on the page.
- Record each finance person's name and title exactly as shown.
- Compare against the "Team-page watch" section of the most recent "Weekly finance job scan" email. Report any name added, removed, or with a changed title as a CHANGE.
- If there is no previous email to compare against, report the current list as the baseline.

## Link rules (strict)
- Include a posting only if you opened that posting's own page during this run, and the page shows the job title.
- Exclude the posting if its page shows any closed signal: "no longer accepting applications", "position filled", "job not found", a 404, or a redirect to the general job search.
- Copy every URL exactly as it appears in the page you fetched. Never build, shorten, or guess a URL.

## Freshness
- List every currently open matching posting, not just recent ones.
- Before writing the draft, search Gmail for the most recent message with the subject "Weekly finance job scan".
- Mark each posting NEW if its URL did not appear in that message, otherwise SEEN.
- Do not rely on the posted date to decide what is new. Sites often refresh the date when they repost a job. Show the date as listed, or "not listed".

## Role match
Match any of these keywords in the job title or the opening of the description:
SOX, Audit, Auditor, Internal Audit, Tax, Finance, Financial, Financial Analyst, FP&A, Controller, Assistant Controller, Treasury, Treasurer, Accounting, Accountant, Senior Accountant, Accounting Manager, Technical Accounting, SEC, CFO, Corporate Development, Strategic Finance, Bookkeeper, Compliance, Revenue, ASC 606.

Match keywords as whole words, case-insensitive, except "SEC", which must be uppercase.

Exclude: roles where the keyword is incidental (e.g. "Financial advisor sales rep," "Tax attorney," "Audit nurse"). Use judgment — the goal is corporate finance/accounting/audit roles.

## Location
Include a posting if any of these is true:
- Fully remote, US-based
- Located in Oregon or the Vancouver, WA metro (Portland, Salem, Eugene, Bend, Tigard, Beaverton, Hillsboro, Lake Oswego, Tualatin, Wilsonville, Sherwood, and so on)
- Hybrid, based out of an Oregon office

"Oregon" must mean the state. Exclude places like "Oregon, IL" or "Oregon, WI". Check the state abbreviation.
Exclude roles based only in other states with no remote option. "Remote-XX" roles limited to one state count only if that state is Oregon.

## Output: the Gmail draft
Subject: Weekly finance job scan — {today's date}

1. **Senior roles, new**: table with columns Company | Title | Location / Remote | Date listed | Link | Notes.
2. **Senior roles, still open**: same table.
3. **Other finance roles**: one line per posting: Company, Title, Location, Link. Mark new ones "(new)".
4. **Couldn't check**: each company and the reason.
5. **Coverage**: one line, "Checked X of 36 companies; Y senior (Z new), W other."

Write "not listed" for any field you can't find. Never fill a field with a guess.
