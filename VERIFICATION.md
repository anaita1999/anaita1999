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

**Pending:** live GitHub profile verification. Local browser checks do not establish that the files have been published or prove identical rendering in every browser or GitHub image-serving configuration. Contact identities and project destinations are grounded in the public sources listed in [SOURCES.md](./SOURCES.md).
