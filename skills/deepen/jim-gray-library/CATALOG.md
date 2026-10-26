# Jim Gray local library

Cached full texts so /deepen phase 2 does not re-download papers on every run.

- `text/<file>.txt` — full extracted text (pdftotext -layout / catdoc). Read and grep these.
- `raw/` — original PDF/DOC as downloaded, kept for page checks.
- Source URLs are where the copy was fetched; cite them as the link. Venue details marked
  "unverified" come from memory, not from the document itself — check before relying on them.

## Index

| File (text/) | Title | Authors | Year | Venue / report | Source URL | Topics |
|---|---|---|---|---|---|---|
| 1981_transaction_concept.txt | The Transaction Concept: Virtues and Limitations | Jim Gray | 1981 | Tandem TR 81.3; Proc. 7th VLDB, Sept 1981 (per doc) | https://jimgray.azurewebsites.net/papers/thetransactionconcept.pdf | atomicity/durability/consistency, update-in-place vs. never-overwrite ("poison apple"), time-domain addressing, logging & locking, nested and long-lived transactions |
| 1985_why_do_computers_stop.txt | Why Do Computers Stop and What Can Be Done About It? | Jim Gray | 1985 | Tandem TR 85.7, June 1985 | https://pages.cs.wisc.edu/~remzi/Classes/739/Fall2018/Papers/gray85-easy.pdf (2025 retypeset of the 1985 TR; original hpl.hp.com mirror is down) | failure causes (administration 42%, software 25%…), fail-fast modules, Heisenbugs vs. Bohrbugs, process pairs, transactions, reliable storage |
| 1994_synthetic_data_gen.txt | Quickly Generating Billion-Record Synthetic Databases | Gray, Sundaresan, Englert, Baclawski, Weinberger | 1994 | SIGMOD 1994 (unverified) | https://jimgray.azurewebsites.net/papers/SyntheticDataGen.pdf | reproducible seeded generators, Zipfian/skewed distributions, parallel data generation |
| 1995_ansi_isolation_critique.txt | A Critique of ANSI SQL Isolation Levels | Berenson, Bernstein, Gray, Melton, O'Neil, O'Neil | 1995 | MSR-TR-95-51; SIGMOD 1995 (unverified) | https://jimgray.azurewebsites.net/Isolation.doc | isolation anomalies, snapshot isolation, precise spec of concurrency behavior |
| 1996_dangers_of_replication.txt | The Dangers of Replication and a Solution | Gray, Helland, O'Neil, Shasha | 1996 | SIGMOD 1996, San Francisco | https://jimgray.azurewebsites.net/replicas.doc | update-anywhere instability, master copy, two-tier replication for mobile/disconnected nodes, tentative transactions |
| 1996_db_history.txt | Data Management: Past, Present, and Future | Jim Gray | 1996 | Draft (MSR); later IEEE Computer, Oct 1996 (unverified) | https://jimgray.azurewebsites.net/DB_History.doc | history of data management, trends |
| 1997_five_minute_rule.txt | The Five-Minute Rule Ten Years Later, and Other Computer Storage Rules of Thumb | Gray, Graefe | 1997 | SIGMOD Record 26(4), 1997 | https://jimgray.azurewebsites.net/5_min_rule_SIGMOD.doc | memory vs. disk caching economics, storage rules of thumb (historical prices) |
| 1999_scalability_terminology.txt | Scalability Terminology: Farms, Clones, Partitions, and Packs: RACS and RAPS | Devlin, Gray, Laing, Spix | 1999 | MS-TR-99-85 | https://jimgray.azurewebsites.net/papers/MS_TR_99_85_Scalability_Terminology.pdf | scale-out vocabulary, clones, partitions, packs |
| 1999_turing_talk.txt | What Next? A Dozen Information-Technology Research Goals | Jim Gray | 1999 | MS-TR-99-50 (Turing Award lecture) | https://jimgray.azurewebsites.net/papers/MS_TR_99_50_TuringTalk.pdf | long-range research goals, Turing test, trouble-free systems, personal memex |
| 2000_rules_of_thumb.txt | Rules of Thumb in Data Engineering | Gray, Shenoy | 2000 | MS-TR-99-100 (rev. March 2000) | https://jimgray.azurewebsites.net/papers/MS_TR_99_100_Rules_of_Thumb_in_Data_Engineering.pdf | storage/network/CPU ratios and cost rules (historical) |

## Not cached yet (fetch on demand, then add a row)

Discovery index: https://jimgray.azurewebsites.net/NoFrameDefault.htm (the `papers.htm` page is a frameset).
Notable candidates: The Benchmark Handbook (1993, ed. Gray), "A Measure of Transaction Processing Power" (1985),
Transaction Processing: Concepts and Techniques (Gray & Reuter, 1992 — book, not freely available),
"The Cost of Messages" (1988), "Granularity of Locks" (1975), AlphaSort (1994), TerraServer (1998–99),
Sloan Digital Sky Survey (1999), "Queues Are Databases" (1995), Digital Immortality (2000).
