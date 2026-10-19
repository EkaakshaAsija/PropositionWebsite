# The Ballot Project — static website prototype

A single-page educational guide to five selected California ballot measures. The visual direction uses a restrained public-information style: editorial serif headings, neutral sans-serif body text, clear section labels, minimal card decoration, and a muted navy / slate / white palette.

## Run it

1. Extract the ZIP.
2. Open `index.html` in a modern browser. No build tools, account, database, framework, or sign-in are needed.
3. Internet access is needed for YouTube embeds and official source links. If an embedded player is blocked by a browser preview, firewall, or content-security policy, use the visible “Watch on YouTube” link below that player.

## Interaction behavior

- A sticky sidebar highlights the current measure while the reader scrolls.
- Clicking a proposition takes the reader to the matching section on the same page; no measure opens in another page.
- Navigation calculates offsets from the actual sticky header and the mobile proposition bar. It also handles direct links such as `index.html#prop-39` and correctly marks the final section when the document bottom is reached.
- On narrow screens, the sidebar becomes a horizontally scrollable selector; the active measure is scrolled into view.
- The five sections each contain an official California Secretary of State quick-reference video, plus a visible direct YouTube link as an embed fallback.
- Numbered disclosure rows use native HTML `<details>` / `<summary>` controls. In the collapsed state, each row shows only its number, heading, and centered plus icon. The entire header is clickable and keyboard operable.
- Reduced-motion preferences are respected, visible focus outlines are provided, and the page includes a skip link and print styling.

## Content and sources

The measures and summaries are based on the California Secretary of State's November 3, 2026 Official Voter Information Guide. The guide is the authoritative source for complete text, impartial fiscal analysis, and the submitted arguments for and against each measure:

- [Proposition 3](https://voterguide.sos.ca.gov/propositions/3/)
- [Proposition 4](https://voterguide.sos.ca.gov/propositions/4/)
- [Proposition 38](https://voterguide.sos.ca.gov/propositions/38/)
- [Proposition 39](https://voterguide.sos.ca.gov/propositions/39/)
- [Proposition 43](https://voterguide.sos.ca.gov/propositions/43/)
- [Official ASL quick-reference video list](https://voterguide.sos.ca.gov/asl/)

The embedded videos are the state Secretary of State's official ASL quick-reference videos, with audio and on-screen guide text. They are included as external YouTube embeds, not copied or hosted locally.

## Design research

The redesign follows general patterns described in these public-sector design references:

- [California State Web Template V6](https://template.webstandards.ca.gov/) — consistency, responsive structure, updated typography, and enhanced navigation.
- [California State Web Standards: Design and UX](https://webstandards.ca.gov/web-policies/design-and-ux/) — clear content paths and the maintained state web template/UI kit.
- [U.S. Web Design System: Side navigation](https://designsystem.digital.gov/components/side-navigation/) — short labels and a clearly indicated current section.
- [U.S. Web Design System: In-page navigation](https://designsystem.digital.gov/components/in-page-navigation/) — smooth jumps and active-section state for long pages.
- [U.S. Web Design System: Accordion](https://designsystem.digital.gov/components/accordions/) — clear, clickable headers and keyboard accessibility.
- [W3C WCAG 2.2 focus visibility](https://www.w3.org/WAI/WCAG22/Understanding/focus-visible/) — visible keyboard focus.

These are design references, not a formal accessibility certification. Test the final hosted implementation with the agency's accessibility and security review process before publication.

## Before publication

This is a front-end concept, not an official State of California website. Have the appropriate agency review content, source citations, accessibility, branding, privacy, video behavior, and hosting/security policies before public release. Confirm all summaries against the live voter guide immediately before publication.
