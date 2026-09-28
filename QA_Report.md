# QA Report: Thesis_Final.docx

**Thesis:** بررسی عوامل کلیدی موفقیت و بهره‌وری صرافی‌های رمزارز در ایران (مورد مطالعه استارتاپ‌های کریپتویی)
**Input:** `Draft_5_Final_References.docx` · **Formatting reference:** `__ نازی پایان نامه_.pdf` · **Audit date:** 2026-09-28

---

## 0. Status: NOT final

`Thesis_Final.docx` is structurally complete, validates against the OOXML schema, has no tracked changes, comments or hidden text, and was inspected page by page in a rendered copy. **It cannot yet be called final** because of the blockers below. Only you can resolve them.

| # | Blocker | Why it blocks | What is needed from you |
|---|---|---|---|
| B1 | **Appendix A (پیوست الف) is missing.** The text says the interview protocol and the full transcripts are in Appendix A (§3-8-3, §4-1, §4-4-2). Neither the draft nor the project folder contains them. | A cited appendix that doesn't exist; the 95 open codes also can't be checked against transcripts. | The protocol and transcript files. They can then be appended after a «پیوست‌ها» cover page, as in Nazi's thesis. |
| B2 | **The Phase-1 publisher table (Tables 3-5 and 4-1: Springer 29, Elsevier 34, Emerald 14, Wiley 11, OECD 6 = 94) contradicts your own 40-source corpus (Table 4-4).** The 40 selected sources include 8 Persian-language journal articles, several MDPI and ACM papers, and theses/course papers from university repositories. None of these can come from those five publishers, yet the selected sources must be a subset of the identified ones. Nazi's thesis uses the *same five publishers* (Springer 80, Elsevier 92, Emerald 38, Wiley 30, OECD 21 = 261), so this table looks carried over from her template. | An unsupported data table in the method and findings chapters. The screening funnel 94→89→61→45→40 (Table 4-3) is also undocumented. | The real search log (database, query, hits per database, screening counts), or a decision to rewrite §3-7-1 / §4-3-2 / §4-3-3 around what can be documented. **I did not change these numbers.** |
| B3 | **8 in-text citations have no reference-list entry** (see §4.2). | Citation integrity. | Full bibliographic details. I didn't invent them. |
| B4 | **Items that need your confirmation in the English back matter** (§3.8). | Transliteration and date conventions are your call. | Confirm or correct them. |

---

## 1. What was done and how it was checked

1. **Shell access** was checked with a harmless command (`echo ok`) before any work.
2. **Everything was read first:** the full draft (all paragraphs and all 66 tables), Nazi's thesis (all 254 pages, examined as page images because its PDF text layer is corrupted), and all 43 source files. Scanned or garbled PDFs were read from page images. Appendix A and an existing `Thesis_Final.docx` were not present.
3. **Source validation:** each key claim was traced from claim → citation → reference entry → full text of the source (§4).
4. **Chapter 4 audit:** every number was recomputed by script from the coding matrices (§2).
5. **Editing** was done with scripts on the Word XML so formatting, footnotes and tables were preserved. Every text change is listed in §3.
6. **Final QA:** schema validation passed; there are no `w:ins`/`w:del`/comment/`vanish`/`highlight` elements; metadata was cleaned; caption numbering is sequential in every chapter; every «جدول/شکل n-m» reference points to an existing caption; TOC/LoT/LoF page numbers were measured from a render and re-measured after insertion (0 differences); all 175 rendered pages were visually inspected.

**Tooling caveat:** the preview PDF (`Thesis_Final_preview.pdf`) was rendered with LibreOffice. *B Nazanin* is not available here, so the similar *Nazli* font was substituted. Line breaks in Word with B Nazanin may differ slightly. The document is set to prompt Word to update fields on opening. **Accept that prompt** (or press Ctrl+A, then F9) so Word recalculates TOC and list page numbers with the real font.

