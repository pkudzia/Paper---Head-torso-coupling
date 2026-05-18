# Section-by-Section Manuscript Review

**Manuscript:** Video-based analysis of head-torso coupling during lateral impacts under passive and co-contracted conditions
**Version:** March 3, 2026
**Overall score: 124 / 160 (78%)**

---

## Score Summary

| Section | Score | Status |
|---------|:-----:|--------|
| Title Page | 17/20 | Good |
| Abstract | 18/20 | Strong |
| Introduction | 16/20 | Solid, needs tightening |
| Methods | 16/20 | Thorough, label needs fixing |
| Results | 18/20 | Strong |
| Discussion | 15/20 | Needs trimming |
| Declarations / End-matter | 11/20 | Incomplete |
| References | 13/20 | Ordering problem |

---

## 1. Title Page — 17/20

**Strengths:** Descriptive title. Two corresponding authors now listed with emails. Affiliations on separate lines. Word counts, figure/table counts, disclosure, and clinical trial status all present.

| # | Issue | Suggested Edit |
|---|-------|---------------|
| 1.1 | Keywords use semicolons | Change to middle dots to match published ABME style: "Head-torso coupling · Kinematic response · Video-based motion analysis · Muscle activation" |
| 1.2 | No ORCID for corresponding authors | Springer increasingly requires ORCID. Add ORCID iDs for Kudzia and Cripton beneath their emails. |
| 1.3 | "Disclosure: None" is informal | Change to "Disclosures: The authors have no relevant disclosures." or remove entirely since Competing interests covers this. |

---

## 2. Abstract — 18/20

**Strengths:** Structured format (Purpose/Methods/Results/Conclusion) now matches ABME style. Quantitative results are specific. Word count (220) falls within the 200-250 range. Conclusion is concise and actionable.

| # | Issue | Suggested Edit |
|---|-------|---------------|
| 2.1 | "in vivo" not italicized | Italicize: "*in vivo*" |
| 2.2 | Purpose opens with surrogate limitation rather than the broader clinical problem | Consider leading with the clinical gap (head-torso coupling during impact is poorly characterized) before narrowing to surrogates. This broadens the audience appeal. |

---

## 3. Introduction — 16/20

**Strengths:** Clear problem statement in paragraph 1. Logical flow from clinical significance to biomechanical gap to surrogate needs to study aims. Strong final paragraph stating the hypothesis.

| # | Issue | Suggested Edit |
|---|-------|---------------|
| 3.1 | Paragraph 4 ("Head-torso coupling modulates...") runs ~250 words | Split after "...across a larger effective mass, rather than by reducing peak contact forces." Start a new paragraph at "The degree of head-torso coupling..." |
| 3.2 | "Sports represent the second leading cause of traumatic brain injury in young adults after motor vehicle crashes [16]" — only one citation for a strong epidemiological claim | Verify this claim and add a second supporting reference if available. |
| 3.3 | "No existing surrogate modulates mechanical properties based on muscle activation state." followed by "Researchers adopt a single intermediate stiffness..." | These two sentences say the same thing. Delete one. |
| 3.4 | "Video tracking with fiducial markers measures positions directly, achieving average errors of 1--1.5 mm during impact events [17]." | Specify the context (e.g., "during football head impacts") so the reader knows this accuracy applies to comparable conditions. |
| 3.5 | Several sentences exceed 25 words | Shorten: "Coupling provides this protective effect by distributing impact energy across a larger effective mass, rather than by reducing peak contact forces." (21 words — this one is fine). But "Accelerometers measure acceleration at individual anatomical locations, requiring double integration to obtain position data with associated drift errors." (18 words — fine). Scan paragraph 5 for long compound sentences. |
| 3.6 | Paragraph 6 (study aims) contains "The original study measured head kinematics only." | Move this context to Methods. The Introduction should state your aim, not describe the parent study's limitations. |

---

## 4. Methods — 16/20

**Strengths:** Well-organized subsections. Statistical justification for no multiple comparisons correction is sound. Table 1 variable definitions are excellent. Signal processing pipeline is reproducible.

| # | Issue | Suggested Edit |
|---|-------|---------------|
| 4.1 | Section labeled "2.0 Methods" | Rename to "2.0 Materials and Methods" per ABME guidelines. |
| 4.2 | Video processing subsection (~280 words in the digitization paragraph) is dense | Split the paragraph starting "We tracked a point on the head..." into two: one for head tracking, one for torso tracking. |
| 4.3 | "A single trained operator digitized all trials to maintain consistency." | State who: "A single trained operator (G.B.) digitized all trials..." to establish accountability. |
| 4.4 | "Using Tracker software (Open-Source Physics, version 6.2.0)" | Good version reporting. Add the URL or citation for Tracker if a citable reference exists. |
| 4.5 | Statistical analysis: "We did not apply corrections for multiple comparisons because we prioritized effect size interpretation..." | This justification is valid but could be tighter. Consider: "We did not correct for multiple comparisons because our primary conclusions rest on large effect sizes (d > 1.0), not marginal p-values." (cuts ~15 words) |
| 4.6 | "We report means ± standard deviations with 95% confidence intervals" ends awkwardly — period is on a separate line in the extracted text | Check formatting in the actual docx — likely a stray paragraph break before the period. |

---

## 5. Results — 18/20

**Strengths:** Clear subsection structure (trajectories, coupling, kinematics, angular). Quantitative throughout with p-values and effect sizes. Good use of "all 19 participants" to emphasize universality. Tables 2 and 3 are comprehensive and well-formatted.

