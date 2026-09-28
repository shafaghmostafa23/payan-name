# FINAL QA REPORT — Thesis_FINAL.docx (final cleanup and submission pass)

Thesis: «بررسی عوامل کلیدی موفقیت و بهره‌وری صرافی‌های رمزارز در ایران؛ مورد مطالعه استارتاپ‌های کریپتویی»

- **Base file:** the latest `Thesis_FINAL.docx`, the 65-reference version from the previous finalization.
- **Note on the upload:** the attached `Thesis_Final_1.docx` is the older 51-reference version, so it was not used as the base.
- **Standard:** `shivehnamehpn.pdf` (University of Tehran thesis guide).
- **Also used:** the source PDFs in the repository and Appendix A (`Appendix-A-Interviews-Revised_1_1.docx`).

## 0. Read first: the correction file was not available

The file **«mostafa shafagh payan name» was not in the upload or the repository**, including every branch and the full git history. Instead, every mistake identified in the three earlier QA reports was used as the correction list:

- `QA_Report.md` on the compassionate-mccarthy branch;
- `QA_Report.md` on the intelligent-archimedes branch;
- `FINAL_QA_REPORT.md`.

As requested, this list was used as a pattern library: each item was searched for across the whole thesis, not only where it was first reported. If the correction file contains items not listed in §2, they have not been checked.

## 1. Summary counts

