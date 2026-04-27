# Ganglia Terminal

<div align="center">

**Own Your AI. Own Your Future.**

A native financial intelligence terminal for the Ganglia Network ecosystem.
Built for traders who deploy lobsters, not workers.

[![License: AGPL-3.0](https://img.shields.io/badge/license-AGPL--3.0-B22222)](LICENSE)
[![C++20](https://img.shields.io/badge/C%2B%2B-20-00599C?logo=cplusplus)](https://isocpp.org/)
[![Qt6](https://img.shields.io/badge/Qt-6-2E75B6?logo=qt&logoColor=white)](https://www.qt.io/)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Brand](https://img.shields.io/badge/Ganglia-Network-1B2A4A)](https://ganglia.netlify.app/)

</div>

---

## Attribution & Provenance

**Ganglia Terminal is a derivative work of [FinceptTerminal](https://github.com/Fincept-Corporation/FinceptTerminal)** by Fincept Corporation, used under the GNU Affero General Public License v3.0. We thank the FinceptTerminal team for the foundational native-Qt architecture, theme system, and analytics modules that made this brand customization possible.

- Upstream repository: <https://github.com/Fincept-Corporation/FinceptTerminal>
- Upstream license: AGPL-3.0 (preserved in `LICENSE`)
- Upstream commercial-licensing inquiries: `support@fincept.in`
- Per AGPL §7, this fork preserves all original copyright notices, the LICENSE file, and the upstream source-code availability obligation. See `NOTICE.md` for the full attribution chain.

This product is **not endorsed by, sponsored by, or affiliated with Fincept Corporation**. "Fincept" and "Fincept Terminal" remain trademarks of Fincept Corporation; the `LegalCopyright` field in the Windows EXE properties names both copyright holders explicitly.

---

## What Ganglia Terminal Is

A desktop financial terminal customized for the Ganglia Network community — Lobster Owners who deploy AI agents to monitor markets 7×24, executing strategies on-chain. Where the upstream is a generic financial intelligence platform, Ganglia Terminal layers in:

- **Ganglia brand identity** — Deep Navy / Lobster Red / Neural Blue palette per the official Brand Book v1.0.
- **Lobster-themed UX language** — *Deploy a lobster*, *evolve your G-tier*, *the Colony*, *$GANG / $AXON* token semantics throughout the interface.
- **Native performance retained** — C++20 + Qt6, single binary, no Electron / web overhead. Same engine, different skin and voice.

## Brand Identity

| Element | Value |
|---|---|
| Tagline (primary) | *Own Your AI. Own Your Future.* |
| Tagline (community) | *Deploy Your Lobster.* |
| Mascot | The Ganglia lobster (G1 → G10 Nexus evolution) |
| Tokens | `$GANG` (value, scarcity) · `$AXON` (signal, connection) |

### Color System

| Token | Hex | Role |
|---|---|---|
| Ganglia Red | `#B22222` | Brand, $GANG, primary CTA |
| Neural Blue | `#2E75B6` | Network, $AXON, info, focus |
| Deep Navy | `#1B2A4A` | Background, authority — **never use pure black** |
| Signal Gold | `#D4A843` | VIP, achievements, important data |
| Data Green | `#5DCAA5` | Positive returns, gain, up signal |
| Pulse White | `#F0F4F8` | Body text, data panels |
| Burn Red | `#E24B4A` | Loss, down, $GANG burn events |
| Alert Amber | `#EF9F27` | Warnings, whale alerts |

### Typography

- **Display / brand name:** Inter (Bold), letter-spacing +10% on `GANGLIA NETWORK` (always uppercase)
- **Body:** Inter (Regular / Medium)
- **Data / code:** JetBrains Mono — terminal-wide default

### Voice & Tone

Ganglia speaks in three layers — *manifesto* for big launches, *product* for in-app copy, *community* for social. We are direct, confident, technically deep but jargon-free. We say *Lobster Owner* not *user*, *Colony* not *platform*, *$GANG burned* not *transaction fee*. See the Brand Book for the full forbidden-words list.

## Architecture (inherited from upstream)

```
fincept-qt/                  Native Qt6 / C++20 desktop app
├── src/app/                 Main window, screen router, entry point
├── src/ui/theme/            Theme tokens, ThemeManager, QSS generators
│   ├── ThemeTokens.h        Pure data struct of design tokens
│   ├── ThemeManager.cpp     THEME_GANGLIA + THEME_OBSIDIAN definitions
│   └── StyleSheets.cpp      QSS interpolators
├── src/ui/components/       Reusable widgets
├── src/ui/navigation/       Toolbar, F-key bar, command bar, status bar
├── src/screens/             70+ feature screens (markets, news, ai_chat, …)
├── src/services/            Data feeds, notifications, updater
├── src/python/              Embedded Python runtime + analytics scripts
└── resources/               Icons, splash, app.rc.in (Windows VERSIONINFO)
```

To switch palettes at runtime, call `ThemeManager::instance().apply_theme("Obsidian")` to drop into the upstream Fincept palette, or omit the argument / pass any other name to use Ganglia (default).

## Building

Same build matrix as upstream — see [`fincept-qt/CMakeLists.txt`](fincept-qt/CMakeLists.txt) and [`docs/`](docs/) for full instructions. Quick path on Windows:

```powershell
cd fincept-qt
cmake --preset msvc-release
cmake --build --preset msvc-release
```

## License

This project is licensed under **AGPL-3.0-or-later**, inherited from upstream. The full text is in [`LICENSE`](LICENSE). Per AGPL §13, **if you operate Ganglia Terminal as a network service for paying members, you must offer them the complete corresponding source code** — including all modifications you make to this fork. Plan accordingly.

For commercial-license inquiries about the upstream FinceptTerminal codebase or Fincept Data APIs, contact `support@fincept.in` directly.

For Ganglia Network business inquiries (community licensing of the lobster mascot, brand partnerships, the $GANG / $AXON token ecosystem), contact `support@ganglia.network`.

---

<div align="center">

**Own Your AI. Own Your Future.**
🦞 Deploy Your Lobster.

</div>
