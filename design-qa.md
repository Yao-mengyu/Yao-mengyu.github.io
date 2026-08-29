# Design QA

## Comparison target

- Source visual truth: `/tmp/zzq-reference-1440.png`, captured from `https://zzq-bot.github.io/`.
- Rendered implementation: `/tmp/academic-research-1440.png`, captured from `http://127.0.0.1:4000/`.
- Combined comparison evidence: `/tmp/research-layout-comparison.png`.
- Responsive evidence: `/tmp/academic-research-mobile.png`.
- Title-treatment references: `/tmp/ref-al-folio.png` and `/tmp/ref-yuzhe.png`.
- Updated title/profile evidence: `/tmp/academic-title-icons.png` and `/tmp/academic-title-icons-mobile.png`.
- Updated combined comparison evidence: `/tmp/title-reference-comparison.png`.
- Canonical-paper-figure evidence: `/tmp/academic-paper-figs-headings.png` and `/tmp/academic-paper-figs-mobile.png`.
- Canonical-figure combined comparison: `/tmp/paper-figs-comparison.png`.
- Corrected-heading and first-page-preview evidence: `/tmp/academic-research-title-transaction-preview.png`, `/tmp/academic-transaction-preview-mobile.png`, and `/tmp/final-paper-preview-comparison.png`.
- Navigation-reference evidence: `/tmp/acad-home-nav.png`, captured from `https://rayeren.github.io/acad-homepage.github.io/`.
- Revised navigation evidence: `/tmp/revised-home-nav.png` and `/tmp/revised-home-nav-mobile.png`.
- Navigation comparison evidence: `/tmp/nav-comparison.png`.
- State: default homepage, light theme, no hover or focused control.

## Normalization

- Source pixels: 1440 × 2400.
- Implementation pixels: 1440 × 2400.
- CSS viewport: 1440 × 2400 for both desktop captures.
- Device scale factor: 1.
- Combined comparison: both full-page captures are presented at equal scale in adjacent columns.
- Responsive capture: 500 × 1400 CSS px and pixels at device scale factor 1; the mobile breakpoint is active.

## Required fidelity surfaces

- Structure: the page now follows the reference sequence `Research [Google Scholar]` → one research-interest paragraph → consecutive image-and-text publication rows.
- Publication hierarchy: separate Publications, year, conference, journal, and workshop group headings have been removed. Venue and year remain within each paper record.
- Publication geometry: desktop rows use the reference's 30% media / 70% copy split with centered figures and compact 20 px cell padding.
- Typography and palette: narrow 820 px canvas, Palatino-style academic body copy, restrained sans-serif headings, dark neutral text, and muted blue links match the reference's visual language.
- Image fidelity: eight publication rows use the user's canonical figures from `paper_figs/`. The final transaction paper uses an authentic first-page preview rather than a fabricated figure.
- Profile treatment: `profile-2.png` is shown in a bordered 3:4 frame with padding and a centered full-body crop.
- Section-heading treatment: small Font Awesome motifs identify Research, Internship Experience, Education, and Honors and Awards. They respond subtly on hover without competing with the page title.
- Responsive behavior: the 500 px layout preserves the two-column paper rhythm without horizontal overflow; narrower screens stack each figure above its citation.

## Findings

- No actionable P0/P1/P2 findings remain.
- Expected content deviation: News is intentionally omitted, so Research begins higher than on the reference homepage.
- Expected asset deviation: the final transaction paper has no canonical figure, so its real first page is used as a distinct paper-preview thumbnail.
- Accessibility check: the section-heading motifs are decorative and hidden from assistive technology; reduced-motion preferences collapse their transitions to a near-instant frame.

## Comparison history

1. Initial site version grouped papers under Publications and year headings and placed venue metadata in a text-only left column.
   - Finding: P1 — the organization read like a project/publication index rather than the requested academic-homepage pattern.
   - Fix: replaced the section with the reference's Research heading, inline Scholar link, research paragraph, and direct paper sequence.
2. First image pass used raw paper-page crops.
   - Finding: P2 — full-page density made the publication thumbnails visually weak at the 30% media width.
   - Fix: selected and tightly cropped representative workflows, architecture diagrams, screenshots, plots, and tables from the source papers.
3. Desktop comparison showed the implementation and reference now share the same narrow canvas, intro composition, research-heading treatment, and 30/70 paper rows.
   - Result: passed at the normalized 1440 × 2400 viewport.
4. Responsive capture at 500 px showed readable titles, aligned thumbnails, and no horizontal overflow.
   - Result: passed.
5. The title/profile refinement was compared with al-folio's restrained icon language and Yuzhe's more personal visual motifs.
   - Finding: large illustration or typing effects would overpower the compact academic layout.
   - Fix: retained the existing hierarchy, switched to `profile-2`, and added only three small domain-specific icon chips with one-time entrance and hover micro-interactions.
   - Result: passed on desktop and at 500 px.
6. User clarification moved visual motifs away from the personal name and onto module headings.
   - Fix: removed the three name-adjacent icons and assigned one semantic icon to each major section heading.
   - Paper assets: replaced eight generated/cropped thumbnails with the user's canonical figures in `paper_figs/`; the final transaction paper intentionally has no figure and retains the aligned citation column.
   - Result: passed in the normalized desktop comparison and the 500 px responsive capture.
7. Follow-up inspection revealed that `.research-heading span` reduced both the Scholar link and the containing Research label.
   - Fix: narrowed the selector to `.research-heading__scholar`, restoring the module title to the standard h2 size.
   - Final paper treatment: replaced the awkward empty media column with a bordered first-page preview generated from the paper's authentic public PDF.
   - Result: passed in the normalized desktop comparison and the 500 px responsive capture.
8. The first section navigation used a centered, bold row of links with root-relative fragment URLs.
   - Finding: P1 — it read like a generic directory bar and same-section repeat clicks did not reliably retrigger scrolling.
   - Fix: matched the reference's restrained academic navigation language with a left-aligned name, right-aligned sans-serif links, a thin rule, and a compact native mobile menu. Fragment-only URLs and an explicit click handler now retrigger `scrollIntoView` on every click.
   - Result: passed in the normalized desktop comparison, the 500 px responsive capture, and a two-click Microsoft Edge interaction test.

## Interaction and implementation checks

- Email, GitHub, Google Scholar, all nine paper-title links, all nine thumbnail links, and all nine `[paper]` links are present.
- External links use `target="_blank"` with `rel="noopener noreferrer"`.
- Every publication image has meaningful alternative text and fixed intrinsic dimensions.
- The current rendered page references `/images/profile-2.png`; all four section-heading icons resolve through the bundled Font Awesome set.
- Desktop navigation exposes all six section links; the mobile layout replaces horizontal overflow with a native disclosure menu.
- An automated Microsoft Edge interaction check clicked the Research link twice and observed two calls to the page's scroll handler with the correct `#research` URL state.
- Jekyll production build completed successfully.
- Rendered HTML contains no News, Lab Homepage, Services, Friends, Main Collaborators, Code, PDF, Research Experience, Publications, or year-group headings.

## Implementation checklist

- [x] Match the reference Research heading and inline Scholar link.
- [x] Place research interests directly below the heading.
- [x] Remove publication-type and year grouping.
- [x] Use the supplied canonical figure for each of the first eight paper rows.
- [x] Use an authentic first-page preview when the final paper has no canonical figure.
- [x] Link titles, available thumbnails, and `[paper]` labels to canonical paper pages.
- [x] Compare reference and implementation at the same viewport.
- [x] Verify the active responsive layout.

final result: passed
