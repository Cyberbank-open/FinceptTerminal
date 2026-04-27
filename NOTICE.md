# NOTICE

This product, **Ganglia Terminal**, is a derivative work of the open-source project
**FinceptTerminal** by **Fincept Corporation**, distributed here under the terms of
the GNU Affero General Public License, version 3 (AGPL-3.0).

## Upstream Source

- Project: FinceptTerminal
- Copyright holder: Fincept Corporation
- Upstream repository: https://github.com/Fincept-Corporation/FinceptTerminal
- License: AGPL-3.0-or-later (see `LICENSE`)
- Trademark policy: https://github.com/Fincept-Corporation/FinceptTerminal/blob/main/docs/TRADEMARK.md

## What Ganglia Network Has Modified

This fork (operated by Ganglia Network) introduces, on top of the upstream:

1. A new theme preset (`THEME_GANGLIA`) defined in
   `fincept-qt/src/ui/theme/ThemeManager.cpp` and declared in `ThemeTokens.h`,
   using the official Ganglia Network color palette and typography from
   *Ganglia Network Brand Book v1.0*.
2. Switched the default active theme from `THEME_OBSIDIAN` to `THEME_GANGLIA`.
3. Replaced user-visible brand strings (window title, application name, splash
   text, About screen, info screens, EXE VERSIONINFO) from "Fincept Terminal"
   to "Ganglia Terminal", from "Fincept Corporation" to "Ganglia Network".
4. Replaced the application icon (`fincept.ico`, `fincept_icon.ico`) with the
   Ganglia lobster mascot in multi-resolution Windows ICO format. The new
   source SVG is preserved at
   `fincept-qt/resources/ganglia_app_icon.svg`.
5. Updated About-screen trademark attribution to clarify dual-source ownership:
   - "Ganglia", "Ganglia Network", "Ganglia Terminal" — trademarks of
     Ganglia Network.
   - "Fincept", "Fincept Terminal", and the original Fincept logo — remain
     trademarks of Fincept Corporation, used under AGPL-3.0 source-code
     license, **not** under any Fincept trademark license.
6. Updated this README, this NOTICE, and the upstream attribution chain.

The upstream `LICENSE` file remains unchanged and is the authoritative license
text for this fork as well.

## Trademark Status

| Mark | Owner | This fork's use |
|---|---|---|
| "Fincept", "Fincept Terminal", original Fincept logo | Fincept Corporation | Source-code attribution only; not a trademark license. This fork does NOT claim trademark rights to these marks. |
| "Ganglia", "Ganglia Network", "Ganglia Terminal", lobster mascot, $GANG / $AXON marks | Ganglia Network | Trademarks of Ganglia Network. |

## Network-Service Distribution Reminder (AGPL §13)

If you, as an operator of a derivative of Ganglia Terminal, make this software
available to users over a network (including SaaS, member-only platforms,
trading clubs, and similar), you are required by AGPL-3.0 §13 to offer those
users the complete corresponding source code — **including all modifications
you make on top of this fork** — under AGPL-3.0 or a later version. Failure
to do so is a license violation. If you wish to distribute a closed-source
product based on FinceptTerminal, you must obtain a commercial license from
Fincept Corporation directly: `support@fincept.in`.

## Contact

- Ganglia Network: support@ganglia.network
- Fincept Corporation (upstream): support@fincept.in

---

© 2025 Fincept Corporation. © 2026 Ganglia Network. AGPL-3.0-or-later.