---

## 2. Chapter 4 audit (Shannon entropy and Kappa remain fully excluded)

### 2.1 Checks that passed (no numerical change was needed)
Recomputed from the six 25-column coding matrices (Tables 4-18, 4-20, 4-22, 4-24, 4-26, 4-28):

- All 95 row sums equal the «جمع» column.
- All 95 frequencies in the priority tables (4-19…4-29) match the matrices.
- All percentages equal f/25, rounded.
- All case spans («گستره موردها») match the A–E columns.
- All within-category ranks are correct (tied values share a rank).
- For all 95 codes, the interviewee quoted as the example source in Table 4-16 is marked 1 for that code in the matrix.
- Open-code labels are identical in Tables 4-16, 4-17, the matrices and Table 4-30.
- Table 4-30 (95 rows): frequency, percentage and span all consistent.
- Table 4-31: codes per class 13/16/11/19/21/15 = 95; references 70/108/36/94/130/76 = 514; shares 14/21/7/18/25/15 %. Correct.
- Table 4-32: per-case code counts 41/55/36/39/25 and reference totals 82/140/103/102/87. Correct.
- Table 4-33 (12 codes with span ≥ 4) and the span distribution 38/29/16/8/4. Correct.
- Table 4-34: 8 codes found only in case A, and 10 codes absent from A but present in ≥ 3 active cases. Correct.
- Model figure 4-1: all rank numbers in parentheses are correct.
- Phase 1: Table 4-5 has 29 factors and 78 references; each row's count equals its listed sources; Tables 4-8…4-14 frequencies, percentages and ranks are correct.
- Number of axial categories = **21** (3+3+3+4+4+4).

### 2.2 Corrections that the data forced
| Location | Draft | Corrected | Evidence |
|---|---|---|---|
| Abstract | «۲۰ مقوله محوری» | «۲۱ مقوله محوری» | Table 4-17 contains 21 distinct axial categories |
| §4-3-3 (two places), §5-1 | «سی‌ویک منبع بین‌المللی و نُه منبع فارسی» | «سی‌ودو منبع انگلیسی‌زبان و هشت منبع فارسی‌زبان» | Table 4-4 rows 33–40 are the only Persian-language sources. Jaladati & Chitsaz (2023) and Ghaffary Fard et al. (2026) are English-language articles (checked in the PDFs) |
| §4-5 paragraph after Table 4-34 | Claimed all 10 codes absent from A show «وجود قابلیت», listing «انجام تحقیق کاربر» | Rewritten: 5 of the 10 are execution mechanisms (O25, O26, U32, O35, T13); the others (N21, M41, U15 *limited* user research, U25, T12) are scale-related issues | U15 is «محدود بودن تحقیق کاربر…», i.e. the opposite of «انجام تحقیق کاربر» |
| Table 5-4 | Fee structure: interview rank «اول» | «چهارم (M11)» | M11 is ranked 4th in Table 4-25 |
| Table 5-5 | Knowledge management: interview rank «—» | «چهارم (O13)» | O13 «جابه‌جایی نیرو و از دست رفتن دانش سازمانی» exists and is ranked 4th in Table 4-27 |

### 2.3 Not verifiable (recorded, not changed)
- **Codes vs. transcripts:** transcripts are unavailable (B1). The coding was checked for internal consistency only.
- **Table 3-4 user-scale figures:** already labeled in the thesis as self-reported.
- **Phase-1 expert confirmation** of the six-class grouping (Table 4-7) and the **three-expert protocol review** (Table 3-7): no documentation in the project files.
- **Table 4-7 «all 40 sources re-read against full text»:** the project folder has no usable file for Galati (2024), Mann (2023) or Magnusson & Stenberg (2022). See §4.3.

---

## 3. Changes made

