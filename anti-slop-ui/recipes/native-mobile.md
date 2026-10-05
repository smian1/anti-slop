# Recipe: Native mobile

iOS, Android, React Native / Expo, SwiftUI screens. Web tells still apply (purple gradient, emoji icons, glass soup, oversized radius). These are the ones that only show up on a phone.

## Defaults

- **Edit** default: minimum visual change; keep navigation structure and real data.
- Platform chrome first: system tab bar, navigation stack and header back, sheets, platform icon set (SF Symbols / Material), semantic system colors, Dynamic Type / font scaling. Taste lives inside the system chrome, not in a rebuilt copy of it.
- Name the screen's job before styling it.

## Cuts that matter most here

| Tell | Fix |
|------|-----|
| **Web chrome on a phone**: hamburger + logo + links row, hand-rolled tab bar or modal, a "< Back" text link duplicating the header back | Native navigator, tab bar, and sheet; one header owner per screen |
| **Landing page as an app screen**: hero headline, three equal feature cards, CTA; giant centered title on every screen | Top-aligned content for the task; large titles stay leading-aligned navigation, not a hero. Paywall is the one promotional screen |
| **"Welcome back, Name! 👋" over a stat triplet**: greeting header plus three equal stat cards with invented numbers | Content first; greeting only when personalization is real; real numbers or labelled empty states |
| **Card-stack screen**: grey background, every row or setting its own white rounded shadowed card; shadows on several cards per screen | Grouped lists with hairline separators; elevation only for the one element that actually floats |
| **Decorative blur in the content layer**: frosted cards and list rows "for premium feel" | Material only on chrome over moving content (nav, tab bar, sheets), and only where the OS target supports it; never faked on older targets |
| **Fixed-pixel layout and safe-area hacks**: `width: 350`, `paddingTop: 50`, an implicit 375pt design, content under the home indicator or nav bar | Flex / size classes and safe-area insets; check the smallest phone and the largest text size |
| **Web-default font bundled on native**: Inter / Poppins / Space Grotesk shipped with no design decision behind it | System font with text styles, or the brand font DESIGN.md names; do not crown a replacement |

## Don't

- Restyle the platform's own controls into a web look-alike
- Invent users, streaks, or KPIs for preview data; use plausible, labelled placeholders
- Strip a deliberate brand system back to stock iOS; the filter removes defaults, not identity
