# Changelog 📝

All notable changes to the **Pitch Black Modern** extension will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.4] - 2026-06-20

### Changed

- **Syntax Palette Overhaul:** Completely rebalanced the syntax colors to prioritize readability on the `#000000` OLED canvas.
- **Color Assignments:**
  - **Keywords & Control:** Updated to `#C678DD` (Purple/Magenta) for high-impact logic visualization.
  - **Strings:** Set to `#CE9178` (Soft Orange) for distinct differentiation from standard text.
  - **Functions & Components:** Locked to `#38BDF8` (Sky Blue) to highlight execution blocks.
  - **Operators & Punctuation:** Grouped under `#94A3B8` (Slate) to minimize visual noise.
  - **Variables:** Set to `#E2E8F0` (Off-White) to maintain natural text flow.
- **UI Consistency:** Forced all background elements (Sidebars, Terminal, Tabs, Status Bar) to an absolute `#000000` to ensure zero light bleed.

### Fixed

- **Token Leakage:** Refined `tokenColors` scope definitions to prevent interference from default VS Code syntax rules.
- **UI Contrast:** Adjusted `editorLineNumber.activeForeground` to `#94A3B8` for better visibility without distraction.

---

## [1.0.3] - 2026-06-20

### Changed

- **String Refinement:** Shifted string colors to a soothing Mint Green (`#86EFAC`) to balance perfectly with the high-contrast syntax.
- **Operator & Punctuation Split:** Separated structural punctuation from logical operators for better visual code flow.
  - **Operators:** Now pop in vibrant Cyber-Pink (`#FF79C6`) to make logic (`=`, `=>`, `&&`) stand out.
  - **Punctuation:** Commas, periods, and semicolons now use a subtle Slate Gray (`#64748B`) to reduce visual clutter against the black canvas.

### Fixed

- **Settings Restoration:** Ensured `"semanticHighlighting": false` and dynamic bracket colorization were properly packaged in the final build payload.

---

## [1.0.2] - 2026-06-20

### Added

- **Dynamic Bracket Pairs:** Integrated VS Code's native bracket pair colorization. Brackets now dynamically cycle through Yellow (`#FBBF24`), Pink (`#FF79C6`), Turquoise (`#4EC9B0`), Purple (`#BD93F9`), and Green (`#A6E22E`) for perfect nested readability.

### Changed

- **Syntax Revert & Overhaul:** Scrapped the One Dark Pro syntax engine. Reverted to a custom, highly vibrant neon and pastel color palette that pops beautifully against the `#000000` canvas.
- **Semantic Highlighting:** Disabled (`"semanticHighlighting": false`) to ensure custom TextMate rules take full priority without interference.
- **Color Palette Updates:**
  - **Strings:** Completely removed muddy oranges and reds, replacing them with a clean Soft Pastel Yellow (`#F1FA8C`).
  - **Comments:** Shifted to a bright Neon Green (`#A6E22E`).
  - **Keywords & Control Flow:** Updated to a punchy Cyber-Pink (`#FF79C6`).
  - **Classes & Types:** Highlighted in Turquoise (`#4EC9B0`).
  - **Object Keys:** Popping in Mint Green (`#4ADE80`).
  - **Variables & Modifiers:** Crisp Light Blue (`#38BDF8`).

---

## [1.0.1] - 2026-06-19

### Added

- **Semantic Highlighting:** Fully integrated `"semanticHighlighting": true` along with comprehensive semantic token colors for advanced, context-aware syntax highlighting in modern languages like TypeScript, Rust, Dart, and Python.
- **Marketplace Links:** Added homepage, repository, and issue-tracking URLs to the package configuration for better community support.

### Changed

- **Syntax Overhaul:** Completely replaced the custom syntax color palette with the legendary **One Dark Pro** ruleset. The theme now perfectly balances industry-standard code legibility with the existing zero-distraction `#000000` canvas.

### Improved

- **Marketplace Presence:** Optimized extension keywords and metadata for the VS Code Marketplace algorithm, explicitly highlighting OLED support and the One Dark syntax engine.

---

## [1.0.0] - 2026-06-17

### Changed

- **Tag Colors:** Updated HTML, XML, and JSX tags from vibrant coral to a classic, readable Dark Blue (`#569CD6`).
- **Attribute Colors:** Shifted HTML and JSX attributes from amber to a crisp Light Cyan (`#9CDCFE`), maintaining italics for clear structural hierarchy.
- **String Literals:** Updated strings (including attribute values) to a warm Orange/Brown (`#CE9178`) for complementary contrast against the new structural blues.

### Improved

- **Visual Comfort:** Overhauled the core web-development palette to reduce visual fatigue, establishing a cleaner, high-contrast aesthetic that remains vibrant without being harsh against the pitch-black background.

---

## [0.1.1] - 2026-06-13

### Added

- **Expanded Syntax Highlighting:** Added deep colorization for HTML, XML, and JSX files.
- **Component Styling:** Tags now feature a vibrant coral (`#F87171`) to easily distinguish structure.
- **Attribute Styling:** HTML and JSX attributes are now formatted with an italicized amber (`#FCD34D`).
- **CSS Support:** Distinct sky blue highlighting added for CSS/SCSS properties.

### Improved

- Broadened language support to provide a highly legible experience across modern web development stacks.

---

## [0.1.0] - Initial Release

### Added

- True pitch-black (`#000000`) UI elements for zero-distraction coding.
- High-contrast syntax highlighting for standard text, keywords, functions, strings, and numbers.
- Seamless blending of the editor, terminal, sidebars, and tab bars.
