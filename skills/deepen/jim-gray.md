# Jim Gray review (phase 2 of /deepen)

Read and follow this after the Deepen assessment and rewrite in SKILL.md. The problem is the same one being deepened.

Review Jim Gray's relevant published works and consider how he might approach the user's problem. Produce an evidence-based analysis, not an impersonation or a claim to know his private views.

## Establish the problem

Use the same problem identified in phase 1. Preserve the user's scope and resource limits. Examine the original problem and its deeper formulation; do not merely critique the wording of the rewritten prompt.

## Review relevant publications

**Use the local library first.** Full texts of core Jim Gray papers are cached in [jim-gray-library/](jim-gray-library/). Read `jim-gray-library/CATALOG.md`, pick candidates by the Topics column, then read or grep `jim-gray-library/text/<file>.txt` directly. Cite the catalog's Source URL as the link. Do not re-download a paper that is already cached.

Go to the web only when the problem needs a work that is not cached. Then discover it from https://jimgray.azurewebsites.net/NoFrameDefault.htm (or the Microsoft Research catalog), download it once into `jim-gray-library/raw/`, extract text into `jim-gray-library/text/` (`pdftotext -layout` for PDF, `catdoc -w` for DOC), and add a row to `CATALOG.md` with title, authors, year, venue, source URL, and topics. Mark venue details as unverified unless the document itself states them. That way the next run finds it locally.

These sources are starting points, not proof of a paper's claims.

Choose a small set of directly relevant publications, usually two to four, rather than claiming to review his entire corpus. One well-matched work can suffice; do not pad the list with weakly related papers. Read the relevant full-text sections when accessible. Search snippets, abstracts, and secondary summaries alone do not support a claim of full-paper review. State exactly what was accessible and reviewed. Follow citations to original works if useful.

For every substantive attribution, provide a direct source link with title and year, and a section or page where available. Identify coauthored work as such. Distinguish publication dates from web upload dates. Never invent quotations, citations, results, or bibliographic details. If browsing or full text is unavailable, request the needed documents or offer a clearly provisional analysis from supplied evidence; do not present remembered themes as a completed literature review.

Let the problem and papers determine the useful principles. Do not force every task into databases, transactions, replication, or distributed systems. If the connection is weak, explain the limit and use only defensible analogies. Treat historical hardware assumptions, prices, and workload measurements as historical; verify current equivalents before using them for a present-day decision.

## Apply the evidence

Give a concise analysis with:

- **Relevant works and findings:** What was actually reviewed and which documented ideas bear on this problem.
- **Application to this problem:** Connect each useful idea to the user's actual constraints or artifacts. Clearly label this as your interpretation of the published work, not a statement Jim Gray made about this particular problem.
- **Recommended approach:** Propose concrete steps, meaningful alternatives, tradeoffs, likely failure modes, and any missing evidence that could change the recommendation. Keep the solution proportional to the original task.
- **Validation:** Identify an observable test, measurement, experiment, or independent check that could support or disprove the approach. Distinguish proposed validation from completed validation.

Do the source review and reasoning during this phase, but do not implement the proposed solution yet. Then return to SKILL.md for the synthesis.
