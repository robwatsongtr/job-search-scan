# Readable with web fetch

## AbSci
- URL: https://api.ashbyhq.com/posting-api/job-board/absci
- Notes: Readable (Ashby public JSON feed; no JS). Returns all jobs with title, department, location, isRemote, publishedAt. Careers page (absci.com/career) embeds Ashby via JS, so use this feed instead. Mostly US remote, none in Vancouver, WA. Confirm the Project's fetch can open it on first run.

## Oregon Tool
- URL: https://jobs.oregontool.com/search/
- Notes: "Oregon" must refer to the state. Exclude locations like "Oregon, IL" (Oregon, Illinois) or "Oregon, WI". Check the state abbreviation.

## NW Natural
- URL: https://careers.nwnatural.com/nwnaturalgas/go/Gas-Search-All-Jobs/9885100/
- Notes: Portland. Skip out-of-area NW Natural Water roles.

## Qorvo
- URL: https://careers.qorvo.com/search/?q=&sortColumn=referencedate&sortDirection=desc
- Notes: Readable. 235 jobs, 10 pages of 25, newest first; no dates in list (dates on job pages only). Needs Oregon/remote filter URL. Has OR roles in Hillsboro and Salem.

## Precoa
- URL: https://apply.workable.com/precoa/jobs.md
- Notes: Workable. Normal page needs JS, but jobs.md is a readable list of all jobs. Backup: https://apply.workable.com/precoa/llms.txt (department counts). Job pages have .md versions with posted date. Corporate roles usually under Strategy/Corporate/Accounting. Portland HQ.

## Frontier Dermatology (Silver Falls Dermatology)
- URL: https://job-boards.greenhouse.io/frontierdermatologystaffcareers
- Notes: Readable. Greenhouse, one page, grouped by department; no dates in list. Mostly clinical roles. Finance/admin roles may post under a separate practice-admin company (unconfirmed).

## GoGuardian
- URL: https://job-boards.greenhouse.io/goguardian
- Notes: Readable. Greenhouse; one page, grouped by department; no dates. Locations show only "United States"/"India" (US roles likely remote; confirm on posting). 

## Airship
- URL: https://job-boards.eu.greenhouse.io/airship
- Notes: Readable. Greenhouse (EU instance). Includes Gummicube (subsidiary) roles. Mostly remote. 

## The Portland Clinic
- URL: https://phh.tbe.taleo.net/phh02/ats/careers/v2/searchResults?org=TPC&cws=43
- Notes: Readable. Taleo; 10/page, "next" link may be session-bound. RSS with posted dates: https://phh.tbe.taleo.net/phh02/ats/servlet/Rss?org=TPC&cws=43&WebPage=SRCHR_V2&WebVersion=0&_rss_version=2 (large; fetch may truncate after ~10 newest). Mostly clinical roles. Portland metro.

## Tillamook (TCCA)
- URL: https://phe.tbe.taleo.net/phe02/ats/careers/v2/searchResults?org=TILLAMOOKCREAMERY&cws=38
- Notes: Readable. Taleo; 10/page, sorted A–Z by title; "next" link may be session-bound. Shows department per job (finance = "Finance & Accounting - 8120"). RSS (newest first, dates): https://phe.tbe.taleo.net/phe02/ats/servlet/Rss?org=TILLAMOOKCREAMERY&cws=38&WebPage=SRCHR_V2&WebVersion=0&_rss_version=2. Corporate roles in Portland.

## Grow Schools (formerly Charter School Capital)
- URL: https://growschools.com/careers/
- Notes: Readable (plain WordPress page). Fully remote company. When roles appear, check whether they link to an external ATS.

## Vector Laboratories
- URL: https://vectorlabs.com/about/careers/
- Notes: Readable (WordPress). Jobs listed on page as PDF links; apply by email, no ATS. No location/date in list; open the PDF to check. HQ Newark, CA; UK site Wilton. Only remote US roles likely fit. Payroll Manager open 10/28 (not in keyword list).

## Advanced Marketing Group (AMG)
- URL: https://advancedmarketinggroupllc.com/
- Notes: No careers page or job board. Small (~20 staff); Wilsonville, OR corporate office. Readable. 

## Centene Corporation
- URL: https://jobs.centene.com/us/en/jobs/
- Notes: READ FULL LIST, FILTER AFTER. Readable with plain fetch (~360 jobs, 10/page, ?page=N), but filters are ignored: team/location/region params in the URL have no effect, even in a real browser (confirmed 10/27). Page through all and keep jobs whose team label is Accounting, Finance & Actuarial; Legal & Compliance; or Executive Leadership. Watch "+N other locations" (open posting to check for Oregon/remote).

# Needs browser or scraper

## Group 1: Filtered URL works (just load it)

