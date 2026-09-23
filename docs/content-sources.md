# Content sources

Prepared on September 24, 2026. This file is excluded from the generated website.

- The user-provided `CV (5).pdf` is the initial source for the biography, education, industry experience, teaching, honors, and professional email addresses. Subsequent direct user edits take precedence. Its bytes are preserved in `assets/files/minho-jeong-cv.pdf`.
- [GitHub profile](https://github.com/Chessjeong): name, portrait, location, GitHub and LinkedIn profiles, and the pinned Causilo project.
- [Google Scholar](https://scholar.google.com/citations?user=d0IeCM4AAAAJ): the user supplied the profile URL. Automated access failed; no citation counts or extra publications were inferred from it.
- [View Space on arXiv](https://arxiv.org/abs/2512.11561): canonical title, full author names, paper URL, and ICML 2026 acceptance. Also corroborated by [the official repository](https://github.com/dooho00/graph-view-space) and [Jaemin Yoo's homepage](https://jaeminyoo.github.io/).
- [Causilo Technical Report on arXiv](https://arxiv.org/abs/2609.22866): title, author order, September 19, 2026 date, preprint status, and concise research summary.
- [Causilo repository](https://github.com/nums-ai/causilo): project description and code/model links.

Editorial decisions:

- Following the website review, lead the biography with the research focus and show selected publications and projects before the compact education/experience/teaching/honors grid. Keep one all-publications link in the home section. The Causilo project describes usage and displays the already-confirmed “Co-creator” role; no unverified individual technical contributions or benchmark claims were added.
- Use the CV's more specific “Integrated M.S.–Ph.D.” degree description rather than the shorter “M.S. Student” on GitHub.
- The user requested removal of manuscripts under review and the Research Experience section from the website, and removal of the detailed Teaching description.
- The user supplied the revised biography and the Nums AI description, shortened to “Co-creator of Causilo,” and requested removal of the SK hynix work description. The incomplete trailing phrase “, and a.” in the supplied biography was treated as a typo and omitted.
- All five Causilo authors are marked with equal-contribution asterisks at the user's request. The redundant PDF link was removed; the Paper link leads to arXiv.
- At the user's request, remove biography and project topic tags and append the “Previously” sentence to the research paragraph. Use lowercase “founding research scientist” only in the About Me biography; use “Founding Research Scientist” in the profile, experience, and metadata. The Causilo project subtitle is “Tabular Foundation Model”; its description emphasizes frontier-level predictive performance and fast inference, as described in the technical report.
- The 2026-01-01 date in the View Space record is a sorting key for its conference year, not an asserted publication day. The rendered website displays only 2026.
- Show the CV's graduation GPA, “GPA: 3.72/4.3,” before “Cum Laude” in the KAIST education entry at the user's request. Programming-language lists remain in the CV.
- Keep the SK hynix scholarship description as an offer, not a received scholarship.
- Deployment targets the user-provided existing repository `Chessjeong/Chessjeong.github.io`, as explicitly requested after the local preview review. The initial repository commit is preserved.

Template: [luost26/academic-homepage](https://github.com/luost26/academic-homepage), upstream commit `7bd10b6`. Original MIT license and footer attribution retained.
