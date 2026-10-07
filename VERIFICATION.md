# Verification

Public profile facts and project evidence were checked on **7 October 2026**. Local package and browser checks were completed on **8 October 2026**.

| Check | Result |
| --- | --- |
| Five standalone SVGs | Valid XML, declared SVG namespaces, unique panel-prefixed IDs, and resolved local references. No scripts, `foreignObject`, event handlers or external asset URLs. |
| Embedded assets | Both WOFF2 fonts in every panel match the supplied font files exactly. Hero and ID portraits match `assets/id.png`; the connect character matches `assets/right_pointing.png`. |
| Animation structure | Finite CSS entrances use `animation-fill-mode: both` and retain visible, settled base styles. SMIL starts at `0s`; supplied `keyTimes` values are valid. |
| Timed browser inspection | All five final panels inspected at 0, 2, 5, 9 and 13 seconds. Both embedded fonts loaded in every panel. Audits found no visible text outside panel bounds and no external asset requests. Entrance content is intentionally concealed at the initial animation frame, then appears. |
| Image embedding | The settled panels were visually inspected when displayed using HTML `img` elements. |
| Static fallback | Versions with animation disabled were visually inspected and remained readable. |
| Reduced motion | A forced equivalent of the reduced-motion media rules was visually inspected and remained readable. This checks the reduced-motion presentation, not every operating system's preference integration. |
| Portrait transparency | Both PNGs were visually checked against light and dark backgrounds; their transparent backgrounds were preserved. |
| Mobile width | All five settled panels were inspected at a 375-pixel browser width, with no horizontal overflow, clipped content or overlapping text. Small annotations scale with the artwork; the README also supplies native text and links. |
| README references | Exactly five panel images use relative `./assets/…svg?v=1` paths in the intended order. Contact and project destinations are ordinary Markdown links. |

Contact/project URL check on 8 October 2026: the three featured repositories, GitHub profile, Instagram profile and Arisetek returned HTTP 200. Arisetek required one retry after a hosting cold start. LinkedIn returned HTTP 999, an automated-request restriction; its exact public-profile URL is preserved.

## Live publication verified — 8 October 2026

The public repository [anaita1999/anaita1999](https://github.com/anaita1999/anaita1999) uses `main` as its default branch. The complete package was published in commit `cea75e2981861a55457f2920241b73894fa4b7eb`; all 27 remote file hashes matched the local package before this verification-note update.

The public [GitHub profile](https://github.com/anaita1999) returned HTTP 200. Its rendered README HTML contains exactly the five intended panel images and all seven project/contact links. Each GitHub-rewritten image URL returned HTTP 200 with `image/svg+xml`, and its response bytes matched the locally tested SVG exactly.

**Scope:** local desktop/mobile browser rendering and live GitHub delivery were checked separately. A final visual inspection inside the live GitHub page was unavailable because browser controls were unavailable at publication time. HTTP and byte checks confirm delivery of the tested files; they do not prove identical rendering or animation in every browser. Contact identities and project destinations are grounded in [SOURCES.md](./SOURCES.md).
