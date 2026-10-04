# Decisions and open questions

## Confirmed directions

| Topic | Current direction |
| --- | --- |
| Initial occasions | Weddings and birthday parties |
| Product name and chosen domain | EventCard; `eventcard.cc` (registration, ownership, and deployment unverified) |
| Creation approach | Styled templates with personalization |
| Core flow | Choose → personalize → preview → share |
| Outputs | Hosted webpage link and downloadable image |
| Account and payment timing | Create and preview without signing up; after finishing, prompt sign up/sign in and payment before sharing |
| Paid owner editing | No edit-count limit; can switch templates while preserving entered event details |
| Updates | Edits update the webpage at the same link; downloaded images remain static and must be regenerated after edits |
| Language ambition | 30+ languages for both app interface and invitations; exact list and launch rollout open |
| Freeform canvas | Set aside for now due to development cost |
| Delivery approach | Start with core flow; allow later extension |
| Repository layout | Public `octocl/event-card-planning` with docs under `docs/`; public backend and frontend repositories linked as submodules |
| Human-readable hub and assets | Private [Notion product hub](https://app.notion.com/p/3efa63cd5f7d811c95e7fc779bd06e7d) and its [Assets page](https://app.notion.com/p/3efa63cd5f7d81d98c26e0185b51d1eb) in `counter-arena`; no assets uploaded yet |
| Current phase | Interactive planning wayfinder to resolve open questions; design and implementation later |

## Open questions

- Who is the first target audience, and in which geography or geographies?
- Which fields can users edit for each occasion? Are photos, venue, maps, and custom text needed at launch?
- Should the image mirror the webpage design, be a separate card, or offer both options? Which formats and dimensions matter?
- Which languages launch first, and how should localized templates be handled?
- Which sign-up/sign-in methods, save behavior, autosave rules, and publish timing are needed?
- What are the payment packages and entitlements, including whether one payment unlocks both webpage and image? Pricing discussion is deferred.
- What visual identity should EventCard use?
- What technology stack fits the agreed scope? Should a mobile app or other service be added later?

The planning, backend, and frontend repository names and public visibility are chosen. Stitch may be considered during the later design phase if requested.

Record answers here with dates and update the relevant topic document. Do not treat proposals or competitor observations as approved decisions.
