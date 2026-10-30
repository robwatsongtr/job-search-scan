
## AbSci
- URL: https://www.absci.com/career/#current-openings
- Notes: Vancouver, WA. Confirm the board still lists current jobs.

## Oregon Tool
- URL: https://jobs.oregontool.com/search/
- Notes: "Oregon" must refer to the state. Exclude locations like "Oregon, IL" (Oregon, Illinois) or "Oregon, WI". Check the state abbreviation.

## NW Natural
- URL: https://careers.nwnatural.com/nwnaturalgas/go/Gas-Search-All-Jobs/9885100/
- Notes: Portland. Skip out-of-area NW Natural Water roles.

## Concora Credit
- URL: https://careers-concoracredit.icims.com
- Notes: NEEDS SCRAPER. iCIMS. Job list loads via JS (iframe). Individual job pages readable. Beaverton.

## Banfield Pet Hospital / Mars Veterinary Health
- URL: https://jobs.banfield.com/jobs
- Notes: NEEDS SCRAPER. 2,000+ jobs; search results load via JS. Job pages readable. Likely Workday behind it (R- job IDs). Corporate roles are at the Vancouver, WA HQ (CTS). Interim: Source: site search.

## Hampton Lumber
- URL: https://careers-hamptonlumber.icims.com/jobs/search?ss=1
- Notes: NEEDS SCRAPER. iCIMS, list loads via JS (iframe); fetch returns hamptonlumber.com wrapper only. Job pages readable. Portland HQ; mostly mill roles.

## TEC Equipment
- URL: https://careers-tecequipment.icims.com/jobs/search
- Notes: NEEDS SCRAPER. iCIMS; fetch returns an empty shell. Filter in URL: searchCategory=8713 = [category name]. Example of filter ?ss=1&searchCategory=8713 Job pages readable. Portland HQ.

## Qorvo
- URL: https://careers.qorvo.com/search/?q=&sortColumn=referencedate&sortDirection=desc
- Notes: Readable. 235 jobs, 10 pages of 25, newest first; no dates in list (dates on job pages only). Needs Oregon/remote filter URL. Has OR roles in Hillsboro and Salem.

## Precoa
- URL: https://apply.workable.com/precoa/jobs.md
- Notes: Workable. Normal page needs JS, but jobs.md is a readable list of all jobs. Backup: https://apply.workable.com/precoa/llms.txt (department counts). Job pages have .md versions with posted date. Corporate roles usually under Strategy/Corporate/Accounting. Portland HQ.

## Frontier Dermatology (Silver Falls Dermatology)
- URL: https://job-boards.greenhouse.io/frontierdermatologystaffcareers
- Notes: Readable. Greenhouse, one page, grouped by department; no dates in list. Mostly clinical roles. Finance/admin roles may post under a separate practice-admin company (unconfirmed).

## Northwest Pipe Company (NWPX)
- URL: https://jobs.dayforcehcm.com/nwpx/CANDIDATEPORTAL
- Notes: NEEDS BROWSER/SCRAPER. READ FULL LIST, FILTER AFTER. Dayforce; JS-only. searchText= works in URL but no location filter found (no Vancouver, WA option as of 10/26). Mostly plant roles in other states; keep Vancouver, WA HQ and remote finance roles. Rebranded from Northwest Pipe; nwpx.com/careers links here.

## Centene Corporation
- URL: https://jobs.centene.com/us/en/jobs/?search=&team=Accounting%2C+Finance+%26+Actuarial&team=Legal+%26+Compliance&team=Executive+Leadership&pagesize=10
- Notes: NEEDS SCRAPER. Filters are JS-only: browser shows 55 jobs (10/26), plain fetch returns all ~360 unfiltered. Unfiltered list is readable (?page=N) as a fallback. Watch "+N other locations".

## Intel
- URL: https://intel.wd1.myworkdayjobs.com/en-US/External?locations=1e4a4eb3adf1011246675c76bf81f8ce&jobFamilyGroup=dc8bf79476611087d67aed516c5e702c
- Notes: NEEDS SCRAPER (or built-in browser). Workday; fetch returns empty shell. locations=1e4a… = [e.g., Hillsboro, OR]; jobFamilyGroup=dc8b… = [e.g., Finance]. Browser shows [N] jobs as of 10/26.

## CareOregon
- URL: https://careoregon.wd12.myworkdayjobs.com/CO?jobFamilyGroup=94dda1e4d4b6100172dcb5ca37c60000&jobFamilyGroup=f54399b0b7f7100c271695e8b4870000
- Notes: NEEDS SCRAPER (or built-in browser). Workday; fetch returns empty shell. jobFamilyGroup=94dd… = [name]; jobFamilyGroup=f543… = [name]. Browser shows [N] jobs as of 10/26. Covers Columbia Pacific CCO and Jackson Care Connect. Portland; Oregon-only.