## Intel
- URL: https://intel.wd1.myworkdayjobs.com/en-US/External?locations=1e4a4eb3adf1011246675c76bf81f8ce&jobFamilyGroup=dc8bf79476611087d67aed516c5e702c
- Notes: NEEDS BROWSER/SCRAPER (group 1). Workday; fetch returns empty shell. locations=1e4a… = [e.g., Hillsboro, OR]; jobFamilyGroup=dc8b… = [e.g., Finance]. Browser shows [N] jobs as of 10/26.

## CareOregon
- URL: https://careoregon.wd12.myworkdayjobs.com/CO?jobFamilyGroup=94dda1e4d4b6100172dcb5ca37c60000&jobFamilyGroup=f54399b0b7f7100c271695e8b4870000
- Notes: NEEDS BROWSER/SCRAPER (group 1). Workday; fetch returns empty shell. jobFamilyGroup=94dd… = [name]; jobFamilyGroup=f543… = [name]. Browser shows [N] jobs as of 10/26. Covers Columbia Pacific CCO and Jackson Care Connect. Portland; Oregon-only.

## The Standard (StanCorp)
- URL: https://standard.wd1.myworkdayjobs.com/Search?locations=166b8e1f7d480137f8f159b19801231f&locations=166b8e1f7d480153342713b19801c01d
- Notes: NEEDS BROWSER/SCRAPER (group 1; confirmed working in browser). Workday. locations = Remote, OR + Portland, OR (IDs 166b…231f / 166b…c01d, order unconfirmed). 

## Weir ESCO
- URL: https://weir.wd3.myworkdayjobs.com/Weir_External_Careers?[filters]
- Notes: NEEDS BROWSER/SCRAPER (group 1, once filters are set). Workday; fetch returns an empty shell. TODO: set filters. Global board, so filter to Portland, OR (+ ESCO division). locations=… = [name]; jobFamilyGroup=… = [name]. ESCO HQ in Portland.

## Radius Recycling
- URL: https://recruiting2.ultipro.com/SCH1011SSTL/JobBoard/02ac23c5-914c-4ab4-9851-dc1bc7bd9c94/?q=&o=postedDateDesc&w=Portland%2C+OR%2C+USA&wc=-122.681425%2C45.516018&we=-123.171425%2C46.006018%7C-122.19142500000001%2C45.02601799999999&wpst=2
- Notes: NEEDS BROWSER/SCRAPER (group 1). UKG Pro (UltiPro); JS-only. Filtered to ~30 mi around Portland (w/wc/we params), sorted newest first. "SCH" = former Schnitzer Steel. Corporate finance at Portland HQ.

## UCT (Ultra Clean Holdings)
- URL: https://recruiting2.ultipro.com/ULT1005UCH/JobBoard/93be8725-1d6c-4162-aba5-e796cf8ea1b5/?q=&o=postedDateDesc&f4=eIcFfM9Kj1ibwSsbpyc13A
- Notes: NEEDS BROWSER/SCRAPER (group 1). UKG Pro (UltiPro); JS-only. f4=eIcF… = Hillsboro, OR location filter. Sorted newest first. HQ is Hayward, CA; Oregon site is Hillsboro. No remote filter applied.

## United States Bakery / Franz Bakery
- URL: https://bakeryportal.rec.pro.ukg.net/UNI1118UBAKE/JobBoard/5324de7a-568a-4c02-b992-14593e5888be/?q=&o=postedDateDesc&f5=NrVcEvhvk0WpzgYCE4Q34g+NmXzP5w6EE2qtMG28sNCTQ
- Notes: NEEDS BROWSER/SCRAPER (group 1; confirmed working in browser). UKG Pro. f5= Job Category = Administration + Human Resources (finance roles post under Administration). Read only the "Showing X of Y" results; IGNORE the "Featured Opportunities" box (unfiltered). 

## Lithia Motors
- URL: https://careers.lithiadriveway.com/opportunities?state=Oregon&category=Administrative,Finance/Accounting&
- Notes: NEEDS BROWSER/SCRAPER (group 1; confirmed working in browser). Webflow; fetch returns a TEMPLATE WITH FAKE DATA ("1,234 opportunities", sample "Sales Representative"), never report from it. Filters work in browser. Corporate HQ Medford; Driveway Finance Corp (DFC) in Tigard/Medford. Some miscategorized jobs (e.g., valets).

## Dutch Bros
- URL: https://careers.dutchbros.com/us/en/c/headquarters-jobs
- Notes: NEEDS BROWSER/SCRAPER (group 1). Phenom; search and HQ category pages load via JS. HQ page filters out shop roles. HQ split between Grants Pass, OR and the Phoenix, AZ area. Check /sitemap.xml for a readable job list.

## TEC Equipment
- URL: https://careers-tecequipment.icims.com/jobs/search?ss=1&searchCategory=8713
- Notes: NEEDS BROWSER/SCRAPER (group 1). iCIMS; fetch returns an empty shell. searchCategory=8713 = [category name]. Job pages readable. Portland HQ.

## Group 2: Small list, read everything