### 3.1 Structure and formatting (matched to Nazi)
- **Page:** US Letter, as in Nazi (measured 612×792 pt). Margins: right (binding side) 3.5 cm, left 2.35 cm, top and bottom 2.54 cm. Before, the draft mixed A4, A4-landscape and Letter sections.
- **Orientation:** the draft switched portrait/landscape about 13 times, which turned plain text pages landscape. Now everything is portrait except the six 29-column coding matrices, each on its own landscape page (Nazi is portrait throughout; the matrices can't fit portrait legibly).
- **Front matter in Nazi's order:** title page → «بنام یگانه شایسته پرستش» page → dedication → abstract → فهرست مطالب → فهرست جداول → فهرست اشکال. The front matter is numbered with Persian letters (ا، ب، پ…), as in Nazi; the body restarts at 1.
- **Title page:** centered, with graded sizes. The duplicated empty «استاد راهنما» line was removed (see §5).
- **Chapter cover pages:** each chapter opens on a separate page with a teal box containing the chapter title, following Nazi's design.
- **Heading hierarchy:** Chapters 3–5 headings (previously plain «Normal» text, so missing from the TOC) are now proper Heading 1–4 styles. Numbering was normalized to Nazi's «۲-۳-۳) عنوان» format (fixed «۲-۳-۳( », «۲-۷-۵.», «۲-۳)صرافی…»). Empty headings were removed. Chapter 4's duplicated title (it appeared twice with different wording) was merged into «فصل چهارم: تجزیه‌وتحلیل داده‌ها و اطلاعات».
- **Body text:** B Nazanin 14 pt, justified, 1.5 line spacing, first-line indent, Times New Roman for Latin text. The draft had double spacing and a mix of «Compact» and «Normal» styles.
- **TOC / List of Tables / List of Figures:** real Word fields (levels 1–4; «Table Caption» and «Figure Caption» styles) with dot leaders, pre-filled with measured page numbers. The old TOC was stale (it listed 4-x headings that had lost their heading style).
- **Captions:** table captions above tables, figure captions *below* figures (as in Nazi), bold and centered. «منبع:» notes are styled separately.
- **Tables:** right-to-left column order (6 tables were left-to-right), blue borders (#4F81BD), shaded header row (#B8CCE4), alternate-row banding (#DBE5F1) as in Nazi, header rows repeat across pages, full text width.
- **Footers:** centered page number on every page. The draft had none.
- **References:** heading «فهرست منابع» with «الف) منابع فارسی» and «ب) منابع انگلیسی», numbered entries as in Nazi, hanging indent, left-to-right layout for English entries.
- **Back matter added from existing content only:** an **English Abstract**, translated from your Persian abstract, and an **English title page**, as in Nazi's thesis.

### 3.2 Renumbering (Chapter 3 had gaps and misnamed objects)
| Old | New |
|---|---|
| «شکل ۳-۲» (the seven-step table) | «جدول ۳-۱» |
| جدول ۳-۶ / ۳-۷ / ۳-۸ | جدول ۳-۲ / ۳-۳ / ۳-۴ |
| untitled «ابزار گردآوری اطلاعات فاز اول» table | «جدول ۳-۵) توزیع منابع شناسایی‌شده در فاز اول بر حسب پایگاه یا ناشر علمی» |
| جدول ۳-۹ / ۳-۱۰ | جدول ۳-۶ / ۳-۷ |
| «شکل ۳-۴» | «شکل ۳-۱» |
| references to non-existent «شکل ۳-۱» (Ch. 2, Table 2-5) | «جدول ۴-۱۷» |
| reference to non-existent «بخش ۳-۱۱» | «بخش ۱-۷» |

All cross-references across chapters were updated.