## The Portland Clinic
- URL: https://phh.tbe.taleo.net/phh02/ats/careers/v2/searchResults?org=TPC&cws=43
- Notes: Readable. Taleo; 10/page, "next" link may be session-bound. RSS with posted dates: https://phh.tbe.taleo.net/phh02/ats/servlet/Rss?org=TPC&cws=43&WebPage=SRCHR_V2&WebVersion=0&_rss_version=2 (large; fetch may truncate after ~10 newest). Mostly clinical roles. Portland metro.

## Tillamook (TCCA)
- URL: https://phe.tbe.taleo.net/phe02/ats/careers/v2/searchResults?org=TILLAMOOKCREAMERY&cws=38
- Notes: Readable. Taleo; 10/page, sorted A–Z by title; "next" link may be session-bound. Shows department per job (finance = "Finance & Accounting - 8120"). RSS (newest first, dates): https://phe.tbe.taleo.net/phe02/ats/servlet/Rss?org=TILLAMOOKCREAMERY&cws=38&WebPage=SRCHR_V2&WebVersion=0&_rss_version=2. Corporate roles in Portland.

## Dutch Bros
- URL: https://careers.dutchbros.com/us/en/c/headquarters-jobs
- Notes: NEEDS SCRAPER (or built-in browser). Phenom; search and HQ category pages load via JS. HQ page filters out shop roles. HQ split between Grants Pass, OR and the Phoenix, AZ area. Check /sitemap.xml for a readable job list.

## Rogers Machinery
- URL: https://rogersmachinery.rec.pro.ukg.net/ROG1500RMCI/JobBoard/3adcc0eb-1570-4f2e-b02a-1a1e6946199a/?q=&o=postedDateDesc
- Notes: NEEDS SCRAPER (or built-in browser). UKG Pro; fetch gets an empty shell / "unsupported browser". Sorted newest first. Small company, short list. Portland HQ.

## Weir ESCO
- URL: https://weir.wd3.myworkdayjobs.com/Weir_External_Careers?[filters]
- Notes: NEEDS SCRAPER (or built-in browser). Workday; fetch returns an empty shell. Global board, so filter to Portland, OR (+ ESCO division). locations=… = [name]; jobFamilyGroup=… = [name]. ESCO HQ in Portland.

## Radius Recycling
- URL: https://recruiting2.ultipro.com/SCH1011SSTL/JobBoard/02ac23c5-914c-4ab4-9851-dc1bc7bd9c94/?q=&o=postedDateDesc&w=Portland%2C+OR%2C+USA&wc=-122.681425%2C45.516018&we=-123.171425%2C46.006018%7C-122.19142500000001%2C45.02601799999999&wpst=2
- Notes: NEEDS SCRAPER (or built-in browser). UKG Pro (UltiPro); JS-only. Filtered to ~30 mi around Portland (w/wc/we params), sorted newest first. "SCH" = former Schnitzer Steel. Corporate finance at Portland HQ.

## TransPak
- URL: https://myjobs.adp.com/transpakexternalcareersite/cx/job-listing
- Notes: NEEDS BROWSER/SCRAPER. ADP; fetch returns a blank page. Filters (e.g., Oregon) do NOT appear in the URL; read full list and keep Oregon/remote finance roles, or use ADP's backend JSON request (Network tab). 80+ locations, mostly crating/logistics, so the full list may be large. Oregon site: Tualatin.