## Rogers Machinery
- URL: https://rogersmachinery.rec.pro.ukg.net/ROG1500RMCI/JobBoard/3adcc0eb-1570-4f2e-b02a-1a1e6946199a/?q=&o=postedDateDesc
- Notes: NEEDS BROWSER/SCRAPER (group 2). UKG Pro; fetch gets an empty shell / "unsupported browser". Sorted newest first. Small company, short list. Portland HQ.

## Columbia Machine
- URL: https://www.paycomonline.net/v4/ats/web.php/portal/9007D08709FB82E604C5E84A9527046C/career-page
- Notes: NEEDS BROWSER/SCRAPER (group 2). Paycom; fetch returns title only. Filters likely not kept in URL (same as Gee's Paycom board, unconfirmed). Small list, mostly shop roles, so read all. Company site colmac.com. Related: Columbia/Okura, same Vancouver, WA address.

## North Coast Container (formerly Myers Container)
- URL: https://northcoastcontainer.applicantpro.com/jobs/
- Notes: NEEDS BROWSER/SCRAPER (group 2). isolved (ApplicantPro); list loads via JS (fetch shows none; browser shows all). All plant roles in Charlotte, NC and Chicago, IL; none in Oregon. Confirm where corporate/finance sits post-rename. List shows address, dept, pay, posted date.

## Springbrook Software
- URL: https://springbrooksoftware.isolvedhire.com/jobs/
- Notes: NEEDS BROWSER/SCRAPER (group 2). isolved Hire ("Springbrook Holding Company LLC"); list loads via JS, so fetch sees nothing even when jobs exist (confirmed via ApplicantPro, same platform). Board live but empty as of 10/28/26 (checked in browser). Not linked from springbrooksoftware.com. Job alert sign-up available on page. Portland HQ.

## Concora Credit
- URL: https://careers-concoracredit.icims.com
- Notes: NEEDS BROWSER/SCRAPER (group 2; filters untested). iCIMS. Job list loads via JS (iframe). Individual job pages readable. Beaverton.

## Hampton Lumber
- URL: https://careers-hamptonlumber.icims.com/jobs/search?ss=1
- Notes: NEEDS BROWSER/SCRAPER (group 2; filters untested). iCIMS, list loads via JS (iframe); fetch returns hamptonlumber.com wrapper only. Job pages readable. Portland HQ; mostly mill roles.

## Group 3: Needs filtering, but filters can't go in a URL

## TransPak
- URL: https://myjobs.adp.com/transpakexternalcareersite/cx/job-listing
- Notes: NEEDS BROWSER/SCRAPER (group 3). ADP; fetch returns a blank page. Filters (e.g., Oregon) do NOT appear in the URL; read full list and keep Oregon/remote finance roles, or use ADP's backend JSON request (Network tab). 80+ locations, mostly crating/logistics, so the full list may be large. Oregon site: Tualatin.

## Gee Automotive
- URL: https://www.paycomonline.net/v4/ats/web.php/jobs?clientkey=EE0962D7FEFB07F5DA15E78B08A461D8&fromClientSide=true
- Notes: NEEDS BROWSER/SCRAPER (group 3). Paycom (iframe on geeautomotive.com/careers). Filters do NOT appear in any URL; read full list and keep sales/finance, corporate, accounting/admin, or use Paycom's backend JSON request. HQ Spokane, WA.

## Northwest Pipe Company (NWPX)
- URL: https://jobs.dayforcehcm.com/nwpx/CANDIDATEPORTAL
- Notes: NEEDS BROWSER/SCRAPER (group 3). Dayforce; JS-only. searchText= works in URL but no location filter found (no Vancouver, WA option as of 10/26/26). Read full list and keep Vancouver, WA HQ and remote finance roles. Mostly plant roles in other states. Rebranded from Northwest Pipe; nwpx.com/careers links here.

## Banfield Pet Hospital / Mars Veterinary Health
- URL: https://jobs.banfield.com/jobs
- Notes: NEEDS BROWSER/SCRAPER (group 3; filters untested). 2,000+ jobs; search results load via JS. Job pages readable. Likely Workday behind it (R- job IDs). Corporate roles are at the Vancouver, WA HQ (CTS). Interim: Source: site search.

## Fluidra
- URL: https://jobs.fluidra.com/search/?searchResultView=LIST&sortBy=date&pageNumber=0
- Notes: NEEDS BROWSER/SCRAPER (group 3; filters untested). SAP SuccessFactors, newer JS template (unlike Oregon Tool / NW Natural / Qorvo). Global board; North America HQ is Carlsbad, CA, so only remote US roles fit. Filter to US + remote if the site allows. Probably low yield to spend scraper effort on.

# Blocked

## Precision Castparts (PCC)
- URL: https://pcctalentacquisitionportal.tal.net/vx/lang-en-GB/mobile-0/appcentre-ext/brand-7/candidate/jobboard/vacancy/3/adv/
- Notes: BLOCKED. Oleeo (tal.net) with a human-verification check; no fetch, browser, or scraper. Source: job alert emails (to set up) or manual check.