### 3.3 Citation and source corrections
- **Au et al. (2024), LAS-VICT "C":** the draft described it as «حساسیت به الزامات مقرراتی … کنترل‌های ضدپول‌شویی». The paper defines it as *compliance* measured in two dimensions, **legal and social** (H8/H9). It does not mention AML. Corrected in Ch. 1, §2-7-4 and Table 4-4.
- **Brauneis et al. (2022), §2-8-1:** the draft said liquidity is partly platform-driven and therefore «قابل مدیریت توسط بنگاه». The paper finds liquidity explained by the *same exchange's past liquidity, market-wide liquidity and volatility, and on-chain BTC fees*, and detached from traditional markets. Rewritten to match the source.
- **Table 2-4:** «Davidson et al., 2022» corrected to «Davison et al., 2022».
- **§2-8-2:** «Ghaffary Fard … تنها مطالعه‌ای در فهرست منابع فعلی» (draft wording) replaced with a neutral phrasing.
- **§4-6:** «تنها منبع بین‌المللی … مطالعه ایرانی» (self-contradictory) rewritten to cite Ghaffary Fard et al. (2026) explicitly.
- **Removed: citations with neither a reference entry nor a source file.** The full removed text is kept here so you can restore any of them if you have the source:
  1. §1-1: «بلاک‌چین با فراهم‌کردن بستری برای تعریف انواع جدیدی از خدمات مالی، از جمله اعتبار و پس‌انداز جدای از خدمات پرداخت صرف، زمینه‌ساز شکل‌گیری الگوهای تازه‌ای از کارآفرینی در این حوزه شده است (علیزاده صیقلان و همکاران، ۱۴۰۰).»
  2. §2-4-4: «احمدی و کریمی (۱۴۰۲) چالش‌های نظارتی و حاکمیتی صرافی‌های رمزارز در ایران را تحلیل کرده‌اند؛ یافته آن‌ها این است که نبود چارچوب حاکمیتی متناسب با ماهیت فناوری رمزارز، مسئولیت‌پذیری نهادی صرافی‌ها را کاهش می‌دهد و به ناهمگونی در سیاست‌های امنیتی و شفافیت اطلاعات میان پلتفرم‌های مختلف می‌انجامد. …» (and its repeat in §2-8-2)
  3. §2-4-4: «رضایی و ابراهیمی (۱۴۰۱) اخلاق و مسئولیت در اکوسیستم رمزارز را با مطالعه موردی صرافی‌های ایرانی بررسی کرده‌اند … گیمیفیکیشن …»
  4. §2-4-4: «مروت و نظری‌زاده (۱۴۰۱) با روش تحلیل اثرات متقاطع، سناریوهای آینده استارتاپ‌های فین‌تک و بانکداری ایران تا افق ۱۴۱۰ …»
  5. §2-4-4: «یعقوبی و همکاران (۱۴۰۱) با تحلیل داده‌های ۶۶۵ پروژه … دیفای …»
  6. §2-4-4: «علیزاده صیقلان و همکاران (۱۴۰۰) فرصت‌های کارآفرینی مبتنی بر بلاک‌چین را در قالب چهار محور …»
  7. §3-5: «فرامطالعه شامل سه قسمت است … (چنیل و وس، 2007)»

  Items 2–5 read like generic placeholder citations (common surnames, very specific claims, no bibliographic trace anywhere in the project). Please treat them as unverified unless you hold the papers.