| # | Issue | Suggested Edit |
|---|-------|---------------|
| 5.1 | "Video derived spatial trajectories" subsection title | Hyphenate: "Video-derived spatial trajectories" |
| 5.2 | "Individual reductions ranged from 6% to 62%." | Strong detail. Consider adding this range for coupling metrics too (relative excursion range). |
| 5.3 | Torso displacement paragraph: "though individual responses varied widely, ranging from a 33% increase to a 36% decrease" | This bidirectional variability deserves one more sentence of interpretation. Why did some participants' torsos move more under co-contraction? |

---

## 6. Discussion — 15/20

**Strengths:** Addresses the hypothesis directly. Discusses surrogate design implications (paragraph 3). Honest limitations. Future directions are specific and feasible.

| # | Issue | Suggested Edit |
|---|-------|---------------|
| 6.1 | Opening paragraph (~180 words) largely repeats Results | Cut by 40-50%. Keep: study aim, key finding (30% head displacement reduction, 36% coupling reduction, unchanged acceleration), and the mechanistic interpretation. Remove redundant statistics already in Results. |
| 6.2 | Limitations paragraph runs ~220 words as a single block | Split into three shorter paragraphs, one per limitation: (1) sample demographics and single severity, (2) video digitization resolution and torso tracking variability, (3) two discrete activation states only. |
| 6.3 | "These methodological differences caution against direct comparison of our kinematics with those reported by Reynier et al. (2020)" | Good, but the sentence that follows ("Center of mass measurement at higher sampling rates provides more accurate kinematics than surface tracking.") reads as self-deprecating without payoff. Follow immediately with: "Despite these differences, both approaches found unchanged peak acceleration, reinforcing this finding's robustness." |
| 6.4 | Future research paragraph mixes two topics: (1) participant/protocol extensions and (2) computer vision methods | Split into two paragraphs. The computer vision content (DeepLabCut, OpenPose) reads as tangential; tighten to 2-3 sentences. |
| 6.5 | "In conclusion" paragraph repeats the opening discussion paragraph and the Abstract conclusion | Cut by 30%. Remove any statistic already stated in Results and the opening discussion paragraph. Focus on the take-home message and what the field should do with these data. |
| 6.6 | "our data does not address" | "our data do not address" (data is plural) |

---

## 7. Declarations / End-matter — 11/20

**Strengths:** Author contributions use CRediT taxonomy. Data availability addresses both processed and raw data. Funding acknowledges both the secondary analysis and original study.

| # | Issue | Suggested Edit |
|---|-------|---------------|
| 7.1 | No "Statements and Declarations" parent heading | Add "Statements and Declarations" as the parent heading above all declaration subsections, per ABME requirements. |
| 7.2 | Missing "Ethics approval" declaration | Add: "**Ethics approval.** The original experimental protocol was approved by the University of Virginia Institutional Review Board (Reynier et al. 2020). The present study is a secondary analysis of video recordings collected under that approved protocol." |
| 7.3 | Missing "Consent to participate" declaration | Add: "**Consent to participate.** All participants provided written informed consent for both the original data collection and future secondary analyses." |
| 7.4 | Missing "Consent for publication" declaration | Add: "**Consent for publication.** Participants consented to use of video recordings for research purposes. Raw footage is not published due to participant identifiability." |
| 7.5 | Redundant conflict of interest line at bottom | Line 167: "Declarations Conflict of interest No potential conflict of interest was reported by the authors." duplicates "Competing interests" above. Remove the redundant line. |
| 7.6 | Declarations not ordered per ABME convention | Reorder to: Ethics approval, Consent to participate, Consent for publication, Author Contributions, Competing interests, Funding, Data availability. |

---

## 8. References — 13/20

**Strengths:** Consistent format (Author. Title. *J. Abbrev.* vol:pages, year). All authors listed (no et al.). Paperpile hyperlinks removed. Duplicate Dibb et al. reference removed.

| # | Issue | Suggested Edit |
|---|-------|---------------|
| 8.1 | References are now in order of citation (sequential), not alphabetical | ABME requires references "arranged alphabetically by author and numbered serially." Re-sort all references alphabetically by first author surname, renumber, and update all in-text citations accordingly. |
| 8.2 | All 41 references run together as a single text block | Add line breaks between each reference for readability (one reference per line/paragraph). |
| 8.3 | Ref 36 (Liu et al. 2025) lists only a DOI, no volume or pages | Add "Epub ahead of print" or "in press" after the DOI to clarify publication status. |
| 8.4 | Ref 39 (Cao et al. 2019) lists only a DOI, no volume or pages | Same — add volume/pages if now available (this paper has been published: *IEEE Trans. Pattern Anal. Mach. Intell.* 43:172-186, 2021). Update the year and page numbers. |
| 8.5 | Refs 12 and 14 (both Viano, Casson, Pellman, 2007) have nearly identical titles | These are distinct publications (Part 14 vs. general reconstruction) but a reviewer may question it. Ensure in-text citations point to the correct paper. |

---

## Top 5 Priority Actions

1. **Re-alphabetize references** and renumber all in-text citations (item 8.1) — this affects the entire manuscript.
2. **Add Statements and Declarations** with Ethics approval, Consent to participate, and Consent for publication (items 7.1-7.4).
3. **Rename "Methods" to "Materials and Methods"** (item 4.1).
4. **Trim Discussion redundancy** — cut the opening and concluding paragraphs by ~30-40% (items 6.1, 6.5).
5. **Split long paragraphs** in Introduction (item 3.1), Methods (item 4.2), and Discussion limitations (item 6.2).