| Item | Value |
|---|---|
| Final reference count | **65** |
| Persian references | **17** |
| English references | **48** |
| In-text citation instances (all mapped to the reference list) | **446** (366 Latin + 80 Persian), covering 65 distinct sources |
| Unmatched citations (citation without a reference entry) | **0** |
| Unused references (entry never cited) | **0** |
| References removed as unused or unsupported | **0**: every entry is cited, and no entry was found to be a fabricated source |
| Numbered tables | **53** (Ch2: 5, Ch3: 6, Ch4: 36, Ch5: 6), numbered in sequence and all referenced in the text |
| Numbered figures | **5** (2-1, 3-1, 3-2, 4-1, 4-2), all referenced |
| Track changes (`w:ins`/`w:del`) | **0** |
| Comments | **0** |
| Shannon / entropy | **0** in the thesis. Two mentions found in Appendix A («ماتریس آنتروپی») and one in its methods note («ماتریس تصمیم آنتروپی شانون») were removed. |
| Kappa | **0** |
| TODO / TBD / [citation needed] / «□» placeholders | **0** |
| AI or production notes (Claude, ChatGPT, drafting notes) | **0** |
| Corrections extracted from the correction sources (see §0) | **45** |
| Corrections applied in this pass | **21** |
| Corrections already fixed (verified in the current text) | **17** |
| Checked against the source and found correct, so no change needed | **2** |
| Unresolved (need the author's records or decision) | **5** |
| Unsupported or overstated claims removed or rewritten | **52** (listed in §3) |
| Persian abstract / English abstract | 299 / 298 words (limit 300) |
| Pages (LibreOffice render, A4, substitute Nazli font) | 253 in total. The main text is pages 1–150; the reference list is 151–156; Appendix A starts at 157. |
| OOXML schema validation | **Passed** |

## 2. Correction checklist

Sources of the items:
- **M:** QA report on the mccarthy branch.
- **A:** QA report on the archimedes branch.
- **F:** FINAL_QA_REPORT.

Status values:
- **Applied:** fixed in this pass.
- **Already fixed:** verified as fixed in the current text.
- **No change:** checked against the source and found correct.
- **Unresolved:** needs the author.

| # | Src | Issue | Status and evidence |
|---|---|---|---|
| 1 | M | Zimmer 2004 → 2006 | Already fixed (2 citations, both 2006) |
| 2 | M/A | Davidson → Davison | Already fixed (0 occurrences of "Davidson") |
| 3 | M/A | Au et al. (2024) "fees: necessary but not sufficient". The two earlier QA reports disagreed. | **Applied.** The paper's Table 4 says low cost is a "must-be" expectation that "will not provide any advantage". The claim is kept with exact wording in §1-3, §5-2-1-4 and Tables 4-35 and 5-4. |
| 4 | M | LAS-VICT "L" was defined as keeping profit margins low; the paper calls it *low user-burden* | **Applied.** §2-7-4 now defines L as low user-burden, following the paper's Table 2 description and how the authors measured it (financial costs and benefits). |
| 5 | A | LAS-VICT "C" had been described as AML | Already fixed: it is compliance, with legal and social dimensions |
| 6 | M/A | Brauneis et al. (2022): liquidity described as manageable by the firm | Already fixed |
| 7 | M | Lee & Milunovich (2023) predictors | Already fixed |
| 8 | M | «نبود اعتماد، اثر سرمایه‌گذاری در توسعه محصول را خنثی می‌سازد» attributed to Vidal-Tomás and ناصحی‌فر | **Applied.** The claim was still in §2-9-1. It was replaced with what Vidal-Tomás actually shows: proof of solvency used to rebuild trust after exchange collapses. |
| 9 | M | «قیدهای نهادی سقف عملی بهره‌برداری از منابع درونی» attributed to Ghaffary Fard | **Applied.** It was still in §2-9-1. It was replaced with the paper's actual finding: weak macro-level management is the root of the other challenges. |
| 10 | M/A | Sadeghi et al. (2026) method | **Applied.** It is a mixed design: trading data for seven exchanges plus expert-based DANP. Fixed in §2-8-2 and in the Table 4-4 method column. |
| 11 | M | Yu et al. «به‌طور معناداری ناکافی» (implies statistics) | **Applied:** «به‌شدت ناکافی» |
| 12 | M | Usman et al. (2026) key finding worded ambiguously | **Applied.** Now: system quality is the most influential determinant of use and satisfaction; service quality has a limited direct effect. |
| 13 | M | یعقوبی و همکاران claims | Already fixed (absent) |
| 14 | M | «دلالت مستقیم» overclaims (first found for Chutipat) | **Applied** at all 3 occurrences (Chutipat, Werth, Makarov & Schoar) and the similar wording in §2-3-4 |
| 15 | M/A | Cited methodology books missing from the reference list | Already fixed |
| 16 | M/F | Missing bibliographic details (عربیون, Xia DOI, Vidal-Tomás title) | Already fixed |
| 17 | M/A | Table 4-34 text | Already fixed earlier. **Applied now:** one of the 10 codes absent from case A (T12) had been left out of the prose. |
| 18 | M/A | «۳۱ + ۹» → 32 English + 8 Persian sources | Already fixed |
| 19 | M/A | Abstract said 20 axial categories instead of 21 | Already fixed |
| 20 | M | «تفاوتی معنادار» | **Applied.** It was still in §4-4-11 and is now «درخور توجه». A note was also added that the two phases count different units (sources vs. interviewees). |
| 21 | M | «منسجم‌ترین روایت» (case E) | **Applied.** It was still in §4-5. |
| 22 | M/A | §4-6 «تنها منبع بین‌المللی» | Already fixed |
| 23 | M | «هشت کد اختصاصی E … همگی» when only six were named | **Applied.** It was still in §4-5; now «بیشترشان … از جمله», with the omitted codes added. |
| 24 | M/A | Shannon / Kappa removal | Thesis was already clean. **Applied:** entropy references and production notes were removed from Appendix A. |
| 25 | M | Six identical template sentences after Tables 4-8 to 4-13 | **Applied.** They were still templated. They were rewritten, and two tie errors were corrected: the text had wrongly named a single top factor in Tables 4-9 and 4-13, but three factors tie in each. |
| 26 | M/A | Unverifiable citations: احمدی و کریمی، رضایی و ابراهیمی، علیزاده صیقلان، مروت، یعقوبی، سخدری، چنیل و وس، اوپنهایم، «الری جنسیک» | Already fixed (all absent) |
| 27 | M/A/F | Appendix A missing | **Applied.** It is now integrated after the reference list, as the guide's order requires; see §4. |
| 28 | A/F | Phase-1 publisher table contradicted the 40 selected sources | Already fixed |
| 29 | M/A | «ده سال اخیر» vs. Barney (1991) | **Applied.** §3-8-2 and §4-3-2 still said "94 articles in the last 10 years"; now «۹۴ منبع … عمدتاً در ده سال اخیر». |
| 30 | M | Interviewee A5: age 27 with 15 years of experience | **Unresolved.** Appendix A has the same values, so the data were not changed. The author should check. |
| 31 | A | Title page: possible co-supervisor or advisor | **Unresolved** (author) |
| 32 | M | Au et al. (2024) as a source for the fee-structure factor (Table 4-5) | **No change.** The paper does analyse financial costs (H1a/b). |
| 33 | M | Au et al. (2024) MTurk / PLS details | **No change.** Verified from the PDF: MTurk, SmartPLS 4, 213 valid responses. |
| 34 | M/A | Expert reviews (Phase-1 grouping; three-expert protocol review) have no supporting documents | **Unresolved.** These are author-reported and kept as stated; not strengthened. |
| 35 | A | Davison et al. (2022): Table 4-4 finding was taken from the paper's motivation, not its results | **Applied.** Now reports the actual result: AHP, 34 experts, six criteria. The same fix was made in §2-8-1. |
| 36 | A | مشهدی عبدل و همکاران method listed as «کیفی ـ داده‌بنیاد» | **Applied.** The abstract (page 1 image) confirms grounded theory plus a questionnaire and SWOT. |
| 37 | A | Kurkinen (2023): "security and performance are not independent axes" | **Applied.** Not in the source, so removed. Replaced with the thesis's actual findings: user segmentation, volume-based fees, token discounts. |
| 38 | A | Galati (2024): the source file in the repo is a ScienceDirect security page | **Unresolved (residual).** The claims are kept as verified in the previous finalization; the full text is not in the repository. |
| 39 | A | Wrong ranks in Tables 5-4 and 5-5 | Already fixed. All Chapter 5 ranks were re-checked against Tables 4-8 to 4-30. |
| 40 | A/F | §1 market-growth and user-count claims | Already fixed. **Applied:** remaining unsupported claims in §1-1 to §1-4 (see §3). |
| 41 | A | §1-4 "new users compare Iranian exchanges with global ones" | Already fixed (absent) |
| 42 | A/F | §2-3-4 rial/stablecoin pairs claim | Already fixed (absent) |
| 43 | A | English back matter: transliterated name, degree wording, date | **Unresolved** (author to confirm) |
| 44 | M | «به‌مثابه» in running prose (code labels excepted) | Already fixed. **Applied** at 3 more places. |
| 45 | F | Citation page numbers that cannot be verified | Already fixed (none remain) |

## 3. Unsupported or overstated claims removed or rewritten (52)

Each was deleted, reduced to what the cited source actually says, or reframed as the author's assumption.

**Chapter 1 (13)**

1. «مهم‌ترین زیرساخت معاملاتی» (§1-1)
2. "Exchanges are the entry/exit point for most users" (§1-1): no source. Thomas (n.d.) is now cited only for what it says.
3. "Market growth was not matched by exchange maturity" (§1-2)
4. «ریسک‌های سایبری خاص این بستر» (§1-2)
5. Nasehifar attributed a claim about ambiguity fostering innovation and instability (§1-2). Replaced with the verified category «اثر محیط قانونی ایران».
6. Economic claims (capital flight, informal markets, jobs) in §1-3
7. «با افزایش تعداد صرافی‌های فعال» (§1-3)
8. «رشد سریع تقاضا» (§1-4)
9. «رقابت صرافی‌های نسل اول و دوم» (§1-4)
10. "Absence of productivity metrics", which is now limited to "not found in the reviewed sources"
11. §1-7 claim that the literature review used data from 1400–1404 (false: the review includes Barney 1991)
12. §1-7 "continuously serving users", which contradicted the discontinued case A
13. Koidis et al.: "less attention to exchange-level effects" softened to what the review's framing supports

**Chapter 2 (22)**

14. Fang et al. overgeneralisation (§2-1)
15. Revenue from listing fees and institutional services (§2-3-3): uncited, so removed; replaced with Kurkinen's verified finding
16. Two-sided-platform and network-effect claim (§2-3-3)
17. Makarov & Schoar: "price quality largely depends on global connectivity" (§2-3-4)
18. «شرط تداوم فعالیت» stated as an absolute (§2-3-5)
19. «به‌طور فزاینده» (§2-3-6)
20. «در بسیاری از کشورها / پیچیده‌ترین حوزه» (§2-3-7)
21. «هیچ‌یک از این پژوهش‌ها» (§2-4-4), now limited to "among the reviewed studies"
22. "Presented in chronological order" (§2-7): false, since the frameworks are not in date order
23. Kurkinen "not independent axes" (§2-8-1)
24. Chutipat developing-economy generalisation (§2-8-1)
25. Davison "used in this thesis's measurement framework" (no such framework exists)
26. Sapkota: "failure factors are usually visible before the crisis"
27. Makarov & Schoar implication for Iran (§2-8-1)
28. Hudaverdi "disclosure plays the decisive role": replaced with the thesis's actual finding (communication quality as the strongest correlate)
29. Estavi "decision bundle, not a static feature": replaced with the thesis's four themes
30. Nasehifar et al.: level-ordering claim and causal clause replaced with the verified 42 themes / 12 categories / eight-level model
31. §2-9-1 chain of attributions: items 8 and 9 in §2 above, plus «مستقیماً هم‌سو» with an untested model
32. §2-9-2 productivity "main mechanism of success", reframed as the study's assumption
33. §2-3-2 «یافته‌های چنین مقایسه‌هایی نشان می‌دهد», reframed as the author's product-design view
34. روشنی و همکاران (۱۳۹۹): «اعتمادسازی … ابهام شرایط سیاسی» (§2-8-2 and Table 2-4) is not in the paper's abstract. Replaced with the abstract's findings (strategic thinking, communications, marketing mix, founder and team characteristics).
35. باغانی (۱۳۹۹) cited for "risks intensified by limited international access" (§1-2). Replaced with what the paper covers (the need for a regulatory framework).

**Chapter 3 (9)**

36. "Audited performance data do not exist publicly; surveys impossible" (§3-1), rewritten as the researcher's own access situation
37. §3-1 roadmap listed sections that do not exist (scope, ethics, limitations)
38. "Rapid growth of studies" (§3-5)
39. Unsourced "three aims of meta-synthesis" (§3-5)
40. "Balanced distribution prevents dominance / is a necessary condition" (§3-7-2)
41. "Interviews used to validate the proposed framework" (§3-8-1): not done
42. "Random interviewer errors cancel out" (§3-8-3)
43. «تضمین می‌کند … هر شش بُعد دست‌کم با دو محور»: false, since the security dimension has one axis (Table 3-5)
44. «بدون تردید … قطعی خواهد بود» (§3-9-2). The unsourced textbook lists of interview advantages and disadvantages (12 paragraphs) were also removed.

**Chapter 4 (4)**

45. Qualitative analysis "enables generalisation" (§4-1)
46. "International literature rarely treats institutional constraints", now limited to "in this study's corpus" (§4-3-4)
47. "Actors see success in organisation rather than business model" (§4-4-11), now hedged
48. «در ادبیات … دو عامل مستقل و هم‌جهت» (§4-6), now limited to the coded sources

**Chapter 5 (4)**

49. «تلقی خطیِ رایج در ادبیات» (§5-2-1-3)
50. Estavi "sustainability is a condition of long-term survival" (§5-2-1-4 and Table 4-35)
51. Kristensen "customer-centricity" used as unrelated support (§5-2-1-5)
52. «در ادبیات بین‌المللی … صورت‌بندی نشده بود», now limited to the sources reviewed (§5-2-1-4, §5-2-1-6)

**Tables**

In Table 4-4 (Hudaverdi, Estavi, Vidal-Tomás, Thomas) and Table 4-35, the cells above were corrected to match the sources.

## 4. Appendix A

- Integrated after the reference list and before the English abstract, following the guide's order: پیوست الف with sections الف-۱ to الف-۴.
- **Removed** (production or identifying material, not research content):
  - the anonymisation key that named the five exchanges (الف-۴ of the draft);
  - the participant table whose columns were «□» placeholders; it duplicated Table 3-3, and the text now refers to Table 3-3;
  - the draft pre-coding mapping (الف-۷);
  - notes addressed to the researcher;
  - the two "entropy matrix" notes, replaced with a plain statement of which protocol questions went unanswered;
  - references to the "reference thesis".
- **Anonymised:** «بانک مرکزی» and the company name «توسان» were replaced with «[نهاد پشتیبان]», in Appendix A and in the matching quotation in Table 4-16.
- **Headings:** the 25 interview headings and 375 question headings are bold paragraphs, so they stay out of the table of contents. Titles were normalised to the thesis terms («مدیر بازاریابی», «مدیر محصول»).
- **Checked against the thesis:**
  - The protocol's five parts were wrongly described in §3-8-3; the text now follows Appendix A.
  - The 15 protocol questions match Table 3-5.
  - The B5 quote in §5-2-1-1 matches the transcript.
- **Tables corrected to match Appendix A:**
  - Table 3-3: D5 experience changed to «کمتر از یک».
  - Table 3-4: activity periods changed to «حدود ۷ سال» for B (active since 1397–98) and «حدود ۵ سال» for C (launched 1399).
- **No transcript content was changed** beyond the anonymisation above.

## 5. Other fixes

**Footnotes**
- The Liquidity and UX footnote anchors were misplaced; they were moved to the right terms.
- The redundant Sandelowski & Barroso footnote was removed.
- Four footnotes with no anchor in the text were deleted.
- Footnote IDs now run in reading order.

**Chapter 4 consistency**
- The UX class has a tie at frequency 11 (U11 and U22). It was not reported before; it is now in §4-4-6, §5-2-1-2 and Table 4-36.
- The claim that "six classes were not predetermined" contradicted §2-9-3. It now says the six classes follow the six sub-questions, while the 95 codes and 21 axial categories emerged from the data.

**Chapter 5**
- Tables 5-3, 5-4 and 5-5 are now referenced in the text directly.
- A seventh limitation was added: the data come from managers, not users.

**Writing style**
- Repeated template openers such as «نتایج فراوانی ارجاع نشان داد که …» (six times) were varied.
- «در ادامه، فراوانی … محاسبه گردید. جدول … نشان می‌دهد» (six times) was varied.
- First-person-plural passages in Chapter 4 were changed to the thesis's passive voice.
- Absolute wording («در این صنعت», «اتکای شدید») was limited to «در موردهای مطالعه‌شده».

**Metadata**
- 24,916 revision IDs (rsid) were stripped.
- Two stray LRM characters were removed.
- The modified date and page count were updated.
- The author field is the student.

**TOC, List of Tables and List of Figures**
- All page numbers were re-measured from the new render.
- Appendix entries were added to the TOC.
- Word asks to update fields when the file is opened. Accept, so the numbers are recalculated with B Nazanin.

**Chapter 4 data**
- No codes, frequencies, categories, ranks or model elements were changed.
- All matrix row sums, spans, per-case counts (41/55/36/39/25) and case-specific code lists were recomputed and match.

## 6. Unresolved items (need the author)

1. The correction file «mostafa shafagh payan name» was not provided (see §0).
2. Interviewee A5: age 27 with 15 years' experience (Table 3-3 and Appendix A agree, but this looks like a data-entry error).
3. The Phase-1 search export (for the 94 → 89 → 61 → 45 → 40 screening) and records of the expert reviews are missing. The counts are author-reported and were not changed.
4. The signed approval page (صفحه تصویب) is still to be inserted after the title page. Any co-supervisor or advisor should be added to the title page.
5. Confirm the English back-matter wording: the name transliteration, the degree line, and the date "March 2026".
6. Galati (2024): the repository holds only a publisher security page, not the article; the claims rest on the earlier verification.
7. Case B user scale: Table 3-4 says «بیش از ۵ میلیون» (more than 5 million), while Appendix A says «حدود ده میلیون ثبت‌نام‌شده» (about 10 million registered users). These are compatible, but the author may want one figure.

**Rendering note:** previews used LibreOffice with Nazli substituted for B Nazanin, so pagination in Word may differ slightly.
