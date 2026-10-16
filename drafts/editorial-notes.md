# Community reframing — September 8, 2026

The manuscript now leads with engineers inspecting and contributing to software
trust evidence. This is a working paper draft, not a submission-ready artifact.

## Evidence boundary

- Current behaviour was checked against TrustSECO-Next/docs/live-community-pilot.md,
  docs/community-prototype.md, services/ledger/src/app/modules/community/policy.ts,
  services/ledger/src/app/modules/pilot/policy.ts and tools/pilot/client.cjs.
- The numerical Flask example is the documented September 8 four-metric run:
  12 observations, four corroborated rounds, score 52.55, coverage 4/21. It is a
  historical functional run, not a claim about the latest collector coverage.
- Local tests use locally controlled identities and validators. Do not describe
  these as independent operators or claim production-level resilience.
- Random observer assignment is being developed in a separate task/worktree.
  Its eventual guarantees, tests and integration status must replace the baseline
  paragraph after review. Do not describe it as already deployed.
- The old 20-practitioner evaluation and 400-package claim are excluded pending
  source/provenance checks. The old text is preserved in the preceding draft.
- npmSECO remains prior work only. Its publication year was corrected to 2025 and
  its DOI added. Compare the full prior papers before finalizing novelty claims.

## Remaining authoring work

1. Select a reproducible release/commit and verify every demo step against it.
2. Capture current portal/community screenshots and add a clear workflow figure.
3. Integrate the tested observer-assignment design when ready.
4. Replace development-status language with release-specific facts.
5. Provide the accessible reviewer artifact, usage instructions and 3–5 minute
   video; put the video URL at the end of the abstract as required by the call.
6. Restore the agreed authors for single-anonymous submission.
7. Verify bibliography metadata and broaden the comparison with relevant tools;
   no unverified superiority claims have been retained.
8. Rebuild and inspect the final PDF within four pages including references.

Compilation and PDF text checks passed; three pages, no unresolved citations,
no author metadata, no overfull boxes. The rendered pages were inspected.

## Added ICSE context

- Beller and Hejderup, ICSE-NIER 2019, DOI 10.1109/ICSE-NIER.2019.00022.
  Publisher abstract and accepted manuscript at https://pure.tudelft.nl/ws/files/57741633/paper.pdf.
  Direct conceptual predecessor for blockchain-based SE infrastructure.
- Boughton et al., ICSE-NIER 2024, DOI 10.1145/3639476.3639775.
  Author record: https://dwermke.com/publications/2024-conf-icse-boughton/.
  Relationship/behaviour-based measurement of trust; corroboration alone does not
  validate a metric as an indicator of trust.
- Benedetti et al., ICSE 2025, DOI 10.1109/ICSE55347.2025.00136.
  Author manuscript: https://www.cs.cmu.edu/~ckaestne/pdf/icse25_rb.pdf.
  Independent verification of packaging is complementary, not a current feature.

Venue labels distinguish ICSE-NIER from the ICSE main proceedings. The ACM 2024
landing page has an inconsistent conference ordinal; the bibliography omits the
ordinal for that entry rather than copying it.

After adding the ICSE comparison: four pages including references; rebuilt and
visually checked, with no unresolved citations or overfull boxes.

## Company funding and provisional screenshot

The company-funded demand model comes from the author's stated vision. The paper
does not claim an implemented purchase, fiat conversion, or company onboarding flow.

`images/flask-detail-current.png` is a genuine browser capture from the local
port-3005 Flask 3.1.2 detail page on September 8, 2026. It shows the upper viewport,
including scores 62.7, coverage 10/21, and 36 confirmed observations. This is later
than the four-metric historical validation run and is not substituted for it.
The screenshot is provisional and should be refreshed for the submitted release.

## Restored scoring equations

Checked against services/ledger/src/app/modules/trustfacts/endpoint.ts and
apps/coordinator/src/pilot-portal.ts. Log metrics use log(reference value) in
the denominator. The displayed overall logistic uses growth 0.02 and midpoint 50.
The formula is stated for nonnegative observations, as accepted by the pilot.
The generic implementation averages multiple observations per metric; the pilot
selects one input per metric for each score. Coverage is an accompanying count
out of 21, not a score normalization factor. Weights include heuristic choices.
The screenshot was reduced from 92% to 72% of text width to retain page space.
