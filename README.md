# Heavy Software Suite

50 open-source projects in Python, with 1,227 automated tests and about 30,000 lines of code and tests. Each project has its own repository, README, MIT licence and continuous integration.

Most need only Python. The web apps run on your own computer with no internet, and keep data in one file.

## How this was checked

- Every project's tests pass from a clean clone of its repository.
- All 25 web apps were started as real processes and tested over real sockets, including a restart with saved data and refusal of forged requests.
- Independent references were used where they exist. TinySQL runs 400 random queries against SQLite, TinyGit matches real Git's hashes, mAP Evaluator matches pycocotools to 9 decimal places, SeedBench matches SciPy, and TreeBoost is compared with scikit-learn.

## What was not checked

The web apps have not been used by real teachers, field teams or shops. Three of them were reviewed on screen at phone and desktop sizes, in light and dark mode, which found three layout problems that the tests had missed, all now fixed. The other 22 share the same styling, but were not looked at one by one. BubbleSheet is tested on simulated photos only. Each README states its own limits. These are teaching and small-scale tools, and they have not had a security review.

These projects were built with AI assistance (Claude Code), as each commit records.

## Systems from scratch

Core computer science, built to be read. Where a real reference exists, the tests compare with it.

| Project | What it does | Tests |
|---|---|---|
| [TinySQL](https://github.com/Apurba94/tinysql) | A relational database engine from scratch: SQL parser, on-disk B-tree pages, joins, aggregates, indexes and crash-safe transactions. | 24 |
| [Forge](https://github.com/Apurba94/forge-lang) | A small statically typed programming language: lexer, parser, type checker, bytecode compiler, optimiser and stack virtual machine. | 29 |
| [TinyGit](https://github.com/Apurba94/tinygit) | Version control from scratch: content-addressed objects, commits, branches, diffs and three-way merges with conflict markers. | 27 |
| [TinyRedis](https://github.com/Apurba94/tinyredis) | An in-memory data server speaking the Redis protocol: strings, lists, hashes, sorted sets, expiry, pub/sub and an append-only log. | 30 |
| [TextSearch](https://github.com/Apurba94/textsearch) | A full-text search engine: on-disk inverted index, BM25 ranking, phrase and boolean queries, fuzzy matching and highlighted snippets. | 27 |
| [SheetCalc](https://github.com/Apurba94/sheetcalc) | A spreadsheet engine: formula parser, dependency graph, incremental recalculation, cycle detection and 40 built-in functions. | 30 |
| [FlowQueue](https://github.com/Apurba94/flowqueue) | A durable job queue and workflow engine: retries with backoff, cron schedules, DAG pipelines and crash recovery on SQLite. | 26 |
| [TinyHTTP](https://github.com/Apurba94/tinyhttp) | An HTTP/1.1 server from raw sockets: request parser, router, middleware, keep-alive, static files and WebSockets on asyncio. | 29 |
| [NetSim Lab](https://github.com/Apurba94/netsim-lab) | A network simulator for teaching: links, switches, routers, link-state routing and a TCP with retransmission and congestion control. | 31 |
| [CPU16](https://github.com/Apurba94/cpu16) | A 16-bit computer from scratch: instruction set, two-pass assembler, emulator with interrupts, debugger and disassembler. | 26 |

## AI and vision research

Research engineering for computer vision and machine learning, checked against standard libraries where possible.

| Project | What it does | Tests |
|---|---|---|
| [mAP Evaluator](https://github.com/Apurba94/map-evaluator) | A from-scratch COCO-style detection evaluator: mAP, AR, per-class and size breakdowns, and an error analysis of what went wrong. | 27 |
| [TrustScore](https://github.com/Apurba94/trustscore) | Model trust toolkit: calibration error, temperature scaling, reliability data, and conformal prediction sets and intervals with coverage. | 24 |
| [LabelCheck](https://github.com/Apurba94/labelcheck) | Find label errors in datasets with confident learning, near-duplicate detection, and agreement statistics between annotators. | 26 |
| [Annotation Forge](https://github.com/Apurba94/annotation-forge) | Convert detection labels between YOLO, COCO and Pascal VOC, validate them, and make stratified group splits that stop data leakage. | 24 |
| [Corrupt Lab](https://github.com/Apurba94/corrupt-lab) | Image corruption and stain augmentation in NumPy: noise, blur, weather, JPEG-style blocking and H&E stain jitter at set severities. | 25 |
| [NumPy CNN](https://github.com/Apurba94/numpy-cnn) | A deep-learning framework in NumPy: reverse-mode autograd, convolutions, batch norm, residual blocks, optimisers and a training loop. | 28 |
| [Track Lab](https://github.com/Apurba94/track-lab) | Multi-object tracking from scratch: Kalman filter, Hungarian matching, SORT and ByteTrack, with MOTA, IDF1 and HOTA metrics. | 26 |
| [SeedBench](https://github.com/Apurba94/seedbench) | Honest model comparison: multi-seed result sets, paired tests, bootstrap intervals, Holm correction and publication-ready LaTeX tables. | 31 |
| [TreeBoost](https://github.com/Apurba94/treeboost) | Tree ensembles from scratch in NumPy: decision trees, random forests and histogram gradient boosting with feature importance. | 24 |
| [FairAudit](https://github.com/Apurba94/fairaudit) | Audit a model across subgroups: fairness metrics with confidence intervals, threshold tuning and generated model cards. | 19 |

## Education and ICT teaching

Offline tools for teachers and computer labs.

| Project | What it does | Tests |
|---|---|---|
| [ExamForge](https://github.com/Apurba94/examforge) | A question bank and exam builder: blueprints, shuffled paper sets, answer keys, marking and classical item analysis. | 30 |
| [GradePath](https://github.com/Apurba94/gradepath) | A competency-based gradebook: weighted assessments, rubrics, competency mastery, report cards and class analytics. | 28 |
| [Timetable Solver](https://github.com/Apurba94/timetable-solver) | A school timetable solver: hard and soft constraints, backtracking with propagation, simulated annealing and printable timetables. | 17 |
| [AutoGrader](https://github.com/Apurba94/autograder-py) | Grade Python programming assignments: isolated runs with limits, hidden tests, partial marks and code similarity reports. | 26 |
| [Recall Cards](https://github.com/Apurba94/recall-cards) | A spaced-repetition study app with SM-2 and FSRS-style scheduling, decks, statistics and retention forecasts, offline in the browser. | 28 |
| [BubbleSheet](https://github.com/Apurba94/bubblesheet) | Optical mark recognition: print bubble answer sheets, then read phone photos with perspective correction, and mark them automatically. | 18 |
| [Typing Lab](https://github.com/Apurba94/typing-lab) | An offline typing tutor for English and Bangla: adaptive lessons from weak keys, speed and accuracy tracking, and class reports. | 22 |
| [ICT Lab Manager](https://github.com/Apurba94/ictlab-manager) | Run a computer lab: device inventory, bookings without clashes, fault tickets, maintenance schedules and licence tracking. | 22 |
| [Curriculum Mapper](https://github.com/Apurba94/curriculum-mapper) | Map competencies to units, lessons and assessments, find coverage gaps, check hours and sequence prerequisites. | 23 |
| [Attendance Radar](https://github.com/Apurba94/attendance-radar) | Attendance registers with early warning: streaks, trend detection and at-risk learner lists a teacher can act on. | 22 |

## Humanitarian field operations

Offline tools for field teams. Read each README's data protection notes before using real data. These are independent projects, and they are not products of, or endorsed by, any humanitarian organisation.

| Project | What it does | Tests |
|---|---|---|
| [Aid Register](https://github.com/Apurba94/aid-register) | Offline beneficiary and distribution register: entitlements, double-collection checks and fuzzy duplicate detection across names. | 25 |
| [FieldSurvey](https://github.com/Apurba94/fieldsurvey) | Offline survey forms from a simple definition: skip logic, validation, data entry in the browser, and automatic tabulation. | 24 |
| [Feedback Desk](https://github.com/Apurba94/feedback-desk) | A community feedback and complaints desk: triage, response deadlines, escalation, trend reports and safe handling of sensitive cases. | 19 |
| [Relief Stock](https://github.com/Apurba94/relief-stock) | Warehouse tracking for relief items: waybills, stock cards, first-expired-first-out picking, losses and reorder forecasts. | 22 |
| [Waterpoint Monitor](https://github.com/Apurba94/waterpoint-monitor) | Track water points: litres per person, queue and quality readings against set targets, breakdown patterns and repair priorities. | 21 |
| [Site Planner](https://github.com/Apurba94/site-planner) | Plan a settlement on a grid: shelters, latrines, water and paths, with spacing and capacity checks and an automatic layout. | 21 |
| [ShiftBuilder](https://github.com/Apurba94/shiftbuilder) | Build fair staff and volunteer rosters: skills, availability, rest rules and load balancing with an optimising solver. | 17 |
| [Training Register](https://github.com/Apurba94/training-register) | Record trainings and participants, score pre- and post-tests, measure learning gain and issue certificates with verification codes. | 24 |
| [Service Directory](https://github.com/Apurba94/service-directory) | A multilingual directory of local services: ranked matching by need and location, opening hours and gaps in coverage. | 25 |
| [SitRep Builder](https://github.com/Apurba94/sitrep-builder) | Turn activity data into situation reports: a who-does-what-where matrix, indicator targets, week-on-week change and print pages. | 18 |

## Office and Bangla tools

Everyday tools for small organisations, and for working with Bangla text.

| Project | What it does | Tests |
|---|---|---|
| [BanglaKit](https://github.com/Apurba94/banglakit) | Bangla text tools: Unicode normalisation, tokenising, a rule stemmer, transliteration, number words and the Bengali calendar. | 32 |
| [DocVault](https://github.com/Apurba94/docvault) | Search all your documents offline: reads text from DOCX, PDF and text files, indexes it, and finds duplicates and versions. | 25 |
| [LedgerBook](https://github.com/Apurba94/ledgerbook) | Double-entry accounting for small organisations: journals, trial balance, income and balance statements and bank reconciliation. | 23 |
| [GrantBudget](https://github.com/Apurba94/grantbudget) | Donor budget tracking: lines and periods, actuals against budget, burn rate, spending forecast and variance reports. | 20 |
| [ClinicQueue](https://github.com/Apurba94/clinicqueue) | A clinic token queue: priority levels, wait prediction, a display screen, and a queue simulator for planning staff numbers. | 19 |
| [ShopDesk](https://github.com/Apurba94/shopdesk) | Point of sale and stock for small shops: fast billing, purchases, customer credit, profit reports and reorder suggestions. | 22 |
| [TenderDesk](https://github.com/Apurba94/tenderdesk) | Procurement records: requests, quotations, weighted bid scoring, award justification and a tamper-evident audit trail. | 26 |
| [DedupVault](https://github.com/Apurba94/dedupvault) | Deduplicating backups: content-defined chunking, snapshots, integrity verification, retention policies and full restore. | 26 |
| [LogSentinel](https://github.com/Apurba94/logsentinel) | Make sense of logs: parsing, template mining, anomaly detection on rates, alert rules and incident timelines. | 28 |
| [NetWatch Lite](https://github.com/Apurba94/netwatch-lite) | Watch your own services: scheduled HTTP, TCP and disk checks, uptime and latency history, outage records and a status page. | 21 |

MIT licence for all projects. By JANIN A APURBA.