## Columbia Machine
- URL: https://www.paycomonline.net/v4/ats/web.php/portal/9007D08709FB82E604C5E84A9527046C/career-page
- Notes: NEEDS BROWSER/SCRAPER. READ FULL LIST, FILTER AFTER. Paycom; fetch returns title only. Filters likely not kept in URL (same as Gee's Paycom board, unconfirmed). Small list, mostly shop roles, so read all. Company site colmac.com. Related: Columbia/Okura, same Vancouver, WA address.

## Precision Castparts (PCC)
- URL: https://pcctalentacquisitionportal.tal.net/vx/lang-en-GB/mobile-0/appcentre-ext/brand-7/candidate/jobboard/vacancy/3/adv/
- Notes: BLOCKED. Oleeo (tal.net) with a human-verification check; no fetch, browser, or scraper. Source: job alert emails (to set up) or manual check. 

## UCT (Ultra Clean Holdings)
- URL: https://recruiting2.ultipro.com/ULT1005UCH/JobBoard/93be8725-1d6c-4162-aba5-e796cf8ea1b5/?q=&o=postedDateDesc&f4=eIcFfM9Kj1ibwSsbpyc13A
- Notes: NEEDS SCRAPER (or built-in browser). UKG Pro (UltiPro); JS-only. f4=eIcF… = Hillsboro, OR location filter. Sorted newest first. HQ is Hayward, CA; Oregon site is Hillsboro. No remote filter applied.

## GoGuardian
- URL: https://job-boards.greenhouse.io/goguardian
- Notes: Readable. Greenhouse; one page, grouped by department; no dates. Locations show only "United States"/"India" (US roles likely remote; confirm on posting). "Revenue Operations" dept = sales ops, not finance.

## Fluidra
- URL: https://jobs.fluidra.com/search/?searchResultView=LIST&sortBy=date&pageNumber=0
- Notes: NEEDS SCRAPER (or built-in browser). SAP SuccessFactors, newer JS template (unlike Oregon Tool / NW Natural / Qorvo). Global board; North America HQ is Carlsbad, CA, so only remote US roles fit. Filter to US + remote if the site allows. Probably low yield to spend scraper effort on.

## Grow Schools (formerly Charter School Capital)
- URL: https://growschools.com/careers/
- Notes: Readable (plain WordPress page). "There are no open positions at this time" as of 10/28; report as "no openings," not "couldn't check." Fully remote company. When roles appear, check whether they link to an external ATS.

## Airship
- URL: https://job-boards.eu.greenhouse.io/airship
- Notes: Readable. Greenhouse (EU instance). Includes Gummicube (subsidiary) roles. Mostly remote. No-unsolicited-agency policy, but I believe Chris has personal contacts there, so finance openings are worth flagging.

## Advanced Marketing Group (AMG)
- URL: https://advancedmarketinggroupllc.com/
- Notes: No careers page or job board. Small (~20 staff); Wilsonville, OR corporate office. Readable. Instead of jobs, watch the "Accounting Staff" section: as of 10/28 it lists a CFO/COO and a Controller. Flag any change to those names or titles.

## United States Bakery / Franz Bakery
- URL: https://bakeryportal.rec.pro.ukg.net/UNI1118UBAKE/JobBoard/5324de7a-568a-4c02-b992-14593e5888be/?q=&o=postedDateDesc&f5=NrVcEvhvk0WpzgYCE4Q34g+NmXzP5w6EE2qtMG28sNCTQ
- Notes: NEEDS SCRAPER (or built-in browser; confirmed working 10/28). UKG Pro. f5= Job Category = Administration + Human Resources (finance roles post under Administration). Read only the "Showing X of Y" results; IGNORE the "Featured Opportunities" box (unfiltered). 2 jobs as of 10/28, incl. Accounting Manager, Vancouver, WA.

## Vector Laboratories
- URL: https://vectorlabs.com/about/careers/
- Notes: Readable (WordPress). Jobs listed on page as PDF links; apply by email, no ATS. No location/date in list; open the PDF to check. HQ Newark, CA; UK site Wilton. Only remote US roles likely fit. Payroll Manager open 10/28 (not in keyword list).

## Springbrook Software
- URL: https://springbrooksoftware.isolvedhire.com/jobs/
- Notes: NEEDS BROWSER/SCRAPER. isolved Hire ("Springbrook Holding Company LLC"); list loads via JS, so fetch sees nothing even when jobs exist (confirmed via ApplicantPro, same platform). Board live but empty as of 10/28 (checked in browser). Not linked from springbrooksoftware.com. Job alert sign-up available on page. Portland HQ.

## The Standard (StanCorp)
- URL: https://standard.wd1.myworkdayjobs.com/Search?locations=166b8e1f7d480137f8f159b19801231f&locations=166b8e1f7d480153342713b19801c01d
- Notes: NEEDS SCRAPER (or built-in browser; confirmed working 10/28). Workday. locations = Remote, OR + Portland, OR (IDs 166b…231f / 166b…c01d, order unconfirmed). 15 jobs as of 10/28; relative dates + REQ IDs. HIGH PRIORITY. Senior actuarial roles open (VP and Director); "Actuary" not in keyword list.

## North Coast Container (formerly Myers Container)
- URL: https://northcoastcontainer.applicantpro.com/jobs/
- Notes: NEEDS BROWSER/SCRAPER. isolved (ApplicantPro); list loads via JS (fetch shows none; browser shows all). 6 jobs as of 10/29, all plant roles in Charlotte, NC and Chicago, IL; none in Oregon. Confirm where corporate/finance sits post-rename. List shows address, dept, pay, posted date.

## Lithia Motors
- URL: https://careers.lithiadriveway.com/opportunities?state=Oregon&category=Administrative,Finance/Accounting&
- Notes: NEEDS BROWSER/SCRAPER (confirmed working in browser 10/29). Webflow; fetch returns a TEMPLATE WITH FAKE DATA ("1,234 opportunities", sample "Sales Representative"), never report from it. Filters work in browser: 9 jobs as of 10/29. Corporate HQ Medford; Driveway Finance Corp (DFC) in Tigard/Medford. Some miscategorized jobs (e.g., valets).

## Gee Automotive
- URL: https://www.paycomonline.net/v4/ats/web.php/jobs?clientkey=EE0962D7FEFB07F5DA15E78B08A461D8&fromClientSide=true
- Notes: NEEDS BROWSER/SCRAPER. Paycom (iframe on geeautomotive.com/careers). Filters do NOT appear in any URL; read full list and keep sales/finance, corporate, accounting/admin, or use Paycom's backend JSON request. HQ Spokane, WA.
