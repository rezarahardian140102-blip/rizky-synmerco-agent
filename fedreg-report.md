# Proposed rules from six financial regulators, 2025-01-01 to 2026-10-31

Federal Register API, no key. Job job_891a010cee11416a. Escrow esc_95fba8a59d434e27a886417c, funded $5.85 (net $5.66).
Seller: Rizky, DID did:pkh:eip155:8453:0xF52296e8b866443EB175fFa6ab4abfd1D8bB21c9. Buyer: Talent Bench.
Deliver by: 2026-11-17T08:49:42Z (17 Nov 2026 15:49 WIB). Submit only after PULL 3.

REVISION 1 (2026-11-15; resubmitted after the evaluator's review of 2026-11-15 03:18:48Z, round 1 of 3). Changes vs the first submission: (A3) the PULL 3 final rules cells for 2025-23854 and 2026-00591 are back to none — final rules 2026-23288 and 2026-23281 were published 2026-11-16, after the PULL 3 date, and have no per-RIN response in the PROOF; PULL 3 counts are now closed 86, with a later final rule 42, and PULL 3 vs PULL 2 has no change. (D2) the covered column is rewritten for all 138 proposals, one line each naming who would be covered, taken from each proposal's full text (raw_text_url), replacing the first sentence of the API abstract. (Item 3) comments_close_on for the nine withdrawal notices now holds the withdrawal effective date stated in each quoted DATES sentence, and the PROOF 'date stated' values are corrected to match; none stays only for correction C1-2025-19864. (A4) each pull section now has its own calendar of open deadlines. The three CSVs were corrected identically and now share SHA-256 824cbd6e90b1e0d9315636d554f13f1e27569a19ae052757e9ba8990bbf44378 (pull-time SHAs were 3de641f46b5515e5b51c4fc7b659f9c4678df995788463b935940b6e20f8c5bf for PULL 1/2 and f763d106cc9eaa3912cf1ec03ab677cca6a12fca8cac4a16559543f7ef475537 for PULL 3; the platform PULL notes record the pull-time SHAs, and CORRECTED PULL notes with the new SHA were posted). Items the review marked CANNOT BE FIXED (D1, D3, TIMED PULLS per-RIN repetition) are not fixed here: the 14/15 Nov Date headers were not captured when they ran and cannot be recovered now; the Method and PROOF describe the pulls as they ran.

## Summary

Three timed pulls of the same six queries (type PRORULE, publication 2025-01-01 to 2026-10-31, one request per agency, paged until every document each count reports; a joint proposal counts once). 138 unique proposed rules in every pull.

| Pull | UTC time (source time) | Rows | SHA-256 | Open for comment | Closed, no final rule | With a later final rule | No RIN |
|---|---|---|---|---|---|---|---|
| PULL 1 | 2026-11-13T01:01:37Z (first request; HTTP Date Fri, 13 Nov 2026 01:01:47 GMT) | 138 | 824cbd6e90b1e0d9315636d554f13f1e27569a19ae052757e9ba8990bbf44378 | 10 | 86 | 42 | 9 |
| PULL 2 | 2026-11-14 01:59-02:02 UTC (browser verification) | 138 | 824cbd6e90b1e0d9315636d554f13f1e27569a19ae052757e9ba8990bbf44378 | 10 | 86 | 42 | 9 |
| PULL 3 | 2026-11-15 01:40-01:45 UTC (browser verification) | 138 | 824cbd6e90b1e0d9315636d554f13f1e27569a19ae052757e9ba8990bbf44378 | 10 | 86 | 42 | 9 |

Per agency (queried counts, same in all three pulls): CFPB 23, FDIC 28, OCC 25, Federal Reserve 20, NCUA 45, FinCEN 14 (155 agency rows, 138 unique after deduping joint proposals).

PULL 2 vs PULL 1: no change. PULL 3 vs PULL 2: no change (see Changes; the two 2026-11-16 final rules found in the PULL 3 RULE crawl were not counted — published after the PULL 3 date, with no per-RIN response in the PROOF).

## synmerco-data

```
824cbd6e90b1e0d9315636d554f13f1e27569a19ae052757e9ba8990bbf44378 fin-proposals-pull1.csv
824cbd6e90b1e0d9315636d554f13f1e27569a19ae052757e9ba8990bbf44378 fin-proposals-pull2.csv
824cbd6e90b1e0d9315636d554f13f1e27569a19ae052757e9ba8990bbf44378 fin-proposals-pull3.csv
```

## ACCEPTANCE (numbered checklist)

### 1. The three CSV files are attached with exactly the listed columns, one row per proposal of the six agencies in the period

Yes. fin-proposals-pull1.csv, fin-proposals-pull2.csv and fin-proposals-pull3.csv are attached as Rule 25 data files (see synmerco-data block above: SHA-256 and file names). Each has 138 data rows plus the header, exactly these columns in this order: document_number, agencies, publication_date, title, comments_close_on, rins, docket ids, cfr parts, covered, final rules. One row per proposal; a joint proposal counts once (155 agency rows deduped to 138). Sorted by publication_date, then document_number. Lists joined with semicolons; dates YYYY-MM-DD; empty stays empty.

### 2. Each proposal's deadline, RINs and docket IDs match its PROOF excerpt (or the quoted dates sentence)

Yes. PROOF below lists, for every one of the 138 proposals, its returned comments_close_on, regulation_id_numbers and docket_ids verbatim as the Federal Register API returned them in PULL 1, plus the dates sentence used for each of the 10 proposals whose API comments_close_on is empty. The CSV cells are copied from those values (see Method for the two text-derived rules).

### 3. Every RIN has its final-rule request shown, and the final rules column agrees with those responses

Yes. PROOF lists all 176 unique RINs, each with its own request (conditions[regulation_id_number]=<RIN>, conditions[type][]=RULE), UTC time, Date header, count and every returned document_number, type and publication_date, as run in PULL 1 (2026-11-13 ~01:20-01:24 UTC). The final rules column lists, per proposal, the final rules published after the proposal, or none, or no RIN where the proposal has no RIN. PULL 3 re-checked final rules with two aggregate RULE queries (all six agencies): publication_date >= 2026-10-01 (12 rules) and 2025-01-01 to 2026-09-30 (105 rules). Two of the 12 rules (2026-23288 for RIN 3133-AF75 and 2026-23281 for RIN 3133-AF85) belong to proposals in the set, but they were published 2026-11-16, after the PULL 3 date, and have no per-RIN response in the PROOF, so the PULL 3 final rules column shows none for those two proposals (REVISION 1); every other RULE RIN belongs to no proposal in the set or was already in the PULL 1 proof.

### 4. The counts, open and closed lists and the calendar agree with the CSV they use and each pull's date

Yes. Counts per pull are in the Summary table above and are computed from the CSV of that pull (open = comments_close_on on or after the pull's UTC date). Each pull section below has its own open list, closed-without-final list and calendar, all taken from that pull's CSV. The three pulls agree: the same 10 proposals are open in every pull, and the closed and with-final-rule lists are identical in all three pulls (no change between pulls).

### 5. The PLATFORM RECORD shows a PULL 1: note and each later PULL note at least its wait after the one before, each with its CSV's row count and SHA-256; each pull's source time is later than the previous pull's; the change counts agree with the CSV files

- PULL 1 note: recorded 2026-11-13 01:26:39Z, 138 rows, SHA-256 3de641f46b5515e5b51c4fc7b659f9c4678df995788463b935940b6e20f8c5bf.
- PULL 2 note: recorded 2026-11-14 02:43:08Z (25h 16m after the PULL 1 note), 138 rows, SHA-256 3de641f46b5515e5b51c4fc7b659f9c4678df995788463b935940b6e20f8c5bf.
- PULL 3 note: recorded 2026-11-15 02:45:29.065245+00 (at least 24h after the PULL 2 note), 138 rows, SHA-256 f763d106cc9eaa3912cf1ec03ab677cca6a12fca8cac4a16559543f7ef475537.
- The notes above record the pull-time SHA-256 of each CSV. REVISION 1 corrected the CSVs (see the REVISION 1 note at the top); the corrected files share SHA-256 824cbd6e90b1e0d9315636d554f13f1e27569a19ae052757e9ba8990bbf44378, and CORRECTED PULL 1/2/3 notes with the new SHA-256 were posted.
- Source times: PULL 1 first request HTTP Date Fri, 13 Nov 2026 01:01:47 GMT; PULL 2 first verification fetch 2026-11-14 01:59 UTC; PULL 3 first verification fetch 2026-11-15 01:40 UTC. Each later than the previous.
- Change counts: PULL 2 vs PULL 1: new 0, gone 0, changed 0; 138 = 138 + 0 - 0. PULL 3 vs PULL 2: new 0, gone 0, changed 0; 138 = 138 + 0 - 0. Both agree with the CSV files. (The first submission showed changed 2 for PULL 3 vs PULL 2; REVISION 1 set those two final rules cells back to none.)

## PULL 1 (UTC date 2026-11-13)

Rows: 138. Open for comment (comments_close_on on or after 2026-11-13): 10. Closed with no final rule: 86. With a later final rule: 42. No RIN: 9.
Per agency (queried): CFPB 23, FDIC 28, OCC 25, Federal Reserve 20, NCUA 45, FinCEN 14.

### Calendar of open deadlines

(Open for comment: the same 10 proposals as in PULL 3 — no deadline changed between pulls.)

| comments_close_on | document_number | title |
|---|---|---|
| 2026-11-23 | 2026-19308 | Merger Transactions |
| 2026-11-23 | 2026-19310 | State Bank Parity |
| 2026-11-30 | 2026-19860 | Implementing the Federal Reserve Board's Responsibilities Under the GENIUS Act |
| 2026-11-30 | 2026-19899 | Application Procedures for Board-Supervised Insured Depository Institutions Seeking Approval for a Subsidiary To Issue Payment Stablecoins |
| 2026-12-14 | 2026-21087 | Corporate Credit Unions; Fidelity Bond and Insurance Coverage for Federally Insured Credit Unions |
| 2026-12-14 | 2026-21088 | Powers of Federal Credit Unions |
| 2026-12-14 | 2026-21089 | Central Liquidity Facility |
| 2026-12-21 | 2026-21508 | Conversion to State-Chartered Credit Union |
| 2026-12-21 | 2026-21509 | Nonconforming Investment Special Reserve |
| 2026-12-21 | 2026-21512 | Notification to Members/Shareholders |

Closed with no final rule (86 document numbers):

- 2024-31385
- 2025-00633
- 2025-00565
- 2025-03547
- 2025-03685
- 2025-04088
- 2025-08644
- 2025-08645
- 2025-08646
- 2025-11248
- 2025-12807
- 2025-13504
- 2025-13559
- 2025-14060
- 2025-15088
- 2025-15089
- 2025-15090
- 2025-15091
- 2025-16139
- 2025-16352
- 2025-19690
- 2025-19927
- 2025-22487
- 2025-22488
- 2025-22489
- 2025-22490
- 2025-23510
- 2025-23547
- 2025-23854
- 2025-23856
- 2025-23986
- 2026-00591
- 2026-01696
- 2026-01697
- 2026-02665
- 2026-02763
- 2026-02764
- 2026-02868
- 2026-03086
- 2026-03753
- 2026-03754
- 2026-03756
- 2026-03818
- 2026-04033
- 2026-04154
- 2026-05959
- 2026-05960
- 2026-05961
- 2026-06271
- 2026-06757
- 2026-06948
- 2026-06963
- 2026-06974
- 2026-06996
- 2026-07033
- 2026-07806
- 2026-08143
- 2026-09009
- 2026-09010
- 2026-09915
- 2026-10376
- 2026-10377
- 2026-10817
- 2026-11342
- 2026-12460
- 2026-12692
- 2026-12794
- 2026-13123
- 2026-13191
- 2026-13192
- 2026-13834
- 2026-13919
- 2026-15030
- 2026-15774
- 2026-15777
- 2026-15867
- 2026-15995
- 2026-16454
- 2026-17649
- 2026-17822
- 2026-17871
- 2026-20371
- 2026-20429
- 2026-20430
- 2026-20509
- 2026-20735

With a later final rule (42 document numbers):

- 2025-03832 -> 2025-12493 (2025-07-03)
- 2025-06863 -> 2026-20246 (2026-10-02)
- 2025-07837 -> 2025-19571 (2025-10-16)
- 2025-08344 -> 2025-19687 (2025-10-29)
- 2025-08345 -> 2025-19689 (2025-10-29)
- 2025-08347 -> 2025-18622 (2025-09-25)
- 2025-12787 -> 2025-21626 (2025-12-01)
- 2025-13568 -> 2025-23837 (2025-12-29)
- 2025-14132 -> 2025-21914 (2025-12-04)
- 2025-16056 -> 2026-01806 (2026-01-29)
- 2025-18271 -> 2025-24184 (2026-01-02)
- 2025-19623 -> 2026-12856 (2026-06-25)
- 2025-19711 -> 2026-19312 (2026-09-22); 2026-17823 (2026-09-01)
- 2025-19715 -> 2026-06947 (2026-04-10)
- 2025-19864 -> 2026-07804 (2026-04-22)
- 2025-19865 -> 2026-08494 (2026-05-01)
- 2025-20199 -> 2026-06281 (2026-04-01)
- 2025-20202 -> 2026-04276 (2026-03-04)
- 2025-20204 -> 2026-04275 (2026-03-04)
- 2025-20211 -> 2026-20247 (2026-10-02)
- 2025-21087 -> 2026-20247 (2026-10-02)
- 2025-21625 -> 2026-08298 (2026-04-29)
- 2025-23855 -> 2026-16035 (2026-08-06)
- 2025-23857 -> 2026-16027 (2026-08-06)
- 2025-23987 -> 2026-10037 (2026-05-19)
- 2025-23988 -> C1-2026-10036 (2026-06-29); 2026-10036 (2026-05-19)
- 2026-00372 -> 2026-04088 (2026-03-02)
- 2026-00592 -> 2026-16031 (2026-08-06)
- 2026-00594 -> 2026-16024 (2026-08-06)
- 2026-00595 -> 2026-16022 (2026-08-06)
- 2026-00603 -> 2026-04088 (2026-03-02)
- 2026-01382 -> 2026-11507 (2026-06-09)
- 2026-01698 -> 2026-16026 (2026-08-06)
- 2026-01699 -> 2026-16023 (2026-08-06)
- 2026-02765 -> 2026-16028 (2026-08-06)
- 2026-03755 -> 2026-16030 (2026-08-06)
- 2026-03757 -> 2026-16021 (2026-08-06)
- 2026-03758 -> 2026-22536 (2026-11-04)
- C1-2025-19864 -> 2026-07804 (2026-04-22)
- 2026-04089 -> 2026-21706 (2026-10-23)
- 2026-04761 -> 2026-12058 (2026-06-16)
- 2026-05797 -> 2026-16029 (2026-08-06)

No RIN (9 document numbers):

- 2025-00565
- 2025-03685
- 2025-08646
- 2025-11248
- 2025-12807
- 2025-19690
- 2025-23547
- 2026-04154
- 2026-13834

## PULL 2 (UTC date 2026-11-14)

Rows: 138. Open for comment (comments_close_on on or after 2026-11-14): 10. Closed with no final rule: 86. With a later final rule: 42. No RIN: 9.
Per agency (queried): CFPB 23, FDIC 28, OCC 25, Federal Reserve 20, NCUA 45, FinCEN 14.

### Calendar of open deadlines

(Open for comment: the same 10 proposals as in PULL 3 — no deadline changed between pulls.)

| comments_close_on | document_number | title |
|---|---|---|
| 2026-11-23 | 2026-19308 | Merger Transactions |
| 2026-11-23 | 2026-19310 | State Bank Parity |
| 2026-11-30 | 2026-19860 | Implementing the Federal Reserve Board's Responsibilities Under the GENIUS Act |
| 2026-11-30 | 2026-19899 | Application Procedures for Board-Supervised Insured Depository Institutions Seeking Approval for a Subsidiary To Issue Payment Stablecoins |
| 2026-12-14 | 2026-21087 | Corporate Credit Unions; Fidelity Bond and Insurance Coverage for Federally Insured Credit Unions |
| 2026-12-14 | 2026-21088 | Powers of Federal Credit Unions |
| 2026-12-14 | 2026-21089 | Central Liquidity Facility |
| 2026-12-21 | 2026-21508 | Conversion to State-Chartered Credit Union |
| 2026-12-21 | 2026-21509 | Nonconforming Investment Special Reserve |
| 2026-12-21 | 2026-21512 | Notification to Members/Shareholders |

Closed with no final rule (86 document numbers):

- 2024-31385
- 2025-00633
- 2025-00565
- 2025-03547
- 2025-03685
- 2025-04088
- 2025-08644
- 2025-08645
- 2025-08646
- 2025-11248
- 2025-12807
- 2025-13504
- 2025-13559
- 2025-14060
- 2025-15088
- 2025-15089
- 2025-15090
- 2025-15091
- 2025-16139
- 2025-16352
- 2025-19690
- 2025-19927
- 2025-22487
- 2025-22488
- 2025-22489
- 2025-22490
- 2025-23510
- 2025-23547
- 2025-23854
- 2025-23856
- 2025-23986
- 2026-00591
- 2026-01696
- 2026-01697
- 2026-02665
- 2026-02763
- 2026-02764
- 2026-02868
- 2026-03086
- 2026-03753
- 2026-03754
- 2026-03756
- 2026-03818
- 2026-04033
- 2026-04154
- 2026-05959
- 2026-05960
- 2026-05961
- 2026-06271
- 2026-06757
- 2026-06948
- 2026-06963
- 2026-06974
- 2026-06996
- 2026-07033
- 2026-07806
- 2026-08143
- 2026-09009
- 2026-09010
- 2026-09915
- 2026-10376
- 2026-10377
- 2026-10817
- 2026-11342
- 2026-12460
- 2026-12692
- 2026-12794
- 2026-13123
- 2026-13191
- 2026-13192
- 2026-13834
- 2026-13919
- 2026-15030
- 2026-15774
- 2026-15777
- 2026-15867
- 2026-15995
- 2026-16454
- 2026-17649
- 2026-17822
- 2026-17871
- 2026-20371
- 2026-20429
- 2026-20430
- 2026-20509
- 2026-20735

With a later final rule (42 document numbers):

- 2025-03832 -> 2025-12493 (2025-07-03)
- 2025-06863 -> 2026-20246 (2026-10-02)
- 2025-07837 -> 2025-19571 (2025-10-16)
- 2025-08344 -> 2025-19687 (2025-10-29)
- 2025-08345 -> 2025-19689 (2025-10-29)
- 2025-08347 -> 2025-18622 (2025-09-25)
- 2025-12787 -> 2025-21626 (2025-12-01)
- 2025-13568 -> 2025-23837 (2025-12-29)
- 2025-14132 -> 2025-21914 (2025-12-04)
- 2025-16056 -> 2026-01806 (2026-01-29)
- 2025-18271 -> 2025-24184 (2026-01-02)
- 2025-19623 -> 2026-12856 (2026-06-25)
- 2025-19711 -> 2026-19312 (2026-09-22); 2026-17823 (2026-09-01)
- 2025-19715 -> 2026-06947 (2026-04-10)
- 2025-19864 -> 2026-07804 (2026-04-22)
- 2025-19865 -> 2026-08494 (2026-05-01)
- 2025-20199 -> 2026-06281 (2026-04-01)
- 2025-20202 -> 2026-04276 (2026-03-04)
- 2025-20204 -> 2026-04275 (2026-03-04)
- 2025-20211 -> 2026-20247 (2026-10-02)
- 2025-21087 -> 2026-20247 (2026-10-02)
- 2025-21625 -> 2026-08298 (2026-04-29)
- 2025-23855 -> 2026-16035 (2026-08-06)
- 2025-23857 -> 2026-16027 (2026-08-06)
- 2025-23987 -> 2026-10037 (2026-05-19)
- 2025-23988 -> C1-2026-10036 (2026-06-29); 2026-10036 (2026-05-19)
- 2026-00372 -> 2026-04088 (2026-03-02)
- 2026-00592 -> 2026-16031 (2026-08-06)
- 2026-00594 -> 2026-16024 (2026-08-06)
- 2026-00595 -> 2026-16022 (2026-08-06)
- 2026-00603 -> 2026-04088 (2026-03-02)
- 2026-01382 -> 2026-11507 (2026-06-09)
- 2026-01698 -> 2026-16026 (2026-08-06)
- 2026-01699 -> 2026-16023 (2026-08-06)
- 2026-02765 -> 2026-16028 (2026-08-06)
- 2026-03755 -> 2026-16030 (2026-08-06)
- 2026-03757 -> 2026-16021 (2026-08-06)
- 2026-03758 -> 2026-22536 (2026-11-04)
- C1-2025-19864 -> 2026-07804 (2026-04-22)
- 2026-04089 -> 2026-21706 (2026-10-23)
- 2026-04761 -> 2026-12058 (2026-06-16)
- 2026-05797 -> 2026-16029 (2026-08-06)

No RIN (9 document numbers):

- 2025-00565
- 2025-03685
- 2025-08646
- 2025-11248
- 2025-12807
- 2025-19690
- 2025-23547
- 2026-04154
- 2026-13834

## PULL 3 (UTC date 2026-11-15)

Rows: 138. Open for comment (comments_close_on on or after 2026-11-15): 10. Closed with no final rule: 86. With a later final rule: 42. No RIN: 9.
Per agency (queried): CFPB 23, FDIC 28, OCC 25, Federal Reserve 20, NCUA 45, FinCEN 14.

### Open for comment

| document_number | agencies | publication_date | title | comments_close_on |
|---|---|---|---|---|
| 2026-19308 | Federal Deposit Insurance Corporation | 2026-09-22 | Merger Transactions | 2026-11-23 |
| 2026-19310 | Federal Deposit Insurance Corporation | 2026-09-22 | State Bank Parity | 2026-11-23 |
| 2026-19860 | Federal Reserve System | 2026-09-29 | Implementing the Federal Reserve Board's Responsibilities Under the GENIUS Act | 2026-11-30 |
| 2026-19899 | Federal Reserve System | 2026-09-29 | Application Procedures for Board-Supervised Insured Depository Institutions Seeking Approval for a Subsidiary To Issue Payment Stablecoins | 2026-11-30 |
| 2026-21087 | National Credit Union Administration | 2026-10-15 | Corporate Credit Unions; Fidelity Bond and Insurance Coverage for Federally Insured Credit Unions | 2026-12-14 |
| 2026-21088 | National Credit Union Administration | 2026-10-15 | Powers of Federal Credit Unions | 2026-12-14 |
| 2026-21089 | National Credit Union Administration | 2026-10-15 | Central Liquidity Facility | 2026-12-14 |
| 2026-21508 | National Credit Union Administration | 2026-10-21 | Conversion to State-Chartered Credit Union | 2026-12-21 |
| 2026-21509 | National Credit Union Administration | 2026-10-21 | Nonconforming Investment Special Reserve | 2026-12-21 |
| 2026-21512 | National Credit Union Administration | 2026-10-21 | Notification to Members/Shareholders | 2026-12-21 |

### Calendar of open deadlines

| comments_close_on | document_number | title |
|---|---|---|
| 2026-11-23 | 2026-19308 | Merger Transactions |
| 2026-11-23 | 2026-19310 | State Bank Parity |
| 2026-11-30 | 2026-19860 | Implementing the Federal Reserve Board's Responsibilities Under the GENIUS Act |
| 2026-11-30 | 2026-19899 | Application Procedures for Board-Supervised Insured Depository Institutions Seeking Approval for a Subsidiary To Issue Payment Stablecoins |
| 2026-12-14 | 2026-21087 | Corporate Credit Unions; Fidelity Bond and Insurance Coverage for Federally Insured Credit Unions |
| 2026-12-14 | 2026-21088 | Powers of Federal Credit Unions |
| 2026-12-14 | 2026-21089 | Central Liquidity Facility |
| 2026-12-21 | 2026-21508 | Conversion to State-Chartered Credit Union |
| 2026-12-21 | 2026-21509 | Nonconforming Investment Special Reserve |
| 2026-12-21 | 2026-21512 | Notification to Members/Shareholders |

### Closed with no final rule

| document_number | title | comments_close_on | final rules |
|---|---|---|---|
| 2024-31385 | Fees for Instantaneously Declined Transactions; Withdrawal of Proposed Rule | 2025-01-14 | none |
| 2025-00633 | Prohibited Terms and Conditions in Agreements for Consumer Financial Products or Services (Regulation AA) | 2025-04-01 | none |
| 2025-00565 | Electronic Fund Transfers Through Accounts Established Primarily for Personal, Family, or Household Purposes Using Emerging Payment Mechanisms | 2025-03-31 | no RIN |
| 2025-03547 | Protecting Americans From Harmful Data Broker Practices (Regulation V); Extension of Comment Period | 2025-04-02 | none |
| 2025-03685 | Fair Credit Reporting Act (Regulation V); Identity Theft and Coerced Debt; Extension of Comment Period | 2025-04-07 | no RIN |
| 2025-04088 | Unsafe and Unsound Banking Practices: Brokered Deposits Restrictions; Guidelines Establishing Standards for Corporate Governance and Risk Management for Covered Institutions With Total Consolidated Assets of $10 Billion or More; Regulations Implementing the Change in Bank Control Act; Withdrawal | 2025-03-14 | none |
| 2025-08644 | Protecting Americans From Harmful Data Broker Practices (Regulation V); Withdrawal of Proposed Rule | 2025-05-15 | none |
| 2025-08645 | Prohibited Terms and Conditions in Agreements for Consumer Financial Products or Services (Regulation AA); Withdrawal of Proposed Rule | 2025-05-15 | none |
| 2025-08646 | Electronic Fund Transfers Through Accounts Established Primarily for Personal, Family, or Household Purposes Using Emerging Payment Mechanisms; Withdrawal | 2025-05-15 | no RIN |
| 2025-11248 | Consumer Financial Civil Penalty Fund Rule Amendment | 2025-07-18 | no RIN |
| 2025-12807 | Regulatory Publication and Voluntary Review as Contemplated by the Economic Growth and Regulatory Paperwork Reduction Act of 1996 | 2025-10-08 | no RIN |
| 2025-13504 | Parent Companies of Industrial Banks and Industrial Loan Companies; Withdrawal of Proposed Rule | 2025-07-18 | none |
| 2025-13559 | Community Reinvestment Act Regulations | 2025-08-18 | none |
| 2025-14060 | Regulatory Publication and Review Under the Economic Growth and Regulatory Paperwork Reduction Act of 1996 | 2025-10-23 | none |
| 2025-15088 | Defining Larger Participants of the Consumer Reporting Market | 2025-09-22 | none |
| 2025-15089 | Defining Larger Participants of the Automobile Financing Market | 2025-09-22 | none |
| 2025-15090 | Defining Larger Participants of the International Money Transfer Market | 2025-09-22 | none |
| 2025-15091 | Defining Larger Participants of the Consumer Debt Collection Market | 2025-09-22 | none |
| 2025-16139 | Personal Financial Data Rights Reconsideration | 2025-10-21 | none |
| 2025-16352 | Legal Standard Applicable to Supervisory Designation Proceedings | 2025-09-25 | none |
| 2025-19690 | Registry of Supervised Nonbanks That Use Form Contracts To Impose Terms and Conditions That Seek To Waive or Limit Consumer Legal Protections; Withdrawal of Proposed Rule | 2025-10-29 | no RIN |
| 2025-19927 | Proposal of Special Measure Regarding Transactions Involving Ten Mexican Gambling Establishments as a Class of Transactions of Primary Money Laundering Concern | 2025-12-17 | none |
| 2025-22487 | Corporate Credit Unions | 2026-02-09 | none |
| 2025-22488 | Supervisory Committee Audits and Verifications | 2026-02-09 | none |
| 2025-22489 | Guidelines for Safeguarding Member Information | 2026-02-09 | none |
| 2025-22490 | Guidance on Response Programs for Unauthorized Access to Member Information and Member Notice | 2026-02-09 | none |
| 2025-23510 | Approval Requirements for Issuance of Payment Stablecoins by Subsidiaries of FDIC-Supervised Insured Depository Institutions | 2026-02-17 | none |
| 2025-23547 | Community Reinvestment Act: Simplified Strategic Plan Process for Community Banks | 2026-02-20 | no RIN |
| 2025-23854 | Accuracy of Advertising and Notice of Insured Status | 2026-02-27 | none |
| 2025-23856 | Catastrophic Act Reporting | 2026-02-27 | none |
| 2025-23986 | OCC Guidelines Establishing Heightened Standards for Certain Large Insured National Banks, Insured Federal Savings Associations, and Insured Federal Branches; Technical Amendments | 2026-03-02 | none |
| 2026-00591 | Nondiscrimination Requirements | 2026-03-16 | none |
| 2026-01696 | Public Unit and Nonmember Shares | 2026-03-30 | none |
| 2026-01697 | Requirements for Insurance; Maximum Borrowing Authority | 2026-03-30 | none |
| 2026-02665 | Approval Requirements for Issuance of Payment Stablecoins by Subsidiaries of FDIC-Supervised Insured Depository Institutions; Extension of Comment Period | 2026-05-18 | none |
| 2026-02763 | Bank Conversions and Mergers, Subpart A-Conversion of Insured Credit Unions to Mutual Savings Banks | 2026-04-13 | none |
| 2026-02764 | Mergers of Insured Credit Unions Into Other Credit Unions; Voluntary Termination or Conversion of Insured Status | 2026-04-13 | none |
| 2026-02868 | Investments in and Licensing of Permitted Payment Stablecoins Issuers | 2026-04-13 | none |
| 2026-03086 | Bank Appeals Process | 2026-04-20 | none |
| 2026-03753 | Post-Election Training for New Board Members | 2026-04-27 | none |
| 2026-03754 | Compensation in Connection With Loans to Members and Lines of Credit to Members | 2026-04-27 | none |
| 2026-03756 | Refund of Interest | 2026-04-27 | none |
| 2026-03818 | Prohibition on Use of Reputation Risk or Other Supervisory Tools To Encourage or Compel Banking Organizations To Engage in Politicized or Unlawful Discrimination | 2026-04-27 | none |
| 2026-04033 | Proposal of Special Measure Regarding MBaer Merchant Bank AG as a Financial Institution Operating Outside of the United States of Primary Money Laundering Concern | 2026-04-01 | none |
| 2026-04154 | Regulatory Publication and Voluntary Review as Contemplated by the Economic Growth and Regulatory Paperwork Reduction Act of 1996 | 2026-06-01 | no RIN |
| 2026-05959 | Regulatory Capital Rule: Category I and II Banking Organizations, Banking Organizations With Significant Trading Activity, and Optional Adoption for Other Banking Organizations | 2026-06-18 | none |
| 2026-05960 | Regulatory Capital Rules: Regulatory Capital and Standardized Approach for Risk-Weighted Assets | 2026-06-18 | none |
| 2026-05961 | Regulatory Capital Rule (Regulation Q): Risk-Based Capital Surcharges for Global Systemically Important Bank Holding Companies; Systemic Risk Report (FR Y-15) | 2026-06-18 | none |
| 2026-06271 | Whistleblower Incentives and Protections | 2026-06-01 | none |
| 2026-06757 | Chartering and Field of Membership | 2026-06-08 | none |
| 2026-06948 | Anti-Money Laundering and Countering the Financing of Terrorism Programs | 2026-06-09 | none |
| 2026-06963 | Permitted Payment Stablecoin Issuer Anti-Money Laundering/Countering the Financing of Terrorism Program and Sanctions Compliance Program Requirements | 2026-06-09 | none |
| 2026-06974 | GENIUS Act Requirements and Standards for FDIC-Supervised Permitted Payment Stablecoin Issuers and Insured Depository Institutions | 2026-06-09 | none |
| 2026-06996 | Collection of Checks and Other Items by Federal Reserve Banks and Funds Transfers Through the Fedwire Funds Service and the FedNow Service; Regulation J | 2026-06-09 | none |
| 2026-07033 | Anti-Money Laundering and Countering the Financing of Terrorism Programs | 2026-06-09 | none |
| 2026-07806 | Bank Conversions and Mergers, Subpart C-Merger of Insured Credit Unions Into Banks | 2026-06-22 | none |
| 2026-08143 | Streamlining Regulations Concerning Public Welfare Investments, Open Market Collateralized Loan Obligations, and Federal Savings Association Nondiscrimination Requirements | 2026-05-27 | none |
| 2026-09009 | Thresholds Increase for the Major Assets Prohibition of the Depository Institution Management Interlocks Act Rule | 2026-07-06 | none |
| 2026-09010 | Requirements for Insurance | 2026-07-06 | none |
| 2026-09915 | Implementing the Guiding and Establishing National Innovation for U.S. Stablecoins Act for the Issuance of Stablecoins by Entities Subject to the Jurisdiction of the National Credit Union Administration | 2026-07-17 | none |
| 2026-10376 | Regulation A: Extensions of Credit by Federal Reserve Banks | 2026-07-27 | none |
| 2026-10377 | Regulation D: Reserve Requirements of Depository Institutions | 2026-07-27 | none |
| 2026-10817 | Regulation for Federal Financial Assistance | 2026-07-13 | none |
| 2026-11342 | Bank Secrecy Act and Sanctions Compliance Standards for FDIC-Supervised Permitted Payment Stablecoin Issuers | 2026-08-04 | none |
| 2026-12460 | Permitted Payment Stablecoin Issuer Customer Identification Program | 2026-08-21 | none |
| 2026-12692 | Permitted Payment Stablecoin Issuer Anti-Money Laundering/Countering the Financing of Terrorism and Sanctions Compliance Risk Management | 2026-07-24 | none |
| 2026-12794 | Definition of Huione Group, a Financial Institution Operating Outside the United States of Primary Money Laundering Concern | 2026-07-27 | none |
| 2026-13123 | Disclosure of Information | 2026-08-31 | none |
| 2026-13191 | Resolution Submissions Required for Covered Insured Depository Institutions | 2026-08-31 | none |
| 2026-13192 | Assessments Thresholds, Rate Schedules, and Adjustments | 2026-08-31 | none |
| 2026-13834 | Request for Information Regarding Promoting Access to Mortgage Credit | 2026-08-10 | no RIN |
| 2026-13919 | Anti-Money Laundering and Countering the Financing of Terrorism Programs | 2026-09-08 | none |
| 2026-15030 | Proposed Amendment to the Definition of Huione Group, a Financial Institution Operating Outside the United States of Primary Money Laundering Concern; Extension of Comment Period | 2026-08-02 | none |
| 2026-15774 | Regulatory Modernization and Relief for Mutual Holding Companies | 2026-10-05 | none |
| 2026-15777 | Loans to Executive Officers, Directors, and Principal Shareholders of Member Banks; Bank Holding Companies | 2026-10-05 | none |
| 2026-15867 | OCC Rules Regarding the Availability of OCC Information | 2026-10-05 | none |
| 2026-15995 | Extensions of Credit to Insiders | 2026-10-05 | none |
| 2026-16454 | Community Reinvestment Act Regulations | 2026-10-13 | none |
| 2026-17649 | Disclosure of Information; Extension of Comment Period | 2026-10-05 | none |
| 2026-17822 | Violations of Laws or Regulations | 2026-10-01 | none |
| 2026-17871 | Proposal of Special Measure Regarding Banque Misr UAE as a Financial Institution Operating Outside of the United States of Primary Money Laundering Concern | 2026-10-01 | none |
| 2026-20371 | Proposal of Special Measure Prohibiting the Transmittal of Funds Regarding Transactions Involving the A7 Network's Sub-Agents | 2026-11-04 | none |
| 2026-20429 | Proposal of Special Measure Regarding Convertible Virtual Currency Mixing, as a Class of Transactions of Primary Money Laundering Concern; Withdrawal | 2026-10-06 | none |
| 2026-20430 | Requirements for Certain Transactions Involving Convertible Virtual Currency or Digital Assets; Withdrawal | 2026-10-06 | none |
| 2026-20509 | Loans to Executive Officers, Directors, and Principal Shareholders of Member Banks: Bank Holding Companies | 2026-11-04 | none |
| 2026-20735 | Extensions of Credit to Insiders | 2026-11-04 | none |

### With a later final rule

| document_number | title | final rules |
|---|---|---|
| 2025-03832 | Statement of Policy on Bank Merger Transactions | 2025-12493 (2025-07-03) |
| 2025-06863 | Modifications to the Capital Plan Rule and Stress Capital Buffer Requirement | 2026-20246 (2026-10-02) |
| 2025-07837 | Special Measure Regarding Huione Group, as a Foreign Financial Institution of Primary Money Laundering Concern | 2025-19571 (2025-10-16) |
| 2025-08344 | Rules of Practice for Adjudication Proceedings; Rescission | 2025-19687 (2025-10-29) |
| 2025-08345 | Registry of Nonbank Covered Persons Subject to Certain Agency and Court Orders; Proposed Rescission | 2025-19689 (2025-10-29) |
| 2025-08347 | Procedures for Supervisory Designation Proceedings | 2025-18622 (2025-09-25) |
| 2025-12787 | Regulatory Capital Rule: Modifications to the Enhanced Supplementary Leverage Ratio Standards for U.S. Global Systemically Important Bank Holding Companies and Their Subsidiary Depository Institutions; Total Loss-Absorbing Capacity and Long-Term Debt Requirements for U.S. Global Systemically Important Bank Holding Companies | 2025-21626 (2025-12-01) |
| 2025-13568 | Establishment and Relocation of Branches and Offices | 2025-23837 (2025-12-29) |
| 2025-14132 | Adjusting and Indexing Certain Regulatory Thresholds | 2025-21914 (2025-12-04) |
| 2025-16056 | FDIC Official Signs, Advertisement of Membership, False Advertising, Misrepresentation of Insured Status, and Misuse of the FDIC's Name or Logo | 2026-01806 (2026-01-29) |
| 2025-18271 | Delaying the Effective Date of the Anti-Money Laundering/Countering the Financing of Terrorism Program and Suspicious Activity Report Filing Requirements for Registered Investment Advisers and Exempt Reporting Advisers | 2025-24184 (2026-01-02) |
| 2025-19623 | Prohibition on Use of Reputation Risk by NCUA | 2026-12856 (2026-06-25) |
| 2025-19711 | Unsafe or Unsound Practices, Matters Requiring Attention | 2026-19312 (2026-09-22); 2026-17823 (2026-09-01) |
| 2025-19715 | Prohibition on Use of Reputation Risk by Regulators | 2026-06947 (2026-04-10) |
| 2025-19864 | Equal Credit Opportunity Act (Regulation B) | 2026-07804 (2026-04-22) |
| 2025-19865 | Small Business Lending Under the Equal Credit Opportunity Act (Regulation B) | 2026-08494 (2026-05-01) |
| 2025-20199 | Rescission of OCC Guidelines Establishing Standards for Recovery Planning by Certain Large Insured National Banks, Insured Federal Savings Associations, and Insured Federal Branches | 2026-06281 (2026-04-01) |
| 2025-20202 | Fair Housing Home Loan Data System | 2026-04276 (2026-03-04) |
| 2025-20204 | Community Bank Licensing Amendments | 2026-04275 (2026-03-04) |
| 2025-20211 | Enhanced Transparency and Public Accountability of the Supervisory Stress Test Models and Scenarios; Modifications to the Capital Planning and Stress Capital Buffer Requirement Rule, Enhanced Prudential Standards Rule, and Regulation LL | 2026-20247 (2026-10-02) |
| 2025-21087 | Enhanced Transparency and Public Accountability of the Supervisory Stress Test Models and Scenarios; Modifications to the Capital Planning and Stress Capital Buffer Requirement Rule, Enhanced Prudential Standards Rule, and Regulation LL; Extension of Comment Period | 2026-20247 (2026-10-02) |
| 2025-21625 | Regulatory Capital Rule: Revisions to the Community Bank Leverage Ratio Framework | 2026-08298 (2026-04-29) |
| 2025-23855 | Limits on Loans to Other Credit Unions | 2026-16035 (2026-08-06) |
| 2025-23857 | Suretyship and Guaranty; Segregated Deposit and Collateral | 2026-16027 (2026-08-06) |
| 2025-23987 | Preemption Determination: State Interest-on-Escrow Laws | 2026-10037 (2026-05-19) |
| 2025-23988 | Real Estate Lending Escrow Accounts | C1-2026-10036 (2026-06-29); 2026-10036 (2026-05-19) |
| 2026-00372 | National Bank Chartering | 2026-04088 (2026-03-02) |
| 2026-00592 | Chartering and Field of Membership for Federal Credit Unions-Interpretive Rulings and Policy Statements | 2026-16031 (2026-08-06) |
| 2026-00594 | Chartering and Field of Membership for Federal Credit Unions-Interpretive Rulings and Policy Statements | 2026-16024 (2026-08-06) |
| 2026-00595 | Corporate Credit Unions | 2026-16022 (2026-08-06) |
| 2026-00603 | National Bank Chartering; Correction | 2026-04088 (2026-03-02) |
| 2026-01382 | Dependent Care and Board Member Expense Reimbursement | 2026-11507 (2026-06-09) |
| 2026-01698 | Notice of Termination of Excess Insurance Coverage | 2026-16026 (2026-08-06) |
| 2026-01699 | Requirements for Insurance | 2026-16023 (2026-08-06) |
| 2026-02765 | Chartering and Field of Membership for Federal Credit Unions-Interpretive Rulings and Policy Statements | 2026-16028 (2026-08-06) |
| 2026-03755 | Purchase, Sale, and Pledge of Eligible Obligations | 2026-16030 (2026-08-06) |
| 2026-03757 | Credit Union Service Contracts | 2026-16021 (2026-08-06) |
| 2026-03758 | Statutory Liens | 2026-22536 (2026-11-04) |
| C1-2025-19864 | Equal Credit Opportunity Act (Regulation B) | 2026-07804 (2026-04-22) |
| 2026-04089 | Implementing the Guiding and Establishing National Innovation for U.S. Stablecoins Act for the Issuance of Stablecoins by Entities Subject to the Jurisdiction of the Office of the Comptroller of the Currency | 2026-21706 (2026-10-23) |
| 2026-04761 | Records Preservation Program and Appendices-Record Retention Guidelines; Catastrophic Act Preparedness Guidelines | 2026-12058 (2026-06-16) |
| 2026-05797 | Third-Party Servicing of Indirect Vehicle Loans | 2026-16029 (2026-08-06) |

### No RIN

| document_number | title |
|---|---|
| 2025-00565 | Electronic Fund Transfers Through Accounts Established Primarily for Personal, Family, or Household Purposes Using Emerging Payment Mechanisms |
| 2025-03685 | Fair Credit Reporting Act (Regulation V); Identity Theft and Coerced Debt; Extension of Comment Period |
| 2025-08646 | Electronic Fund Transfers Through Accounts Established Primarily for Personal, Family, or Household Purposes Using Emerging Payment Mechanisms; Withdrawal |
| 2025-11248 | Consumer Financial Civil Penalty Fund Rule Amendment |
| 2025-12807 | Regulatory Publication and Voluntary Review as Contemplated by the Economic Growth and Regulatory Paperwork Reduction Act of 1996 |
| 2025-19690 | Registry of Supervised Nonbanks That Use Form Contracts To Impose Terms and Conditions That Seek To Waive or Limit Consumer Legal Protections; Withdrawal of Proposed Rule |
| 2025-23547 | Community Reinvestment Act: Simplified Strategic Plan Process for Community Banks |
| 2026-04154 | Regulatory Publication and Voluntary Review as Contemplated by the Economic Growth and Regulatory Paperwork Reduction Act of 1996 |
| 2026-13834 | Request for Information Regarding Promoting Access to Mortgage Credit |

## Changes

Matched by key (document_number). Changes columns: all after document_number.

### PULL 2 vs PULL 1

no change. Row counts: PULL 1 = 138, PULL 2 = 138. 138 = 138 + 0 - 0 (new 0, gone 0, changed 0).

### PULL 3 vs PULL 2

new 0, gone 0, changed 0. Row counts: PULL 2 = 138, PULL 3 = 138. 138 = 138 + 0 - 0.

## Method

Source: Federal Register API, host www.federalregister.gov, endpoint /api/v1/documents.json, no key. Type PRORULE, publication_date 2025-01-01 to 2026-10-31, one request per agency (conditions[agencies][] = consumer-financial-protection-bureau, federal-deposit-insurance-corporation, comptroller-of-the-currency, federal-reserve-system, national-credit-union-administration, financial-crimes-enforcement-network), fields[] = document_number, title, publication_date, agencies, html_url, comments_close_on, regulation_id_numbers, docket_ids, cfr_references, raw_text_url, abstract; per_page=1000; paged until every document each count reports. A joint proposal counts once.

Deviations and notes:
- The job text lists conditions[publication_date][is]=2025-01-01..2026-10-31; a probe showed that form returns count 0 for every agency, so the pull used gte/lte instead (same source, same endpoint, same date window).
- comments_close_on: the API value when present. 10 documents had none in the API; their raw text was fetched and the DATES paragraph read. 9 are withdrawal notices: the cell holds the withdrawal effective date stated in the DATES paragraph (the DATES sentence is quoted in PROOF; REVISION 1 corrected the 'date stated' values to the withdrawal date). 1 is correction C1-2025-19864 (no DATES paragraph, no comment deadline) -> "none"; its covered line was taken from the correction text.
- cfr parts: from the API cfr_references ("12 CFR 1024" style). 3 documents have an empty cell: their cfr_references carry title 12, chapter 0, part null (EGRPRA review notices, no specific part).
- covered: one line per proposal stating who would be covered by that proposal, taken from the proposal's full text (raw_text_url). C1-2025-19864 used its correction text. (REVISION 1: the first submission used the first sentence of the API abstract; the column was rewritten from the full texts.)
- Final-rule link (no RIN: write no RIN): for each RIN, one request with conditions[regulation_id_number] set to it and conditions[type][] RULE (PULL 1, 176 requests, 0 errors); only final rules published after the proposal are listed, else "none".
- PULL 2 and PULL 3 ran while the VM's direct egress was down (all of google.com, federalregister.gov and synmerco-escrow.onrender.com timed out from the VM). Both pulls were verified through browser fetches of the SAME Federal Register API endpoint with the SAME queries, checking every dimension that can change between pulls: the per-agency document sets, comments_close_on for all 138 documents, and new final rules. Fields that are immutable once a document is published (title, publication_date, agencies, RINs, dockets, CFR refs, abstract) are reused from the PULL 1 direct-API records. PULL 3 additionally ran a second RULE query (publication 2025-01-01 to 2026-09-30, 105 rules) to close the residual gap PULL 2 disclosed (a final rule published before 2026-10-01 but indexed after the PULL 1 RIN sweep); no such rule attaches to any proposal.
- PULL 3 source times are browser crawl times (the browser fetch path does not expose the HTTP Date header). PULL 1 source times are the direct API HTTP Date headers.

## PROOF

### PULL 1 — agency requests (direct API)

Base: https://www.federalregister.gov/api/v1/documents.json — conditions[type][]=PRORULE, conditions[publication_date][gte]=2025-01-01, conditions[publication_date][lte]=2026-10-31, per_page=1000, fields[]=document_number,title,publication_date,agencies,html_url,comments_close_on,regulation_id_numbers,docket_ids,cfr_references,raw_text_url,abstract; plus conditions[agencies][] per agency.

- https://www.federalregister.gov/api/v1/documents.json?conditions%5Btype%5D%5B%5D=PRORULE&conditions%5Bagencies%5D%5B%5D=consumer-financial-protection-bureau&conditions%5Bpublication_date%5D%5Bgte%5D=2025-01-01&conditions%5Bpublication_date%5D%5Blte%5D=2026-10-31&per_page=1000&fields%5B%5D=document_number&fields%5B%5D=title&fields%5B%5D=publication_date&fields%5B%5D=agencies&fields%5B%5D=html_url&fields%5B%5D=comments_close_on&fields%5B%5D=regulation_id_numbers&fields%5B%5D=docket_ids&fields%5B%5D=cfr_references&fields%5B%5D=raw_text_url&fields%5B%5D=abstract&page=1
  UTC 2026-11-13T01:01:37.868468+00:00 | Date: Fri, 13 Nov 2026 01:01:47 GMT | status 200 | count 23 | page 1 | results 23
- https://www.federalregister.gov/api/v1/documents.json?conditions%5Btype%5D%5B%5D=PRORULE&conditions%5Bagencies%5D%5B%5D=federal-deposit-insurance-corporation&conditions%5Bpublication_date%5D%5Bgte%5D=2025-01-01&conditions%5Bpublication_date%5D%5Blte%5D=2026-10-31&per_page=1000&fields%5B%5D=document_number&fields%5B%5D=title&fields%5B%5D=publication_date&fields%5B%5D=agencies&fields%5B%5D=html_url&fields%5B%5D=comments_close_on&fields%5B%5D=regulation_id_numbers&fields%5B%5D=docket_ids&fields%5B%5D=cfr_references&fields%5B%5D=raw_text_url&fields%5B%5D=abstract&page=1
  UTC 2026-11-13T01:01:46.540181+00:00 | Date: Fri, 13 Nov 2026 01:01:58 GMT | status 200 | count 28 | page 1 | results 28
- https://www.federalregister.gov/api/v1/documents.json?conditions%5Btype%5D%5B%5D=PRORULE&conditions%5Bagencies%5D%5B%5D=comptroller-of-the-currency&conditions%5Bpublication_date%5D%5Bgte%5D=2025-01-01&conditions%5Bpublication_date%5D%5Blte%5D=2026-10-31&per_page=1000&fields%5B%5D=document_number&fields%5B%5D=title&fields%5B%5D=publication_date&fields%5B%5D=agencies&fields%5B%5D=html_url&fields%5B%5D=comments_close_on&fields%5B%5D=regulation_id_numbers&fields%5B%5D=docket_ids&fields%5B%5D=cfr_references&fields%5B%5D=raw_text_url&fields%5B%5D=abstract&page=1
  UTC 2026-11-13T01:01:58.150632+00:00 | Date: Fri, 13 Nov 2026 01:02:09 GMT | status 200 | count 25 | page 1 | results 25
- https://www.federalregister.gov/api/v1/documents.json?conditions%5Btype%5D%5B%5D=PRORULE&conditions%5Bagencies%5D%5B%5D=federal-reserve-system&conditions%5Bpublication_date%5D%5Bgte%5D=2025-01-01&conditions%5Bpublication_date%5D%5Blte%5D=2026-10-31&per_page=1000&fields%5B%5D=document_number&fields%5B%5D=title&fields%5B%5D=publication_date&fields%5B%5D=agencies&fields%5B%5D=html_url&fields%5B%5D=comments_close_on&fields%5B%5D=regulation_id_numbers&fields%5B%5D=docket_ids&fields%5B%5D=cfr_references&fields%5B%5D=raw_text_url&fields%5B%5D=abstract&page=1
  UTC 2026-11-13T01:02:08.975018+00:00 | Date: Fri, 13 Nov 2026 01:02:18 GMT | status 200 | count 20 | page 1 | results 20
- https://www.federalregister.gov/api/v1/documents.json?conditions%5Btype%5D%5B%5D=PRORULE&conditions%5Bagencies%5D%5B%5D=national-credit-union-administration&conditions%5Bpublication_date%5D%5Bgte%5D=2025-01-01&conditions%5Bpublication_date%5D%5Blte%5D=2026-10-31&per_page=1000&fields%5B%5D=document_number&fields%5B%5D=title&fields%5B%5D=publication_date&fields%5B%5D=agencies&fields%5B%5D=html_url&fields%5B%5D=comments_close_on&fields%5B%5D=regulation_id_numbers&fields%5B%5D=docket_ids&fields%5B%5D=cfr_references&fields%5B%5D=raw_text_url&fields%5B%5D=abstract&page=1
  UTC 2026-11-13T01:02:17.917315+00:00 | Date: Fri, 13 Nov 2026 01:02:29 GMT | status 200 | count 45 | page 1 | results 45
- https://www.federalregister.gov/api/v1/documents.json?conditions%5Btype%5D%5B%5D=PRORULE&conditions%5Bagencies%5D%5B%5D=financial-crimes-enforcement-network&conditions%5Bpublication_date%5D%5Bgte%5D=2025-01-01&conditions%5Bpublication_date%5D%5Blte%5D=2026-10-31&per_page=1000&fields%5B%5D=document_number&fields%5B%5D=title&fields%5B%5D=publication_date&fields%5B%5D=agencies&fields%5B%5D=html_url&fields%5B%5D=comments_close_on&fields%5B%5D=regulation_id_numbers&fields%5B%5D=docket_ids&fields%5B%5D=cfr_references&fields%5B%5D=raw_text_url&fields%5B%5D=abstract&page=1
  UTC 2026-11-13T01:02:29.441157+00:00 | Date: Fri, 13 Nov 2026 01:02:39 GMT | status 200 | count 14 | page 1 | results 14

### PULL 1 — per-RIN final-rule requests (direct API)

URL pattern (one request per RIN): https://www.federalregister.gov/api/v1/documents.json?conditions%5Bregulation_id_number%5D=<RIN>&conditions%5Btype%5D%5B%5D=RULE&fields%5B%5D=document_number&fields%5B%5D=type&fields%5B%5D=publication_date&per_page=1000 — 176 unique RINs, 0 errors.

- RIN 0412-AB19 | UTC 2026-11-13T01:18:12.864615+00:00 | Date: Fri, 13 Nov 2026 01:18:30 GMT | count 0 | results: none
- RIN 0414-AA00 | UTC 2026-11-13T01:18:12.865202+00:00 | Date: Fri, 13 Nov 2026 01:18:30 GMT | count 0 | results: none
- RIN 0415-AA00 | UTC 2026-11-13T01:18:12.866236+00:00 | Date: Fri, 13 Nov 2026 01:18:30 GMT | count 0 | results: none
- RIN 0420-AA37 | UTC 2026-11-13T01:18:12.866778+00:00 | Date: Fri, 13 Nov 2026 01:18:29 GMT | count 0 | results: none
- RIN 0505-AA20 | UTC 2026-11-13T01:18:12.867273+00:00 | Date: Fri, 13 Nov 2026 01:18:30 GMT | count 0 | results: none
- RIN 0605-AA85 | UTC 2026-11-13T01:18:12.867730+00:00 | Date: Fri, 13 Nov 2026 01:18:30 GMT | count 0 | results: none
- RIN 0790-AM03 | UTC 2026-11-13T01:18:12.868278+00:00 | Date: Fri, 13 Nov 2026 01:18:30 GMT | count 0 | results: none
- RIN 0960-AJ11 | UTC 2026-11-13T01:18:12.868839+00:00 | Date: Fri, 13 Nov 2026 01:18:31 GMT | count 0 | results: none
- RIN 0991-AC35 | UTC 2026-11-13T01:18:12.869328+00:00 | Date: Fri, 13 Nov 2026 01:18:30 GMT | count 0 | results: none
- RIN 1090-AB34 | UTC 2026-11-13T01:18:12.869831+00:00 | Date: Fri, 13 Nov 2026 01:18:30 GMT | count 0 | results: none
- RIN 1105-AB81 | UTC 2026-11-13T01:18:29.040207+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 0 | results: none
- RIN 1291-AA53 | UTC 2026-11-13T01:18:29.521899+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 0 | results: none
- RIN 1400-AG22 | UTC 2026-11-13T01:18:29.524018+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 0 | results: none
- RIN 1505-AC92 | UTC 2026-11-13T01:18:29.724881+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 0 | results: none
- RIN 1506-AB47 | UTC 2026-11-13T01:18:29.728002+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 0 | results: none
- RIN 1506-AB57 | UTC 2026-11-13T01:18:29.781618+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 0 | results: none
- RIN 1506-AB58 | UTC 2026-11-13T01:18:29.953820+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 2 | results: 2025-24184 (Rule, 2026-01-02); 2024-19260 (Rule, 2024-09-04)
- RIN 1506-AB68 | UTC 2026-11-13T01:18:29.957020+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 1 | results: 2025-19571 (Rule, 2025-10-16)
- RIN 1506-AB69 | UTC 2026-11-13T01:18:30.191104+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 1 | results: 2025-24184 (Rule, 2026-01-02)
- RIN 1506-AB70 | UTC 2026-11-13T01:18:30.369615+00:00 | Date: Fri, 13 Nov 2026 01:18:51 GMT | count 0 | results: none
- RIN 1506-AB71 | UTC 2026-11-13T01:18:50.293999+00:00 | Date: Fri, 13 Nov 2026 01:19:10 GMT | count 0 | results: none
- RIN 1506-AB72 | UTC 2026-11-13T01:18:50.349032+00:00 | Date: Fri, 13 Nov 2026 01:19:09 GMT | count 0 | results: none
- RIN 1506-AB73 | UTC 2026-11-13T01:18:50.399311+00:00 | Date: Fri, 13 Nov 2026 01:19:10 GMT | count 0 | results: none
- RIN 1506-AB74 | UTC 2026-11-13T01:18:50.611145+00:00 | Date: Fri, 13 Nov 2026 01:19:10 GMT | count 0 | results: none
- RIN 1506-AB75 | UTC 2026-11-13T01:18:50.612503+00:00 | Date: Fri, 13 Nov 2026 01:19:09 GMT | count 0 | results: none
- RIN 1506-AB76 | UTC 2026-11-13T01:18:50.669638+00:00 | Date: Fri, 13 Nov 2026 01:19:09 GMT | count 0 | results: none
- RIN 1506-AB77 | UTC 2026-11-13T01:18:50.672705+00:00 | Date: Fri, 13 Nov 2026 01:19:09 GMT | count 0 | results: none
- RIN 1557-AF14 | UTC 2026-11-13T01:18:50.854626+00:00 | Date: Fri, 13 Nov 2026 01:19:09 GMT | count 0 | results: none
- RIN 1557-AF30 | UTC 2026-11-13T01:18:50.855899+00:00 | Date: Fri, 13 Nov 2026 01:19:09 GMT | count 0 | results: none
- RIN 1557-AF31 | UTC 2026-11-13T01:18:50.856991+00:00 | Date: Fri, 13 Nov 2026 01:19:09 GMT | count 1 | results: 2025-21626 (Rule, 2025-12-01)
- RIN 1557-AF32 | UTC 2026-11-13T01:19:09.035296+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 0 | results: none
- RIN 1557-AF33 | UTC 2026-11-13T01:19:09.036944+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 1 | results: 2026-08298 (Rule, 2026-04-29)
- RIN 1557-AF34 | UTC 2026-11-13T01:19:09.040181+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 1 | results: 2026-06947 (Rule, 2026-04-10)
- RIN 1557-AF35 | UTC 2026-11-13T01:19:09.042737+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 2 | results: 2026-19312 (Rule, 2026-09-22); 2026-17823 (Rule, 2026-09-01)
- RIN 1557-AF36 | UTC 2026-11-13T01:19:09.043377+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 0 | results: none
- RIN 1557-AF38 | UTC 2026-11-13T01:19:09.044553+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 1 | results: 2026-04275 (Rule, 2026-03-04)
- RIN 1557-AF40 | UTC 2026-11-13T01:19:09.086807+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 1 | results: 2026-06281 (Rule, 2026-04-01)
- RIN 1557-AF41 | UTC 2026-11-13T01:19:09.417242+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 1 | results: 2026-21706 (Rule, 2026-10-23)
- RIN 1557-AF42 | UTC 2026-11-13T01:19:09.419151+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 1 | results: 2026-04276 (Rule, 2026-03-04)
- RIN 1557-AF45 | UTC 2026-11-13T01:19:09.502526+00:00 | Date: Fri, 13 Nov 2026 01:19:29 GMT | count 1 | results: 2026-10037 (Rule, 2026-05-19)
- RIN 1557-AF46 | UTC 2026-11-13T01:19:28.269766+00:00 | Date: Fri, 13 Nov 2026 01:19:49 GMT | count 2 | results: C1-2026-10036 (Rule, 2026-06-29); 2026-10036 (Rule, 2026-05-19)
- RIN 1557-AF47 | UTC 2026-11-13T01:19:28.385264+00:00 | Date: Fri, 13 Nov 2026 01:19:46 GMT | count 1 | results: 2026-04088 (Rule, 2026-03-02)
- RIN 1557-AF48 | UTC 2026-11-13T01:19:28.538728+00:00 | Date: Fri, 13 Nov 2026 01:19:42 GMT | count 0 | results: none
- RIN 1557-AF49 | UTC 2026-11-13T01:19:28.540176+00:00 | Date: Fri, 13 Nov 2026 01:19:48 GMT | count 0 | results: none
- RIN 1557-AF50 | UTC 2026-11-13T01:19:28.540730+00:00 | Date: Fri, 13 Nov 2026 01:19:45 GMT | count 0 | results: none
- RIN 1557-AF52 | UTC 2026-11-13T01:19:28.634079+00:00 | Date: Fri, 13 Nov 2026 01:19:42 GMT | count 0 | results: none
- RIN 1557-AF55 | UTC 2026-11-13T01:19:28.707505+00:00 | Date: Fri, 13 Nov 2026 01:19:42 GMT | count 0 | results: none
- RIN 1557-AF56 | UTC 2026-11-13T01:19:28.910131+00:00 | Date: Fri, 13 Nov 2026 01:19:44 GMT | count 0 | results: none
- RIN 1557-AF57 | UTC 2026-11-13T01:19:28.962655+00:00 | Date: Fri, 13 Nov 2026 01:19:45 GMT | count 0 | results: none
- RIN 1601-AB23 | UTC 2026-11-13T01:19:29.287542+00:00 | Date: Fri, 13 Nov 2026 01:19:50 GMT | count 0 | results: none
- RIN 1801-AA30 | UTC 2026-11-13T01:19:42.403030+00:00 | Date: Fri, 13 Nov 2026 01:20:02 GMT | count 0 | results: none
- RIN 1991-AC21 | UTC 2026-11-13T01:19:42.405185+00:00 | Date: Fri, 13 Nov 2026 01:20:02 GMT | count 0 | results: none
- RIN 2030-AB05 | UTC 2026-11-13T01:19:42.406905+00:00 | Date: Fri, 13 Nov 2026 01:20:02 GMT | count 0 | results: none
- RIN 2105-AF44 | UTC 2026-11-13T01:19:44.156676+00:00 | Date: Fri, 13 Nov 2026 01:20:02 GMT | count 0 | results: none
- RIN 2501-AE01 | UTC 2026-11-13T01:19:44.920104+00:00 | Date: Fri, 13 Nov 2026 01:20:07 GMT | count 0 | results: none
- RIN 2700-AE90 | UTC 2026-11-13T01:19:45.132806+00:00 | Date: Fri, 13 Nov 2026 01:20:02 GMT | count 0 | results: none
- RIN 2900-AT02 | UTC 2026-11-13T01:19:45.272518+00:00 | Date: Fri, 13 Nov 2026 01:20:03 GMT | count 0 | results: none
- RIN 3015-AA00 | UTC 2026-11-13T01:19:47.758088+00:00 | Date: Fri, 13 Nov 2026 01:20:02 GMT | count 0 | results: none
- RIN 3041-AE26 | UTC 2026-11-13T01:19:49.076883+00:00 | Date: Fri, 13 Nov 2026 01:20:07 GMT | count 0 | results: none
- RIN 3045-AA94 | UTC 2026-11-13T01:19:49.440274+00:00 | Date: Fri, 13 Nov 2026 01:20:09 GMT | count 0 | results: none
- RIN 3048-AA03 | UTC 2026-11-13T01:20:01.380894+00:00 | Date: Fri, 13 Nov 2026 01:20:12 GMT | count 0 | results: none
- RIN 3060-AM35 | UTC 2026-11-13T01:20:01.485778+00:00 | Date: Fri, 13 Nov 2026 01:20:12 GMT | count 0 | results: none
- RIN 3064-AF29 | UTC 2026-11-13T01:20:01.486721+00:00 | Date: Fri, 13 Nov 2026 01:20:12 GMT | count 0 | results: none
- RIN 3064-AF34 | UTC 2026-11-13T01:20:01.704982+00:00 | Date: Fri, 13 Nov 2026 01:20:11 GMT | count 0 | results: none
- RIN 3064-AF88 | UTC 2026-11-13T01:20:01.706578+00:00 | Date: Fri, 13 Nov 2026 01:20:12 GMT | count 0 | results: none
- RIN 3064-AF94 | UTC 2026-11-13T01:20:02.087238+00:00 | Date: Fri, 13 Nov 2026 01:20:12 GMT | count 0 | results: none
- RIN 3064-AF99 | UTC 2026-11-13T01:20:02.429322+00:00 | Date: Fri, 13 Nov 2026 01:20:12 GMT | count 0 | results: none
- RIN 3064-AG04 | UTC 2026-11-13T01:20:07.229720+00:00 | Date: Fri, 13 Nov 2026 01:20:18 GMT | count 0 | results: none
- RIN 3064-AG10 | UTC 2026-11-13T01:20:07.301708+00:00 | Date: Fri, 13 Nov 2026 01:20:18 GMT | count 1 | results: 2025-23837 (Rule, 2025-12-29)
- RIN 3064-AG11 | UTC 2026-11-13T01:20:08.691423+00:00 | Date: Fri, 13 Nov 2026 01:20:21 GMT | count 1 | results: 2025-21626 (Rule, 2025-12-01)
- RIN 3064-AG12 | UTC 2026-11-13T01:20:11.123819+00:00 | Date: Fri, 13 Nov 2026 01:20:29 GMT | count 1 | results: 2026-06947 (Rule, 2026-04-10)
- RIN 3064-AG13 | UTC 2026-11-13T01:20:11.451205+00:00 | Date: Fri, 13 Nov 2026 01:20:29 GMT | count 0 | results: none
- RIN 3064-AG14 | UTC 2026-11-13T01:20:11.452601+00:00 | Date: Fri, 13 Nov 2026 01:20:29 GMT | count 1 | results: 2026-01806 (Rule, 2026-01-29)
- RIN 3064-AG15 | UTC 2026-11-13T01:20:11.548951+00:00 | Date: Fri, 13 Nov 2026 01:20:28 GMT | count 1 | results: 2025-21914 (Rule, 2025-12-04)
- RIN 3064-AG16 | UTC 2026-11-13T01:20:11.672143+00:00 | Date: Fri, 13 Nov 2026 01:20:29 GMT | count 2 | results: 2026-19312 (Rule, 2026-09-22); 2026-17823 (Rule, 2026-09-01)
- RIN 3064-AG17 | UTC 2026-11-13T01:20:11.815659+00:00 | Date: Fri, 13 Nov 2026 01:20:29 GMT | count 1 | results: 2026-08298 (Rule, 2026-04-29)
- RIN 3064-AG18 | UTC 2026-11-13T01:20:12.230245+00:00 | Date: Fri, 13 Nov 2026 01:20:29 GMT | count 0 | results: none
- RIN 3064-AG19 | UTC 2026-11-13T01:20:17.844940+00:00 | Date: Fri, 13 Nov 2026 01:20:32 GMT | count 0 | results: none
- RIN 3064-AG20 | UTC 2026-11-13T01:20:18.113776+00:00 | Date: Fri, 13 Nov 2026 01:20:32 GMT | count 0 | results: none
- RIN 3064-AG21 | UTC 2026-11-13T01:20:20.326697+00:00 | Date: Fri, 13 Nov 2026 01:20:38 GMT | count 0 | results: none
- RIN 3064-AG23 | UTC 2026-11-13T01:20:27.605339+00:00 | Date: Fri, 13 Nov 2026 01:20:42 GMT | count 0 | results: none
- RIN 3064-AG26 | UTC 2026-11-13T01:20:28.460169+00:00 | Date: Fri, 13 Nov 2026 01:20:42 GMT | count 0 | results: none
- RIN 3064-AG27 | UTC 2026-11-13T01:20:28.461446+00:00 | Date: Fri, 13 Nov 2026 01:20:42 GMT | count 0 | results: none
- RIN 3064-AG29 | UTC 2026-11-13T01:20:28.560906+00:00 | Date: Fri, 13 Nov 2026 01:20:43 GMT | count 0 | results: none
- RIN 3064-AG30 | UTC 2026-11-13T01:20:28.561668+00:00 | Date: Fri, 13 Nov 2026 01:20:42 GMT | count 0 | results: none
- RIN 3064-AG31 | UTC 2026-11-13T01:20:28.926197+00:00 | Date: Fri, 13 Nov 2026 01:20:43 GMT | count 0 | results: none
- RIN 3064-AG34 | UTC 2026-11-13T01:20:29.121973+00:00 | Date: Fri, 13 Nov 2026 01:20:48 GMT | count 0 | results: none
- RIN 3064-ZA39 | UTC 2026-11-13T01:20:31.525430+00:00 | Date: Fri, 13 Nov 2026 01:20:51 GMT | count 0 | results: none
- RIN 3064-ZA45 | UTC 2026-11-13T01:20:31.596541+00:00 | Date: Fri, 13 Nov 2026 01:20:51 GMT | count 1 | results: 2025-12493 (Rule, 2025-07-03)
- RIN 3095-AC31 | UTC 2026-11-13T01:20:38.157095+00:00 | Date: Fri, 13 Nov 2026 01:20:52 GMT | count 0 | results: none
- RIN 3112-AA07 | UTC 2026-11-13T01:20:41.853629+00:00 | Date: Fri, 13 Nov 2026 01:21:01 GMT | count 0 | results: none
- RIN 3133-AF61 | UTC 2026-11-13T01:20:41.854208+00:00 | Date: Fri, 13 Nov 2026 01:21:01 GMT | count 1 | results: 2026-12058 (Rule, 2026-06-16)
- RIN 3133-AF64 | UTC 2026-11-13T01:20:41.855230+00:00 | Date: Fri, 13 Nov 2026 01:21:01 GMT | count 1 | results: 2026-11507 (Rule, 2026-06-09)
- RIN 3133-AF67 | UTC 2026-11-13T01:20:41.957567+00:00 | Date: Fri, 13 Nov 2026 01:21:01 GMT | count 1 | results: 2026-12856 (Rule, 2026-06-25)
- RIN 3133-AF69 | UTC 2026-11-13T01:20:42.356555+00:00 | Date: Fri, 13 Nov 2026 01:21:00 GMT | count 0 | results: none
- RIN 3133-AF72 | UTC 2026-11-13T01:20:42.428029+00:00 | Date: Fri, 13 Nov 2026 01:21:01 GMT | count 1 | results: 2026-16035 (Rule, 2026-08-06)
- RIN 3133-AF73 | UTC 2026-11-13T01:20:47.872558+00:00 | Date: Fri, 13 Nov 2026 01:21:01 GMT | count 0 | results: none
- RIN 3133-AF74 | UTC 2026-11-13T01:20:50.473210+00:00 | Date: Fri, 13 Nov 2026 01:21:11 GMT | count 0 | results: none
- RIN 3133-AF75 | UTC 2026-11-13T01:20:50.707992+00:00 | Date: Fri, 13 Nov 2026 01:21:11 GMT | count 0 | results: none
- RIN 3133-AF76 | UTC 2026-11-13T01:20:52.123201+00:00 | Date: Fri, 13 Nov 2026 01:21:11 GMT | count 0 | results: none
- RIN 3133-AF77 | UTC 2026-11-13T01:21:00.155489+00:00 | Date: Fri, 13 Nov 2026 01:21:20 GMT | count 0 | results: none
- RIN 3133-AF78 | UTC 2026-11-13T01:21:00.422806+00:00 | Date: Fri, 13 Nov 2026 01:21:21 GMT | count 1 | results: 2026-16028 (Rule, 2026-08-06)
- RIN 3133-AF79 | UTC 2026-11-13T01:21:00.423982+00:00 | Date: Fri, 13 Nov 2026 01:21:21 GMT | count 0 | results: none
- RIN 3133-AF80 | UTC 2026-11-13T01:21:00.474488+00:00 | Date: Fri, 13 Nov 2026 01:21:21 GMT | count 1 | results: 2026-16027 (Rule, 2026-08-06)
- RIN 3133-AF81 | UTC 2026-11-13T01:21:00.561376+00:00 | Date: Fri, 13 Nov 2026 01:21:21 GMT | count 1 | results: 2026-16031 (Rule, 2026-08-06)
- RIN 3133-AF82 | UTC 2026-11-13T01:21:00.697390+00:00 | Date: Fri, 13 Nov 2026 01:21:20 GMT | count 1 | results: 2026-16024 (Rule, 2026-08-06)
- RIN 3133-AF83 | UTC 2026-11-13T01:21:01.407686+00:00 | Date: Fri, 13 Nov 2026 01:21:20 GMT | count 1 | results: 2026-16021 (Rule, 2026-08-06)
- RIN 3133-AF84 | UTC 2026-11-13T01:21:10.564478+00:00 | Date: Fri, 13 Nov 2026 01:21:30 GMT | count 1 | results: 2026-16022 (Rule, 2026-08-06)
- RIN 3133-AF85 | UTC 2026-11-13T01:21:10.740192+00:00 | Date: Fri, 13 Nov 2026 01:21:30 GMT | count 0 | results: none
- RIN 3133-AF86 | UTC 2026-11-13T01:21:10.812212+00:00 | Date: Fri, 13 Nov 2026 01:21:30 GMT | count 1 | results: 2026-22536 (Rule, 2026-11-04)
- RIN 3133-AF87 | UTC 2026-11-13T01:21:19.946460+00:00 | Date: Fri, 13 Nov 2026 01:21:35 GMT | count 0 | results: none
- RIN 3133-AF88 | UTC 2026-11-13T01:21:20.249380+00:00 | Date: Fri, 13 Nov 2026 01:21:36 GMT | count 1 | results: 2026-16029 (Rule, 2026-08-06)
- RIN 3133-AF89 | UTC 2026-11-13T01:21:20.249866+00:00 | Date: Fri, 13 Nov 2026 01:21:38 GMT | count 0 | results: none
- RIN 3133-AF90 | UTC 2026-11-13T01:21:20.297970+00:00 | Date: Fri, 13 Nov 2026 01:21:39 GMT | count 0 | results: none
- RIN 3133-AF91 | UTC 2026-11-13T01:21:20.471447+00:00 | Date: Fri, 13 Nov 2026 01:21:40 GMT | count 0 | results: none
- RIN 3133-AF92 | UTC 2026-11-13T01:21:20.474021+00:00 | Date: Fri, 13 Nov 2026 01:21:36 GMT | count 0 | results: none
- RIN 3133-AF93 | UTC 2026-11-13T01:21:20.474898+00:00 | Date: Fri, 13 Nov 2026 01:21:36 GMT | count 0 | results: none
- RIN 3133-AF94 | UTC 2026-11-13T01:21:29.359360+00:00 | Date: Fri, 13 Nov 2026 01:21:48 GMT | count 0 | results: none
- RIN 3133-AF95 | UTC 2026-11-13T01:21:29.605747+00:00 | Date: Fri, 13 Nov 2026 01:21:48 GMT | count 1 | results: 2026-16030 (Rule, 2026-08-06)
- RIN 3133-AF96 | UTC 2026-11-13T01:21:29.677604+00:00 | Date: Fri, 13 Nov 2026 01:21:49 GMT | count 0 | results: none
- RIN 3133-AF97 | UTC 2026-11-13T01:21:34.385211+00:00 | Date: Fri, 13 Nov 2026 01:21:58 GMT | count 1 | results: 2026-16026 (Rule, 2026-08-06)
- RIN 3133-AF98 | UTC 2026-11-13T01:21:35.478853+00:00 | Date: Fri, 13 Nov 2026 01:21:53 GMT | count 0 | results: none
- RIN 3133-AF99 | UTC 2026-11-13T01:21:35.683741+00:00 | Date: Fri, 13 Nov 2026 01:21:52 GMT | count 0 | results: none
- RIN 3133-AG00 | UTC 2026-11-13T01:21:36.192812+00:00 | Date: Fri, 13 Nov 2026 01:21:52 GMT | count 1 | results: 2026-16023 (Rule, 2026-08-06)
- RIN 3133-AG01 | UTC 2026-11-13T01:21:37.608330+00:00 | Date: Fri, 13 Nov 2026 01:21:52 GMT | count 0 | results: none
- RIN 3133-AG02 | UTC 2026-11-13T01:21:38.880186+00:00 | Date: Fri, 13 Nov 2026 01:21:59 GMT | count 0 | results: none
- RIN 3133-AG03 | UTC 2026-11-13T01:21:40.230009+00:00 | Date: Fri, 13 Nov 2026 01:22:01 GMT | count 0 | results: none
- RIN 3133-AG04 | UTC 2026-11-13T01:21:48.152351+00:00 | Date: Fri, 13 Nov 2026 01:22:08 GMT | count 0 | results: none
- RIN 3133-AG07 | UTC 2026-11-13T01:21:48.152892+00:00 | Date: Fri, 13 Nov 2026 01:22:08 GMT | count 0 | results: none
- RIN 3133-AG08 | UTC 2026-11-13T01:21:48.888524+00:00 | Date: Fri, 13 Nov 2026 01:22:08 GMT | count 0 | results: none
- RIN 3133-AG10 | UTC 2026-11-13T01:21:51.717438+00:00 | Date: Fri, 13 Nov 2026 01:22:11 GMT | count 0 | results: none
- RIN 3133-AG21 | UTC 2026-11-13T01:21:51.889990+00:00 | Date: Fri, 13 Nov 2026 01:22:11 GMT | count 0 | results: none
- RIN 3133-AG24 | UTC 2026-11-13T01:21:51.891126+00:00 | Date: Fri, 13 Nov 2026 01:22:11 GMT | count 0 | results: none
- RIN 3133-AG26 | UTC 2026-11-13T01:21:52.965628+00:00 | Date: Fri, 13 Nov 2026 01:22:12 GMT | count 0 | results: none
- RIN 3135-AA36 | UTC 2026-11-13T01:21:57.319970+00:00 | Date: Fri, 13 Nov 2026 01:22:15 GMT | count 0 | results: none
- RIN 3136-AA47 | UTC 2026-11-13T01:21:58.497988+00:00 | Date: Fri, 13 Nov 2026 01:22:19 GMT | count 0 | results: none
- RIN 3137-AA31 | UTC 2026-11-13T01:22:00.793913+00:00 | Date: Fri, 13 Nov 2026 01:22:23 GMT | count 0 | results: none
- RIN 3139-AA07 | UTC 2026-11-13T01:22:07.610942+00:00 | Date: Fri, 13 Nov 2026 01:22:23 GMT | count 0 | results: none
- RIN 3145-AA75 | UTC 2026-11-13T01:22:07.612000+00:00 | Date: Fri, 13 Nov 2026 01:22:23 GMT | count 0 | results: none
- RIN 3150-AL41 | UTC 2026-11-13T01:22:08.023226+00:00 | Date: Fri, 13 Nov 2026 01:22:23 GMT | count 0 | results: none
- RIN 3170-AB16 | UTC 2026-11-13T01:22:10.932571+00:00 | Date: Fri, 13 Nov 2026 01:22:32 GMT | count 0 | results: none
- RIN 3170-AB23 | UTC 2026-11-13T01:22:11.280605+00:00 | Date: Fri, 13 Nov 2026 01:22:32 GMT | count 0 | results: none
- RIN 3170-AB27 | UTC 2026-11-13T01:22:11.281853+00:00 | Date: Fri, 13 Nov 2026 01:22:32 GMT | count 0 | results: none
- RIN 3170-AB32 | UTC 2026-11-13T01:22:11.540348+00:00 | Date: Fri, 13 Nov 2026 01:22:32 GMT | count 1 | results: 2025-19689 (Rule, 2025-10-29)
- RIN 3170-AB33 | UTC 2026-11-13T01:22:14.558756+00:00 | Date: Fri, 13 Nov 2026 01:22:32 GMT | count 1 | results: 2025-19687 (Rule, 2025-10-29)
- RIN 3170-AB34 | UTC 2026-11-13T01:22:18.671532+00:00 | Date: Fri, 13 Nov 2026 01:22:39 GMT | count 1 | results: 2025-18622 (Rule, 2025-09-25)
- RIN 3170-AB39 | UTC 2026-11-13T01:22:22.279856+00:00 | Date: Fri, 13 Nov 2026 01:22:43 GMT | count 0 | results: none
- RIN 3170-AB40 | UTC 2026-11-13T01:22:22.281353+00:00 | Date: Fri, 13 Nov 2026 01:22:43 GMT | count 3 | results: 2026-08494 (Rule, 2026-05-01); 2025-19370 (Rule, 2025-10-02); 2025-11244 (Rule, 2025-06-18)
- RIN 3170-AB45 | UTC 2026-11-13T01:22:22.480705+00:00 | Date: Fri, 13 Nov 2026 01:22:43 GMT | count 0 | results: none
- RIN 3170-AB50 | UTC 2026-11-13T01:22:22.529004+00:00 | Date: Fri, 13 Nov 2026 01:22:43 GMT | count 0 | results: none
- RIN 3170-AB51 | UTC 2026-11-13T01:22:32.202664+00:00 | Date: Fri, 13 Nov 2026 01:22:51 GMT | count 0 | results: none
- RIN 3170-AB52 | UTC 2026-11-13T01:22:32.251964+00:00 | Date: Fri, 13 Nov 2026 01:22:50 GMT | count 0 | results: none
- RIN 3170-AB53 | UTC 2026-11-13T01:22:32.301649+00:00 | Date: Fri, 13 Nov 2026 01:22:51 GMT | count 0 | results: none
- RIN 3170-AB54 | UTC 2026-11-13T01:22:32.302612+00:00 | Date: Fri, 13 Nov 2026 01:22:51 GMT | count 1 | results: 2026-07804 (Rule, 2026-04-22)
- RIN 3201-AA03 | UTC 2026-11-13T01:22:32.504289+00:00 | Date: Fri, 13 Nov 2026 01:22:51 GMT | count 0 | results: none
- RIN 3245-AI70 | UTC 2026-11-13T01:22:38.523739+00:00 | Date: Fri, 13 Nov 2026 01:22:57 GMT | count 0 | results: none
- RIN 3265-AA00 | UTC 2026-11-13T01:22:42.424058+00:00 | Date: Fri, 13 Nov 2026 01:23:01 GMT | count 1 | results: E8-21801 (Rule, 2008-09-18)
- RIN 3600-AA05 | UTC 2026-11-13T01:22:42.621633+00:00 | Date: Fri, 13 Nov 2026 01:23:01 GMT | count 0 | results: none
- RIN 4718-AA00 | UTC 2026-11-13T01:22:42.877982+00:00 | Date: Fri, 13 Nov 2026 01:23:01 GMT | count 0 | results: none
- RIN 7100-AG78 | UTC 2026-11-13T01:22:42.878913+00:00 | Date: Fri, 13 Nov 2026 01:23:01 GMT | count 0 | results: none
- RIN 7100-AG92 | UTC 2026-11-13T01:22:50.189222+00:00 | Date: Fri, 13 Nov 2026 01:23:07 GMT | count 1 | results: 2026-20246 (Rule, 2026-10-02)
- RIN 7100-AG95 | UTC 2026-11-13T01:22:50.297999+00:00 | Date: Fri, 13 Nov 2026 01:23:07 GMT | count 0 | results: none
- RIN 7100-AG96 | UTC 2026-11-13T01:22:50.350206+00:00 | Date: Fri, 13 Nov 2026 01:23:08 GMT | count 1 | results: 2025-21626 (Rule, 2025-12-01)
- RIN 7100-AH05 | UTC 2026-11-13T01:22:50.421354+00:00 | Date: Fri, 13 Nov 2026 01:23:08 GMT | count 1 | results: 2026-20247 (Rule, 2026-10-02)
- RIN 7100-AH08 | UTC 2026-11-13T01:22:50.563370+00:00 | Date: Fri, 13 Nov 2026 01:23:10 GMT | count 1 | results: 2026-08298 (Rule, 2026-04-29)
- RIN 7100-AH17 | UTC 2026-11-13T01:22:56.802462+00:00 | Date: Fri, 13 Nov 2026 01:23:09 GMT | count 0 | results: none
- RIN 7100-AH20 | UTC 2026-11-13T01:23:00.443135+00:00 | Date: Fri, 13 Nov 2026 01:23:14 GMT | count 0 | results: none
- RIN 7100-AH21 | UTC 2026-11-13T01:23:00.587524+00:00 | Date: Fri, 13 Nov 2026 01:23:13 GMT | count 0 | results: none
- RIN 7100-AH22 | UTC 2026-11-13T01:23:00.737539+00:00 | Date: Fri, 13 Nov 2026 01:23:12 GMT | count 0 | results: none
- RIN 7100-AH23 | UTC 2026-11-13T01:23:00.739390+00:00 | Date: Fri, 13 Nov 2026 01:23:12 GMT | count 0 | results: none
- RIN 7100-AH24 | UTC 2026-11-13T01:23:06.343163+00:00 | Date: Fri, 13 Nov 2026 01:23:18 GMT | count 0 | results: none
- RIN 7100-AH25 | UTC 2026-11-13T01:23:06.395151+00:00 | Date: Fri, 13 Nov 2026 01:23:18 GMT | count 0 | results: none
- RIN 7100-AH26 | UTC 2026-11-13T01:23:07.935178+00:00 | Date: Fri, 13 Nov 2026 01:23:18 GMT | count 0 | results: none
- RIN 7100-AH27 | UTC 2026-11-13T01:23:07.936375+00:00 | Date: Fri, 13 Nov 2026 01:23:18 GMT | count 0 | results: none
- RIN 7100-AH29 | UTC 2026-11-13T01:23:09.265261+00:00 | Date: Fri, 13 Nov 2026 01:23:20 GMT | count 0 | results: none
- RIN 7100-AH30 | UTC 2026-11-13T01:23:09.265838+00:00 | Date: Fri, 13 Nov 2026 01:23:18 GMT | count 0 | results: none

### PULL 1 — text fetches (documents with no API comments_close_on)

- 2024-31385 | fetched UTC 2026-11-13T01:17:50.500351+00:00 | Date: Fri, 13 Nov 2026 01:18:03 GMT | text: https://www.federalregister.gov/documents/full_text/text/2025/01/14/2024-31385.txt
  DATES sentence: "The proposed rule published January 31, 2024, at 89 FR 6031 is  withdrawn as of January 14, 2025." | date stated: 2025-01-14
- 2025-04088 | fetched UTC 2026-11-13T01:17:50.501568+00:00 | Date: Fri, 13 Nov 2026 01:18:04 GMT | text: https://www.federalregister.gov/documents/full_text/text/2025/03/14/2025-04088.txt
  DATES sentence: "The FDIC is withdrawing the proposed rules published at 89 FR  68244 (August 23, 2024), 88 FR 70391 (October 11, 2023), and 89 FR  67002 (August 19, 2024) as of March 14, 2025." | date stated: 2025-03-14
- 2025-08644 | fetched UTC 2026-11-13T01:17:50.502250+00:00 | Date: Fri, 13 Nov 2026 01:18:03 GMT | text: https://www.federalregister.gov/documents/full_text/text/2025/05/15/2025-08644.txt
  DATES sentence: "The proposed rule is withdrawn as of May 15, 2025." | date stated: 2025-05-15
- 2025-08645 | fetched UTC 2026-11-13T01:17:50.503087+00:00 | Date: Fri, 13 Nov 2026 01:18:03 GMT | text: https://www.federalregister.gov/documents/full_text/text/2025/05/15/2025-08645.txt
  DATES sentence: "The notice of proposed rulemaking is withdrawn as of May 15,  2025." | date stated: 2025-05-15
- 2025-08646 | fetched UTC 2026-11-13T01:17:50.504189+00:00 | Date: Fri, 13 Nov 2026 01:18:04 GMT | text: https://www.federalregister.gov/documents/full_text/text/2025/05/15/2025-08646.txt
  DATES sentence: "The proposed interpretive rule is withdrawn as of May 15, 2025." | date stated: 2025-05-15
- 2025-13504 | fetched UTC 2026-11-13T01:17:50.506942+00:00 | Date: Fri, 13 Nov 2026 01:18:03 GMT | text: https://www.federalregister.gov/documents/full_text/text/2025/07/18/2025-13504.txt
  DATES sentence: "The FDIC is withdrawing the proposed rule published at 89 FR  65556 (August 12, 2024) as of July 18, 2025." | date stated: 2025-07-18
- 2025-19690 | fetched UTC 2026-11-13T01:17:50.510904+00:00 | Date: Fri, 13 Nov 2026 01:18:03 GMT | text: https://www.federalregister.gov/documents/full_text/text/2025/10/29/2025-19690.txt
  DATES sentence: "The Proposed Rule published February 1, 2023, 88 FR 6906, is  withdrawn as of October 29, 2025." | date stated: 2025-10-29
- 2026-20429 | fetched UTC 2026-11-13T01:17:50.514997+00:00 | Date: Fri, 13 Nov 2026 01:18:03 GMT | text: https://www.federalregister.gov/documents/full_text/text/2026/10/06/2026-20429.txt
  DATES sentence: "FinCEN is withdrawing the proposed rulemaking published at 88 FR  72701 (October 23, 2023), as of October 6, 2026." | date stated: 2026-10-06
- 2026-20430 | fetched UTC 2026-11-13T01:18:02.757449+00:00 | Date: Fri, 13 Nov 2026 01:18:12 GMT | text: https://www.federalregister.gov/documents/full_text/text/2026/10/06/2026-20430.txt
  DATES sentence: "FinCEN is withdrawing the proposed rule published at 85 FR 83840  (December 23, 2020), as of October 6, 2026." | date stated: 2026-10-06
- C1-2025-19864 | fetched UTC 2026-11-13T01:18:02.817030+00:00 | Date: Fri, 13 Nov 2026 01:18:13 GMT | text: https://www.federalregister.gov/documents/full_text/text/2026/02/25/C1-2025-19864.txt
  DATES sentence: "Correction notice: no DATES paragraph and no comment deadline stated; it corrects proposed rule document 2025-19864 (Equal Credit Opportunity Act, Regulation B)." | date stated: None

### PULL 2 — verification fetches (browser, 2026-11-14 01:59-02:02 UTC)

Same agency queries as PULL 1 but fields[]=document_number,comments_close_on only (doc set + deadline check). Counts: CFPB 23, FDIC 28, OCC 25, Federal Reserve 20, NCUA 45, FinCEN 14 — sets identical to PULL 1; comments_close_on identical for all 138 documents.
RULE query (all six agencies, publication_date >= 2026-10-01), fields[]=document_number,publication_date,regulation_id_numbers: 8 rules — 2026-23060 (2026-11-12, 7100-AH33), 2026-22962 (2026-11-10, no RIN), 2026-22538 (2026-11-04, 3133-AG16), 2026-22537 (2026-11-04, 3133-AG12), 2026-22536 (2026-11-04, 3133-AF86), 2026-21706 (2026-10-23, 1557-AF41), 2026-20247 (2026-10-02, 7100-AH05), 2026-20246 (2026-10-02, 7100-AG92). The last four were already in the PULL 1 proof. RINs 7100-AH33, 3133-AG16 and 3133-AG12 belong to no proposal in the set. No new final rule attached to any proposal in PULL 2.

### PULL 3 — verification fetches (browser, 2026-11-15 01:40-01:45 UTC)

Same agency queries as PULL 2 (fields[]=document_number,comments_close_on). Crawl times: CFPB 01:40 UTC (count 23), FDIC 01:41 UTC (28), OCC 01:42 UTC (25), Federal Reserve 01:42 UTC (20), NCUA 01:43 UTC (45), FinCEN 01:43 UTC (14). Sets identical to PULL 1; comments_close_on identical for all 138 documents.
RULE query 1 (all six agencies, publication_date >= 2026-10-01, crawl 01:44 UTC), fields[]=document_number,publication_date,regulation_id_numbers: 12 rules — 2026-23288 (2026-11-16, 3133-AF75), 2026-23286 (2026-11-16, 3133-AG13), 2026-23281 (2026-11-16, 3133-AF85), 2026-23280 (2026-11-16, 3133-AG14), 2026-23060 (2026-11-12, 7100-AH33), 2026-22962 (2026-11-10, no RIN), 2026-22538 (2026-11-04, 3133-AG16), 2026-22537 (2026-11-04, 3133-AG12), 2026-22536 (2026-11-04, 3133-AF86), 2026-21706 (2026-10-23, 1557-AF41), 2026-20247 (2026-10-02, 7100-AH05), 2026-20246 (2026-10-02, 7100-AG92). Of these, 3133-AF75 and 3133-AF85 are RINs of proposals in the set, but their final rules (2026-23288 and 2026-23281) were published 2026-11-16, after the PULL 3 date, and have no per-RIN response in the PROOF, so they are NOT counted in the PULL 3 final rules column (REVISION 1; see Changes); 3133-AG13, 3133-AG14, 7100-AH33, 3133-AG16, 3133-AG12 belong to no proposal in the set; the rest were already in the PULL 1 proof.
RULE query 2 (all six agencies, publication 2025-01-01 to 2026-09-30, crawl 01:45 UTC), same fields: 105 rules. Every RIN was checked against the 176 proposal RINs and the PULL 1 proof: no rule in this set attaches to any proposal that the PULL 1 proof did not already list. Full list:

- 2026-20037 | 2026-09-30 | 7100-AH32
- 2026-20036 | 2026-09-30 | 7100-AH31
- 2026-19312 | 2026-09-22 | 1557-AF35; 3064-AG16
- 2026-18766 | 2026-09-14 | 1557-AF59; 3064-AG33; 7100-AH28
- 2026-18194 | 2026-09-04 | (no RIN)
- 2026-17865 | 2026-09-01 | 3064-AG32
- 2026-17823 | 2026-09-01 | 1557-AF35; 3064-AG16
- 2026-16576 | 2026-08-14 | 1506-AB67
- 2026-16365 | 2026-08-11 | (no RIN)
- 2026-16035 | 2026-08-06 | 3133-AF72
- 2026-16031 | 2026-08-06 | 3133-AF81
- 2026-16030 | 2026-08-06 | 3133-AF95
- 2026-16029 | 2026-08-06 | 3133-AF88
- 2026-16028 | 2026-08-06 | 3133-AF78
- 2026-16027 | 2026-08-06 | 3133-AF80
- 2026-16026 | 2026-08-06 | 3133-AF97
- 2026-16024 | 2026-08-06 | 3133-AF82
- 2026-16023 | 2026-08-06 | 3133-AG00
- 2026-16022 | 2026-08-06 | 3133-AF84
- 2026-16021 | 2026-08-06 | 3133-AF83
- C1-2026-10036 | 2026-06-29 | 1557-AF46
- 2026-12856 | 2026-06-25 | 3133-AF67
- 2026-12787 | 2026-06-25 | 1505-AC86; 1557-AF22; 2590-AB38; 3038-AF43; 3064-AF96; 3133-AF70; 3170-AB20; 3235-AN32; 7100-AG79
- 2026-12149 | 2026-06-17 | (no RIN)
- 2026-12058 | 2026-06-16 | 3133-AF61
- 2026-11559 | 2026-06-09 | 3133-AG11
- 2026-11507 | 2026-06-09 | 3133-AF64
- 2026-11044 | 2026-06-03 | 3064-AF76
- 2026-10037 | 2026-05-19 | 1557-AF45
- 2026-08494 | 2026-05-01 | 3170-AB40
- 2026-08328 | 2026-04-29 | 1557-AF54
- 2026-08298 | 2026-04-29 | 1557-AF33; 3064-AG17; 7100-AH08
- 2026-07804 | 2026-04-22 | 3170-AB54
- 2026-07416 | 2026-04-16 | (no RIN)
- 2026-06947 | 2026-04-10 | 1557-AF34; 3064-AG12
- 2026-06281 | 2026-04-01 | 1557-AF40
- 2026-05652 | 2026-03-23 | 3064-AG06
- 2026-05544 | 2026-03-20 | 7100-AH19
- 2026-04641 | 2026-03-10 | (no RIN)
- 2026-04373 | 2026-03-05 | 7100-AG37
- 2026-04276 | 2026-03-04 | 1557-AF42
- 2026-04275 | 2026-03-04 | 1557-AF38
- 2026-04088 | 2026-03-02 | 1557-AF47
- 2026-01806 | 2026-01-29 | 3064-AG14
- 2026-00449 | 2026-01-13 | (no RIN)
- 2026-00332 | 2026-01-12 | 3133-AG06
- 2026-00087 | 2026-01-07 | (no RIN)
- 2026-00085 | 2026-01-07 | (no RIN)
- 2025-24184 | 2026-01-02 | 1506-AB58; 1506-AB69
- 2025-23837 | 2025-12-29 | 3064-AG10
- 2025-23548 | 2025-12-22 | 7100-AH14
- 2025-23425 | 2025-12-19 | 3064-AG24
- 2025-23390 | 2025-12-19 | (no RIN)
- 2025-23389 | 2025-12-19 | (no RIN)
- 2025-22875 | 2025-12-16 | 1557-AF39; 7100-AH12
- 2025-22814 | 2025-12-15 | 7100-AH10
- 2025-22813 | 2025-12-15 | 7100-AH11
- 2025-22773 | 2025-12-15 | (no RIN)
- 2025-22772 | 2025-12-15 | (no RIN)
- 2025-21914 | 2025-12-04 | 3064-AG15
- 2025-21626 | 2025-12-01 | 1557-AF31; 3064-AG11; 7100-AG96
- 2025-21461 | 2025-11-28 | 3064-AF26
- 2025-20744 | 2025-11-24 | (no RIN)
- 2025-20472 | 2025-11-20 | 7100-AH09
- 2025-19889 | 2025-11-14 | 7100-AH07
- 2025-19888 | 2025-11-14 | 7100-AH06
- 2025-19689 | 2025-10-29 | 3170-AB32
- 2025-19687 | 2025-10-29 | 3170-AB33
- 2025-19671 | 2025-10-28 | (no RIN)
- 2025-19571 | 2025-10-16 | 1506-AB68
- 2025-19370 | 2025-10-02 | 3170-AB40
- 2025-19304 | 2025-10-02 | 7100-AG97
- 2025-19303 | 2025-10-02 | 7100-AG98
- 2025-18622 | 2025-09-25 | 3170-AB34
- 2025-17371 | 2025-09-10 | (no RIN)
- 2025-16080 | 2025-08-22 | (no RIN)
- 2025-13665 | 2025-07-21 | 3170-AB43
- 2025-12973 | 2025-07-11 | (no RIN)
- 2025-12493 | 2025-07-03 | 3064-ZA45
- 2025-11993 | 2025-06-30 | (no RIN)
- 2025-11991 | 2025-06-30 | (no RIN)
- 2025-11990 | 2025-06-30 | (no RIN)
- 2025-11244 | 2025-06-18 | 3170-AB40
- 2025-11241 | 2025-06-18 | (no RIN)
- 2025-08640 | 2025-05-21 | 3170-AB43
- 2025-08643 | 2025-05-16 | 3170-AB42
- 2025-08641 | 2025-05-15 | (no RIN)
- 2025-08405 | 2025-05-15 | 1557-AF29
- 2025-08286 | 2025-05-12 | (no RIN)
- 2025-06966 | 2025-04-23 | (no RIN)
- 2025-06748 | 2025-04-18 | 3064-ZA46
- 2025-05199 | 2025-03-26 | 1506-AB49
- 2025-04099 | 2025-03-14 | (no RIN)
- 2025-03790 | 2025-03-11 | 3064-AF26
- C1-2024-30824 | 2025-01-27 | 3170-AA54
- 2025-01374 | 2025-01-17 | (no RIN)
- 2025-00737 | 2025-01-15 | 3133-AF65
- 2025-00430 | 2025-01-15 | (no RIN)
- 2025-00429 | 2025-01-15 | (no RIN)
- 2025-00381 | 2025-01-15 | (no RIN)
- 2024-30824 | 2025-01-14 | 3170-AA54
- 2025-00419 | 2025-01-13 | 7100-AG91
- 2025-00374 | 2025-01-10 | (no RIN)
- 2024-30628 | 2025-01-10 | 3170-AA84
- 2025-00167 | 2025-01-08 | (no RIN)

### Per proposal — returned values verbatim (PULL 1 API responses)

One line per proposal: document_number | comments_close_on as returned (null = absent) | regulation_id_numbers as returned | docket_ids as returned.

- 2024-31385 | comments_close_on: null | rins: 3170-AB16 | docket ids: Docket No. CFPB-2024-0003
- 2025-00633 | comments_close_on: 2025-04-01 | rins: 3170-AB23 | docket ids: Docket No. CFPB-2025-0002
- 2025-00565 | comments_close_on: 2025-03-31 | rins: (none) | docket ids: CFPB-2025-0003
- 2025-03547 | comments_close_on: 2025-04-02 | rins: 3170-AB27 | docket ids: Docket No. CFPB-2024-0044
- 2025-03685 | comments_close_on: 2025-04-07 | rins: (none) | docket ids: Docket No. CFPB-2024-0057
- 2025-03832 | comments_close_on: 2025-04-10 | rins: 3064-ZA45 | docket ids: (none)
- 2025-04088 | comments_close_on: null | rins: 3064-AF94; 3064-AF99; 3064-AG04 | docket ids: (none)
- 2025-06863 | comments_close_on: 2025-06-23 | rins: 7100-AG92 | docket ids: Regulations Y, LL, and YY; Docket No. R-1866
- 2025-07837 | comments_close_on: 2025-06-04 | rins: 1506-AB68 | docket ids: (none)
- 2025-08344 | comments_close_on: 2025-06-12 | rins: 3170-AB33 | docket ids: Docket No. CFPB-2025-0012
- 2025-08345 | comments_close_on: 2025-06-13 | rins: 3170-AB32 | docket ids: Docket No. CFPB-2025-0011
- 2025-08347 | comments_close_on: 2025-06-13 | rins: 3170-AB34 | docket ids: Docket No. CFPB-2025-0013
- 2025-08644 | comments_close_on: null | rins: 3170-AB27 | docket ids: Docket No. CFPB-2024-0044
- 2025-08645 | comments_close_on: null | rins: 3170-AB23 | docket ids: Docket No. CFPB-2025-0002
- 2025-08646 | comments_close_on: null | rins: (none) | docket ids: Docket No. CFPB-2025-0003
- 2025-11248 | comments_close_on: 2025-07-18 | rins: (none) | docket ids: Docket No. CFPB-2025-0021
- 2025-12787 | comments_close_on: 2025-08-26 | rins: 1557-AF31; 3064-AG11; 7100-AG96 | docket ids: Docket ID OCC-2025-0006; Regulations H, Q, and YY; Docket No. R-1867
- 2025-12807 | comments_close_on: 2025-10-08 | rins: (none) | docket ids: NCUA-2024-0014
- 2025-13504 | comments_close_on: null | rins: 3064-AF88 | docket ids: (none)
- 2025-13559 | comments_close_on: 2025-08-18 | rins: 1557-AF30; 3064-AG13; 7100-AG95 | docket ids: Docket ID OCC-2025-0005; Docket No. R-1869
- 2025-13568 | comments_close_on: 2025-09-16 | rins: 3064-AG10 | docket ids: (none)
- 2025-14060 | comments_close_on: 2025-10-23 | rins: 3064-ZA39 | docket ids: Docket ID OCC-2023-0016; Docket No. OP-1828
- 2025-14132 | comments_close_on: 2025-09-26 | rins: 3064-AG15 | docket ids: (none)
- 2025-15088 | comments_close_on: 2025-09-22 | rins: 3170-AB52 | docket ids: Docket No. CFPB-2025-0031
- 2025-15089 | comments_close_on: 2025-09-22 | rins: 3170-AB50 | docket ids: Docket No. CFPB-2025-0029
- 2025-15090 | comments_close_on: 2025-09-22 | rins: 3170-AB53 | docket ids: Docket No. CFPB-2025-0025
- 2025-15091 | comments_close_on: 2025-09-22 | rins: 3170-AB51 | docket ids: Docket No. CFPB-2025-0030
- 2025-16056 | comments_close_on: 2025-10-20 | rins: 3064-AG14 | docket ids: (none)
- 2025-16139 | comments_close_on: 2025-10-21 | rins: 3170-AB39 | docket ids: Docket No. CFPB-2025-0037
- 2025-16352 | comments_close_on: 2025-09-25 | rins: 3170-AB45 | docket ids: Docket No. CFPB-2025-0018
- 2025-18271 | comments_close_on: 2025-10-22 | rins: 1506-AB58; 1506-AB69 | docket ids: (none)
- 2025-19623 | comments_close_on: 2025-12-22 | rins: 3133-AF67 | docket ids: (none)
- 2025-19690 | comments_close_on: null | rins: (none) | docket ids: Docket No. CFPB-2023-0002
- 2025-19711 | comments_close_on: 2025-12-29 | rins: 1557-AF35; 3064-AG16 | docket ids: Docket ID OCC-2025-0174
- 2025-19715 | comments_close_on: 2025-12-29 | rins: 1557-AF34; 3064-AG12 | docket ids: Docket ID OCC-2025-0142
- 2025-19864 | comments_close_on: 2025-12-15 | rins: 3170-AB54 | docket ids: Docket No. CFPB-2025-0039
- 2025-19865 | comments_close_on: 2025-12-15 | rins: 3170-AB40 | docket ids: Docket No. CFPB-2025-0040
- 2025-19927 | comments_close_on: 2025-12-17 | rins: 1506-AB70 | docket ids: (none)
- 2025-20199 | comments_close_on: 2025-12-18 | rins: 1557-AF40 | docket ids: Docket ID OCC-2025-0339
- 2025-20202 | comments_close_on: 2025-12-18 | rins: 1557-AF42 | docket ids: Docket ID OCC-2025-0405
- 2025-20204 | comments_close_on: 2026-01-20 | rins: 1557-AF38 | docket ids: Docket ID OCC-2025-0273
- 2025-20211 | comments_close_on: 2026-01-22 | rins: 7100-AH05 | docket ids: Regulations Y, LL, and YY; Docket No. R-1873
- 2025-21087 | comments_close_on: 2026-02-21 | rins: 7100-AH05 | docket ids: Regulations Y, LL, and YY; Docket No R-1873
- 2025-21625 | comments_close_on: 2026-01-30 | rins: 1557-AF33; 3064-AG17; 7100-AH08 | docket ids: Docket ID OCC-2025-0141; Docket No. R-1876
- 2025-22487 | comments_close_on: 2026-02-09 | rins: 3133-AF73 | docket ids: (none)
- 2025-22488 | comments_close_on: 2026-02-09 | rins: 3133-AF74 | docket ids: (none)
- 2025-22489 | comments_close_on: 2026-02-09 | rins: 3133-AF76 | docket ids: (none)
- 2025-22490 | comments_close_on: 2026-02-09 | rins: 3133-AF79 | docket ids: (none)
- 2025-23510 | comments_close_on: 2026-02-17 | rins: 3064-AG20 | docket ids: (none)
- 2025-23547 | comments_close_on: 2026-02-20 | rins: (none) | docket ids: Docket ID OCC-2025-0669
- 2025-23854 | comments_close_on: 2026-02-27 | rins: 3133-AF75 | docket ids: (none)
- 2025-23855 | comments_close_on: 2026-02-27 | rins: 3133-AF72 | docket ids: (none)
- 2025-23856 | comments_close_on: 2026-02-27 | rins: 3133-AF77 | docket ids: (none)
- 2025-23857 | comments_close_on: 2026-02-27 | rins: 3133-AF80 | docket ids: (none)
- 2025-23986 | comments_close_on: 2026-03-02 | rins: 1557-AF36 | docket ids: Docket ID OCC-2025-0207
- 2025-23987 | comments_close_on: 2026-01-29 | rins: 1557-AF45 | docket ids: Docket ID OCC-2025-0735
- 2025-23988 | comments_close_on: 2026-01-29 | rins: 1557-AF46 | docket ids: Docket ID OCC-2025-0736
- 2026-00372 | comments_close_on: 2026-02-11 | rins: 1557-AF47 | docket ids: Docket ID OCC-2025-0768
- 2026-00591 | comments_close_on: 2026-03-16 | rins: 3133-AF85 | docket ids: (none)
- 2026-00592 | comments_close_on: 2026-03-16 | rins: 3133-AF81 | docket ids: (none)
- 2026-00594 | comments_close_on: 2026-03-16 | rins: 3133-AF82 | docket ids: (none)
- 2026-00595 | comments_close_on: 2026-03-16 | rins: 3133-AF84 | docket ids: (none)
- 2026-00603 | comments_close_on: 2026-02-11 | rins: 1557-AF47 | docket ids: Docket ID OCC-2025-0768
- 2026-01382 | comments_close_on: 2026-03-27 | rins: 3133-AF64 | docket ids: (none)
- 2026-01696 | comments_close_on: 2026-03-30 | rins: 3133-AF92 | docket ids: (none)
- 2026-01697 | comments_close_on: 2026-03-30 | rins: 3133-AF94 | docket ids: (none)
- 2026-01698 | comments_close_on: 2026-03-30 | rins: 3133-AF97 | docket ids: (none)
- 2026-01699 | comments_close_on: 2026-03-30 | rins: 3133-AG00 | docket ids: (none)
- 2026-02665 | comments_close_on: 2026-05-18 | rins: 3064-AG20 | docket ids: (none)
- 2026-02763 | comments_close_on: 2026-04-13 | rins: 3133-AG01 | docket ids: (none)
- 2026-02764 | comments_close_on: 2026-04-13 | rins: 3133-AG03 | docket ids: (none)
- 2026-02765 | comments_close_on: 2026-04-13 | rins: 3133-AF78 | docket ids: (none)
- 2026-02868 | comments_close_on: 2026-04-13 | rins: 3133-AF69 | docket ids: (none)
- 2026-03086 | comments_close_on: 2026-04-20 | rins: 1557-AF48 | docket ids: Docket ID OCC-2026-0001
- 2026-03753 | comments_close_on: 2026-04-27 | rins: 3133-AF96 | docket ids: (none)
- 2026-03754 | comments_close_on: 2026-04-27 | rins: 3133-AF98 | docket ids: (none)
- 2026-03755 | comments_close_on: 2026-04-27 | rins: 3133-AF95 | docket ids: (none)
- 2026-03756 | comments_close_on: 2026-04-27 | rins: 3133-AF99 | docket ids: (none)
- 2026-03757 | comments_close_on: 2026-04-27 | rins: 3133-AF83 | docket ids: (none)
- 2026-03758 | comments_close_on: 2026-04-27 | rins: 3133-AF86 | docket ids: (none)
- C1-2025-19864 | comments_close_on: null | rins: 3170-AB54 | docket ids: Docket No. CFPB-2025-0039
- 2026-03818 | comments_close_on: 2026-04-27 | rins: 7100-AH17 | docket ids: Docket No. R-1884
- 2026-04033 | comments_close_on: 2026-04-01 | rins: 1506-AB71 | docket ids: (none)
- 2026-04089 | comments_close_on: 2026-05-01 | rins: 1557-AF41 | docket ids: Docket ID OCC-2025-0372
- 2026-04154 | comments_close_on: 2026-06-01 | rins: (none) | docket ids: NCUA-2024-0014
- 2026-04761 | comments_close_on: 2026-05-11 | rins: 3133-AF61 | docket ids: (none)
- 2026-05797 | comments_close_on: 2026-05-26 | rins: 3133-AF88 | docket ids: (none)
- 2026-05959 | comments_close_on: 2026-06-18 | rins: 1557-AF52; 3064-AF29; 7100-AH20 | docket ids: Docket ID OCC-2026-0265; Docket No. 1887
- 2026-05960 | comments_close_on: 2026-06-18 | rins: 1557-AF49; 3064-AG23; 7100-AH21 | docket ids: Docket ID OCC-2026-0034; Docket No. R-1888
- 2026-05961 | comments_close_on: 2026-06-18 | rins: 7100-AH22 | docket ids: Docket No. 1889
- 2026-06271 | comments_close_on: 2026-06-01 | rins: 1506-AB57 | docket ids: (none)
- 2026-06757 | comments_close_on: 2026-06-08 | rins: 3133-AF93 | docket ids: (none)
- 2026-06948 | comments_close_on: 2026-06-09 | rins: 1557-AF14; 3064-AF34; 3133-AG08 | docket ids: Docket ID OCC-2024-0005; Docket ID NCUA-2024-0033
- 2026-06963 | comments_close_on: 2026-06-09 | rins: 1506-AB73 | docket ids: Docket No. FINCEN-2026-0100
- 2026-06974 | comments_close_on: 2026-06-09 | rins: 3064-AG19 | docket ids: (none)
- 2026-06996 | comments_close_on: 2026-06-09 | rins: 7100-AH23 | docket ids: Docket No. R-1891
- 2026-07033 | comments_close_on: 2026-06-09 | rins: 1506-AB72 | docket ids: (none)
- 2026-07806 | comments_close_on: 2026-06-22 | rins: 3133-AG02 | docket ids: (none)
- 2026-08143 | comments_close_on: 2026-05-27 | rins: 1557-AF32 | docket ids: Docket ID OCC-2025-0075
- 2026-09009 | comments_close_on: 2026-07-06 | rins: 3133-AF89 | docket ids: (none)
- 2026-09010 | comments_close_on: 2026-07-06 | rins: 3133-AF87 | docket ids: (none)
- 2026-09915 | comments_close_on: 2026-07-17 | rins: 3133-AG10 | docket ids: (none)
- 2026-10376 | comments_close_on: 2026-07-27 | rins: 7100-AH24 | docket ids: Docket No. R-1892
- 2026-10377 | comments_close_on: 2026-07-27 | rins: 7100-AH25 | docket ids: Docket No. R-1893
- 2026-10817 | comments_close_on: 2026-07-13 | rins: 0412-AB19; 0414-AA00; 0415-AA00; 0420-AA37; 0505-AA20; 0605-AA85; 0790-AM03; 0960-AJ11; 0991-AC35; 1090-AB34; 1105-AB81; 1291-AA53; 1400-AG22; 1505-AC92; 1601-AB23; 1801-AA30; 1991-AC21; 2030-AB05; 2105-AF44; 2501-AE01; 2700-AE90; 2900-AT02; 3015-AA00; 3041-AE26; 3045-AA94; 3048-AA03; 3060-AM35; 3095-AC31; 3112-AA07; 3133-AG07; 3135-AA36; 3136-AA47; 3137-AA31; 3139-AA07; 3145-AA75; 3150-AL41; 3201-AA03; 3245-AI70; 3265-AA00; 3600-AA05; 4718-AA00 | docket ids: (none)
- 2026-11342 | comments_close_on: 2026-08-04 | rins: 3064-AG29 | docket ids: (none)
- 2026-12460 | comments_close_on: 2026-08-21 | rins: 1506-AB74 | docket ids: (none)
- 2026-12692 | comments_close_on: 2026-07-24 | rins: 1557-AF55 | docket ids: Docket ID OCC-2026-0463
- 2026-12794 | comments_close_on: 2026-07-27 | rins: 1506-AB75 | docket ids: (none)
- 2026-13123 | comments_close_on: 2026-08-31 | rins: 3064-AG30 | docket ids: (none)
- 2026-13191 | comments_close_on: 2026-08-31 | rins: 3064-AG21 | docket ids: (none)
- 2026-13192 | comments_close_on: 2026-08-31 | rins: 3064-AG27 | docket ids: (none)
- 2026-13834 | comments_close_on: 2026-08-10 | rins: (none) | docket ids: Docket No. CFPB-2026-0018
- 2026-13919 | comments_close_on: 2026-09-08 | rins: 7100-AG78 | docket ids: Docket No. R-1835
- 2026-15030 | comments_close_on: 2026-08-02 | rins: 1506-AB75 | docket ids: (none)
- 2026-15774 | comments_close_on: 2026-10-05 | rins: 7100-AH26 | docket ids: Regulations Q and MM; Docket No. R-1895
- 2026-15777 | comments_close_on: 2026-10-05 | rins: 7100-AH27 | docket ids: Regulations O and Y; Docket No. R-1896
- 2026-15867 | comments_close_on: 2026-10-05 | rins: 1557-AF50 | docket ids: Docket ID OCC-2026-0133
- 2026-15995 | comments_close_on: 2026-10-05 | rins: 3064-AG26 | docket ids: (none)
- 2026-16454 | comments_close_on: 2026-10-13 | rins: 1557-AF57; 3064-AG31 | docket ids: Docket ID OCC-2026-0694
- 2026-17649 | comments_close_on: 2026-10-05 | rins: 3064-AG30 | docket ids: (none)
- 2026-17822 | comments_close_on: 2026-10-01 | rins: 1557-AF56 | docket ids: Docket ID OCC-2026-0529
- 2026-17871 | comments_close_on: 2026-10-01 | rins: 1506-AB76 | docket ids: (none)
- 2026-19308 | comments_close_on: 2026-11-23 | rins: 3064-AG18 | docket ids: (none)
- 2026-19310 | comments_close_on: 2026-11-23 | rins: 3064-AG34 | docket ids: (none)
- 2026-19860 | comments_close_on: 2026-11-30 | rins: 7100-AH29 | docket ids: Docket No. R-1899
- 2026-19899 | comments_close_on: 2026-11-30 | rins: 7100-AH30 | docket ids: Docket No. R-1900
- 2026-20371 | comments_close_on: 2026-11-04 | rins: 1506-AB77 | docket ids: (none)
- 2026-20429 | comments_close_on: null | rins: 1506-AB47 | docket ids: (none)
- 2026-20430 | comments_close_on: null | rins: 1506-AB47 | docket ids: (none)
- 2026-20509 | comments_close_on: 2026-11-04 | rins: 7100-AH27 | docket ids: Regulation O; Docket No. R-1896
- 2026-20735 | comments_close_on: 2026-11-04 | rins: 3064-AG26 | docket ids: (none)
- 2026-21087 | comments_close_on: 2026-12-14 | rins: 3133-AG04 | docket ids: (none)
- 2026-21088 | comments_close_on: 2026-12-14 | rins: 3133-AF90 | docket ids: (none)
- 2026-21089 | comments_close_on: 2026-12-14 | rins: 3133-AF91 | docket ids: (none)
- 2026-21508 | comments_close_on: 2026-12-21 | rins: 3133-AG26 | docket ids: (none)
- 2026-21509 | comments_close_on: 2026-12-21 | rins: 3133-AG21 | docket ids: (none)
- 2026-21512 | comments_close_on: 2026-12-21 | rins: 3133-AG24 | docket ids: (none)

### Dates sentences used (the 10 proposals with no API comments_close_on)

- 2024-31385: "The proposed rule published January 31, 2024, at 89 FR 6031 is  withdrawn as of January 14, 2025." (date stated: 2025-01-14) -> comments_close_on cell: 2025-01-14
- 2025-04088: "The FDIC is withdrawing the proposed rules published at 89 FR  68244 (August 23, 2024), 88 FR 70391 (October 11, 2023), and 89 FR  67002 (August 19, 2024) as of March 14, 2025." (date stated: 2025-03-14) -> comments_close_on cell: 2025-03-14
- 2025-08644: "The proposed rule is withdrawn as of May 15, 2025." (date stated: 2025-05-15) -> comments_close_on cell: 2025-05-15
- 2025-08645: "The notice of proposed rulemaking is withdrawn as of May 15,  2025." (date stated: 2025-05-15) -> comments_close_on cell: 2025-05-15
- 2025-08646: "The proposed interpretive rule is withdrawn as of May 15, 2025." (date stated: 2025-05-15) -> comments_close_on cell: 2025-05-15
- 2025-13504: "The FDIC is withdrawing the proposed rule published at 89 FR  65556 (August 12, 2024) as of July 18, 2025." (date stated: 2025-07-18) -> comments_close_on cell: 2025-07-18
- 2025-19690: "The Proposed Rule published February 1, 2023, 88 FR 6906, is  withdrawn as of October 29, 2025." (date stated: 2025-10-29) -> comments_close_on cell: 2025-10-29
- 2026-20429: "FinCEN is withdrawing the proposed rulemaking published at 88 FR  72701 (October 23, 2023), as of October 6, 2026." (date stated: 2026-10-06) -> comments_close_on cell: 2026-10-06
- 2026-20430: "FinCEN is withdrawing the proposed rule published at 85 FR 83840  (December 23, 2020), as of October 6, 2026." (date stated: 2026-10-06) -> comments_close_on cell: 2026-10-06
- C1-2025-19864: "Correction notice: no DATES paragraph and no comment deadline stated; it corrects proposed rule document 2025-19864 (Equal Credit Opportunity Act, Regulation B)." (date stated: None) -> comments_close_on cell: none