### 3.4 Chapter 5 (rebuilt on Nazi's Chapter 5 structure and your Chapter 4 findings)
Nazi's Chapter 5 structure: 5-1 introduction → 5-2 analysis by research question (main question, then 5-2-1 per-component summary and discussion, each with a "researchers' rank vs. experts' rank" table) → 5-3 recommendations → 5-4 limitations → 5-5 suggestions for future research. Your draft already followed this skeleton. Changes:
- Each 5-2-1-x section now opens with its **research sub-question**, quoted verbatim from §1-6 (Nazi restates each component's question).
- Comparison Tables 5-1…5-6: every rank now shows the **matched code** (e.g. «چهارم (M11)») so it can be traced to Chapter 4. Two wrong ranks were fixed (§2.2). The note that was repeated six times was merged into one note under Table 5-1.
- Claims were softened wherever they went beyond the data: the difference between the discontinued and active cases is described as a **descriptive** observation, not a causal one. «تمایز … در برخورداری از منابع بیشتر نیست» became «… بیشتر در انضباط اجرایی دیده می‌شود (میزان منابع موردها مقایسه نشده است)», because resource levels were never compared.
- No new findings, theories or numbers were introduced. Every number in Chapter 5 is copied from Chapter 4.
- The abstract's paragraph on findings was rewritten to match Chapter 4. The draft's version («پایداری زیرساخت فنی شرط لازم … برای … بهره‌وری سازمانی») did not match the conditional ordering actually stated in §4-7. The method paragraph now mentions Phase 1 (meta-synthesis), which the abstract had omitted.

### 3.5 Writing cleanup
- **Draft and audit residue removed:** «برخلاف نسخه‌های پیشین این فصل…», «در نسخه اولیه این جدول ستونی … پیش‌بینی شده بود…», «تصریح روش‌شناختی/شمارشی…», «هر عددی … قابل بازتولید است», «هیچ روش تحلیلی تازه‌ای … به کار نرفته است», «این تفکیک، مرز میان ادعای روش‌شناختی و اجرای واقعی…», and the paragraph naming Shannon entropy and Kappa. **Shannon entropy and Kappa no longer appear anywhere in the thesis.** The limitation itself (no second coder, so no inter-coder agreement) is kept.
- **Chapter 3 passages that reproduced Nazi's methodology text almost verbatim** were rewritten in your own words with the same meaning and citations: §3-1 intro, the paradigm passage, §3-3, the meta-study paragraph (which also had typos: «عمید», «رفاتئوری», «گه»), §3-6, the interview passages («الری جنسیک … موورد»), and the Phase-1 validity paragraph. The duplicated §3-4 paragraph (same content twice) was removed.
- «به‌مثابه» was replaced with «به‌عنوان» in 19 prose places. **Code labels were not touched** (they are research data).
- Missing zero-width non-joiners fixed in the Phase-1 reliability paragraph («داده‌ها»، «به‌صورت»، «مرحله‌ای» …).
- Chapter 5 opening: the sentence copied from the start of Chapter 4 was replaced.

---

## 4. Source validation

### 4.1 Claims verified against the full text
Au et al. 2024 (LAS-VICT definitions, MTurk, SmartPLS, 213 valid responses, "costs necessary but not sufficient"); Au et al. 2025 (tri-ecosystem; Uphold case; research-in-progress paper); Usman et al. 2026 (389 Binance users in Indonesia, PLS-SEM, system quality the strongest determinant); Sapkota 2025 (845 exchanges; centralized, fewer coins, high withdrawal fees, no US restriction → default); Lee & Milunovich 2023 (volume, staff information, lifetime, cybersecurity features); Brauneis et al. 2022 (after correction); Bucko et al. 2015 (volatility, e-wallet theft); Yu et al. 2022 ("significantly insufficient and immature"; top ten platforms); Vidal-Tomás 2025 (proof-of-assets, extra reserves of 6–14%, "guardians of trust"); Gandal et al. 2018 (suspicious Mt. Gox trading); Bentov et al. 2019 (Tesseract, trusted hardware); Chutipat et al. 2023 (Thailand, binary logistic regression, gender and education); Fröhlich et al. 2022 (99 articles, six themes including trust, risk perception, wallets); Hudaverdi 2025 (Zagreb, convergent-parallel mixed methods; Coinbase, Binance, Bitstamp); Estavi 2023 (LUT master's thesis; economic and social sustainability); Kristensen 2020 (CBS master's thesis; customer centricity); Kurkinen 2023 (HAMK bachelor's thesis; fees, UX and security as a basis for competitive advantage); Lee & Shin 2018 (five ecosystem elements, six challenges); Gai et al. 2018 (five technical aspects); Arner et al. 2016 (FinTech 3.0 led by start-ups); Suryono et al. 2020; Voznesenska 2025; Thomas n.d. (DePaul HCI522 course paper, unpublished); Ghaffary Fard et al. 2026 (AHP, 13 experts, weakness of macro-management 0.429, root cause of other challenges); Sadeghi et al. 2026 (mixed methods: 7 exchanges including Binance, Kraken and Uniswap, plus DANP with experts); ناصحی‌فر و همکاران ۱۴۰۲ (42 themes in 12 groups, ISM); آینه و همکاران ۱۴۰۳ (0.951 specialized capital markets); خزاعی و همکاران ۱۴۰۱ (n = 384, PLS); صدرایی و همکاران ۱۴۰۳ (CVR; infrastructure, regulatory, distrust, cultural); روشنی و همکاران ۱۳۹۹ (title «با رویکرد جامعه‌شناسی» confirmed; the PDF file name is misleading); Jaladati & Chitsaz 2023 (English article; grounded theory, 26 interviews).

### 4.2 Citation problems (unresolved; need your input)
| Citation | Problem |
|---|---|
| سخدری ۱۳۸۵، خاکی ۱۳۸۴، دانایی‌فرد و همکاران ۱۳۸۴، نیومن ۱۳۸۹، کرسول ۱۳۹۱، بازرگان و همکاران ۱۳۹۰، اوپنهایم ۱۳۶۹ | Cited in Chapter 3 but **missing from the reference list**. They come from the methodology text shared with Nazi's thesis. Add full entries. |
| Zimmer (2004) | Cited in §3-5, **missing from the reference list**. Nazi's list has: Zimmer, L. (2006). *Qualitative meta-synthesis: A question of dialoguing with texts*. Journal of Advanced Nursing, 53(3), 311–318. **Note the year: 2006, not 2004.** Please check against the source you actually used. |
| Sandelowski & Barroso (2007) | In the reference list, but no source file in the project. |
| Werth et al. 2023, Rockart 1979, Makarov & Schoar 2020, Zetzsche et al. 2020, Xia et al. 2020, Fang et al. 2022, Mann 2023, Magnusson & Stenberg 2022, اسدالله و همکاران ۱۳۹۸، روحانی‌راد ۱۳۹۹، عربیون و همکاران ۱۴۰۲، محمدکاظمی و همکاران ۱۴۰۰ | In the reference list, but **no source file in the project**, so their claims could not be verified. عربیون ۱۴۰۲ also lacks volume, issue and pages. |
| Galati (2024) | The only "source" file is a saved ScienceDirect security-check page with no article text. The claim about Binance zero fees (wider spread, lower depth, higher total cost) is plausible but **unverified**. |
| Barney (1991), Pavlov et al. (2024) | Scanned PDFs with no text layer. Only the bibliographic details were verified, from the page images. |
| مرادی و همکاران ۱۳۹۹، باغانی ۱۳۹۹ | PDF text layers are unreadable (broken font mapping). Title, journal and year were verified from page images; **content claims were not verified**. |
| Davison et al. (2022), Table 4-4 "key finding" | «کاربردپذیری و امنیت، دو معیار اصلی انتخاب…» comes from the paper's *motivation* («users are lost as to which exchanges provide the best usability or security»). It is not a result. The actual study is AHP with 34 experts and six criteria. **Partially supported.** |
| مشهدی عبدل و همکاران ۱۳۹۸, Table 4-4 method | Listed as «کیفی ـ داده‌بنیاد». The paper combines grounded theory, a questionnaire and SWOT. Partially accurate. |
| Kurkinen (2023), §2-8-1 | The claim that security and performance are "not independent axes" was not found in the thesis text. **Unverified.** |

### 4.3 Source file problems
- **Duplicates:** Estavi (2 identical files), باغانی (2), مشهدی عبدل (2), ناصحی‌فر (2), روشنی (2; one is a scanned copy with no text).
- **Misleading file names:** «THE ROLE OF SUSTAINABLE BUSINESS MODEL…» is Estavi's thesis; «رمسگطایی تأمین مالی…» is the English article by Jaladati & Chitsaz; «اینه معصمه» is آینه و همکاران.
- **Not a paper:** the Galati `.html` file (security-check page).
- **Nazi's thesis** is used only as the formatting and Chapter 5 structural reference. None of its research content was copied into your thesis. Only template passages that the draft *had already* borrowed were rewritten (§3.5); the one remaining carry-over is B2.

---

## 5. Unsupported or weakly supported claims still in the text (recorded, not changed)
1. §1-2 opening: growth in Iranian users and trading volume. No citation.
2. §1-4 (fourth necessity): new users compare Iranian exchanges with global ones. No citation.
3. §2-3-4 last paragraph: rial and stablecoin pairs are the backbone of the Iranian market and liquidity is lower than on international platforms. No citation.
4. §3-7-1 / Tables 3-5, 4-1, 4-3: the search and screening numbers (see B2). The draft's «طی ۱۰ سال اخیر» was changed to «عمدتاً در ده سال اخیر» because the 40-source sample includes Barney (1991).
5. Galati (2024) and Kurkinen (2023) claims (see §4.2).
6. The title page had a second, empty «استاد راهنما» label with no name. I removed it. **If there is a co-supervisor or an advisor (استاد مشاور), please add them.**

---

## 6. Formatting differences from Nazi that could not be fully matched
| Item | Status |
|---|---|
| Font | B Nazanin is specified throughout. The preview PDF uses the substitute Nazli font because B Nazanin isn't installed on the build machine, so final pagination must be refreshed in Word (update fields). |
| Chapter cover box | Nazi uses a rounded, gradient teal box; this file uses a teal rectangle with a thick border (Word tables can't have rounded corners). |
| Digits in the preview | LibreOffice shows page numbers with Latin digits. Word shows Persian digits in Persian context. |
| Latin citation years | Nazi writes years in Persian digits inside Latin citations, e.g. (Harrison, ۲۰۱۰). The draft uses APA style with Latin digits. Kept, because APA is more consistent. |
| Reference style | Nazi's reference list mixes styles. Yours was kept in APA 7, with Nazi's layout (two numbered sections). |
| Acknowledgements page (تشکر و قدردانی) | Nazi has one. Your draft doesn't, and I didn't write one for you. |
| Appendices section | Nazi has a «پیوست‌های پژوهش» cover plus the interview protocol. Yours is missing (B1). |
| Six coding matrices | Placed on landscape pages. Nazi uses portrait, but her matrices are much narrower. |
| Paragraph right after some tables | Slightly tight spacing below a few tables in the render. This is cosmetic and may differ in Word. |

---

## 7. English back matter: please confirm (B4)
- Name: **Mostafa Mozhdeh Shafagh** (my transliteration of مصطفی مژده شفق)
- Degree line: **Master of Science (M.Sc.) in Entrepreneurship Management, New Business Creation** (follows Nazi's "Master of Science"; your faculty may prefer M.A.)
- Institution: **University of Tehran, College of Farabi** (from «دانشگاه تهران، دانشکدگان فارابی»)
- Date: **March 2026** (اسفند ۱۴۰۴ spans 20 Feb – 20 Mar 2026)
- The interview period is given as "March to December 2025" (فروردین–آذر ۱۴۰۴).

---

## 8. Deliverables
- `Thesis_Final.docx`: the edited thesis (175 pages in the render).
- `Thesis_Final_preview.pdf`: LibreOffice render used for the page-by-page check (substitute font; for review only, not for submission).
- `QA_Report.md`: this report.
