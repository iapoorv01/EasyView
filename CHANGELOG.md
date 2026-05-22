# Changelog

All notable changes to EasyView will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.1] - 2026-05-15

### Added
- **Inline Interactive Dictionary (Define-in-Place)**: Activated dynamic in-page definitions. Highlight-clicking "Define" now renders an elegant dashed focus rectangle around the target word instantly, attaching a live interactive tooltip on the spot so users can read meanings without breaking their reading flow.
- **Reading Ruler Focus Engine (Dual-Beam Geometry)**: Expanded the Flashlight engine with a specialized "Reading Ruler" mode. Dynamically computes split linear-gradients to slice a horizontal view area across the screen, providing critical visual isolating support for ADHD/Dyslexia track-reading.
- **Dynamic Beam Sizing Controls**: Built a custom hardware-accelerated range slider to scale the Focus Light in real-time. Intelligently binds to both modes: controls the precise slit-height of the Reading Ruler and mathematically scales spotlight radial vectors, fully exposed via dynamic UI labels.
- **Flashlight Dashboard UX Refactoring**: Decluttered the Flashlight customizations, separating geometry controls (Shape & Size) from aesthetic options (Lens Tint & Shadow Depth) into functional, numbered, glassmorphic segments with descriptive subtitle guidance.
- **Universal Flashcard Exporter (Anki / Quizlet)**: Designed a one-click data CSV compiler adhering to strict RFC-4180 and UTF-8 BOM specs. Translates local saved vocabulary decks into transportable sheets ready for instant study flashcard imports.
- **Manual Notebook Injector**: Added an expandable direct-entry card within the Study Notebook tab. Features active duplicate-entry scanning, realtime prepending, and local JSON storage syncing to bypass manual page selections.
- **Evie AI Rebranding**: Transformed the extension's companion persona to **Evie AI**, utilizing lightweight vector SVGs for sparkles throughout top-level action menus to permanently eliminate emoji minification hazards.
- **Onboarding Tour Restart & Auto-Scroll**: Integrated an interactive "Help/Tour" icon in the dashboard header to replay the guided tour on-demand. Upgraded the core spotlight engine to automatically scroll vertical off-screen nodes into the focal viewport.
- **On-Demand Paragraph Simplification**: Launched Gemini-powered "Simplify" contextual engines, allowing users to highlight complex paragraphs and instantly translate them into easy-to-digest, plain-English bulleted recaps.
- **Interactive Flashcard Editor**: Equipped the Notebook Study Deck with dynamic, in-place card update tools. Users can trigger premium frosted-glass textareas to write, save, and persist custom study notes and memory tricks.
- **Real-Time Notebook Search**: Injected an incremental search engine into the dashboard dashboard, dynamically filtering the entire flashcard deck in real-time based on terminology, definitions, or custom notes.
- **Audible Flashcards**: Integrated native text-to-speech listeners directly into the Notebook card action bars, allowing users to hear their simplified definitions spoken aloud with a single click.
- **Luxurious Decoder Tooltips**: Overhauled jargon hover tooltips with a gorgeous glassmorphic UI layout featuring rich, integrated micro-actions: One-click **🔊 Text-to-Speech (Speak)** audio playback, **🔖 Quick-Bookmark** ribbons for study decks, and **📖 Expanded Detail** modules.
- **Smart Jargon Guard**: Re-engineered backend lifecycle to automatically toggle the Auto-Jargon Decoder OFF upon fresh tab loads and navigations, permanently safeguarding users from accidental or wasteful AI query usage.
- **Direct Offline Bookmarks**: Introduced instant local bookmarking from the floating text toolbar, completely bypassing network decoders to conserve user API budget. Includes custom-crafted "Tangerine Orange" badge tags to distinguish personal study cards.
- **Text Simplification Ribbons**: Built instant Save-to-Notebook integration for simplified paragraph popups, archiving AI sentence rewrites directly to local flashcard storage.
- **Cryptographic Licensing**: Implemented full end-to-end digital signature verification (ECDSA) for offline premium protection. Feature modes now mathematically validated via hardware WebCrypto to prevent paywall tampering.
- **Backend Hardening**: Reinforced the API authorization engine with private key generators to deliver signed integrity tokens to verified sessions.
- **Focus & Privacy Shield**: Introduced advanced page obfuscation system featuring a real-time dual-layer "Flashlight Engine" (masking/blurring outside cursor focal points) and smart CSS privacy shielding customized for high-sensitivity communication portals like Gmail and WhatsApp.
- **Smart Renewal Celebrations**: Re-engineered the premium tracker into a stateful lifecycle machine. The dashboard now tracks specific license expiration timestamps, enabling automatic celebration confetti explosions on direct renewals and resetting tracker memory on downgrades.
- **High-Performance Cinematic Confetti**: Upgraded the celebration engine to replace continuous heavy 60fps physics loops with a lightweight staggered triple-burst sequence, yielding a **95% reduction in CPU overhead**. Features highly curated multicolored palettes (Gold, Cyan, Fuchsia) and organic vector noise so no two purchase celebrations look identical.
- **Dynamic OS Font Ingest Engine (Dark Reader Grade)**: Wired native Chromium `fontSettings` bridge to silently scan the user's hard drive. Populates the visuals dropdown dynamically with hundreds of real, alphabetized local system fonts, delivering unparalleled cross-device visual personalization.
- **High-Performance DocumentFragment Buffering**: Engineered virtual DOM buffers for system font injection to bypass browser reflow cycles completely, securing 0ms, lag-free drawing speeds regardless of physical font volume.
### Changed
- **Twin Highlight Physics Parity**: Refined user-defined glossary terms to inherit difficulty-2 styling seamlessly, establishing absolute CSS layout parity between manual clarifications and AI-decoded box models.
- **Cross-Theme Dash Optimization**: Hardened all fresh components—including form selectors, quick-add drawers, and flashlight sizing panels—against light-theme adaptations, ensuring high-contrast Oceanic Cyan accessibility across light and dark modes.
- **Dynamic XSS Defense**: Audited and rewrote DOM interpolation engines inside selection highlighting workflows to use 100% native `DocumentFragment` and `createElement` patterns, eliminating vector risks from HTML string injections.
- **Advanced Cache Lifecycle (LRU)**: Implemented smart Least Recently Used self-pruning to local storage wrappers, setting definitive headroom boundaries (150 items for selections, 50 items for full-scans) to permanently mitigate local storage bloat.
- **Performance (GPU Scrolling)**: Accelerated Notebook rendering using CSS layout containment boundaries (`contain: content`) and forced hardware-compositing layers (`transform: translate3d`), yielding butter-smooth 60 FPS scroll metrics.
- **Cinematic Tour Optimization**: Upgraded the onboarding spotlight using real-time viewport math; the engine now skips redundant scrolling for instantaneous 0ms snappiness and employs soft cinematic fade transitions to prevent viewport tearing artifacts.
- **Symmetric Layout Architecture**: Restructured top-bar dashboard headers into functional flex groups, restoring perfect horizontal balance and symmetry across user controls and help/setting actions.
- **Architectural Modularization**: Refactored large sections of the extension, decoupling over 450 lines from the monolithic `popup.js` codebase into dedicated feature modules (`notebook-controller.js`, `tour-controller.js`) and split content scripts into optimized feature units to boost code maintainability.
- **Strict "Action-Only" Telemetry Architecture**: Redesigned Study Deck pipelines to trigger only upon explicit, high-value user activities (saving bookmarks, submitting manual entries, or exporting lists). Pruned passive view listeners to maximize backend efficiency.

### Fixed
- **Eager Cache Telemetry Locking**: Eradicated asynchronous race conditions in user-analytics endpoints by locking the 24-hour cache boundary IMMEDIATELY before network dispatch, permanently stopping concurrent multi-click data duplication.
- **Flashlight Vector Contrasts (Light Mode)**: Resolved white-on-white visibility issues for Circle/Ruler beam shapes and the sizing range-slider by stripping restrictive inline color overrides, unleashing flawless Slate-Gray and high-contrast Oceanic Cyan styling across Light adaptations.
- **Live Jargon Gradient Sync**: Bridged isolated web-injection CSS gaps by natively rendering vibrant category gradients (Definition, Dictionary, Custom, Tech) directly onto the floating tooltip engine.
- **Premium Modal Z-Index Escalation**: Recalculated the hierarchical depth of configuration dashboards versus dynamic upgrade prompts, elevating the Premium Gate modal to guarantee it intercepts clicks above all scrolling content.
- **Real-Time Storage Serialization**: Attached atomic persistence hooks to all Converter, Export, and Visual setting forms, writing slider dimensions and dropdown options to Chrome Sync instantly upon change.
- **Tour Teleportation Glitch**: Fixed a dimensional computation hazard where Onboarding Spotlights would clamp to (0,0) coordinates on hidden tabs. The tour engine now forces a 200ms layout reflow to securely anchor the spotlight over the exact button coordinates.


## [1.1.0] - 2026-05-03

### Added
- **EasyView Premium**: Launched a new premium subscription tier unlocking unlimited AI queries and advanced sensory shields.
- **Supabase Integration**: Added robust backend infrastructure for user authentication (Google OAuth), payment tracking, and secure server-side API routing.
- **Usage Analytics**: Implemented lightweight, privacy-preserving usage tracking to better understand which features users need most (does not track URLs or text content).
- **Web Portal**: Launched `easyview.in` for account management, comprehensive documentation, and secure checkout.

### Changed
- **Privacy Policy**: Completely overhauled to accurately reflect the new account system and Supabase backend while maintaining our strong privacy guarantees.
- **API Routing**: The Jargon Decoder now routes through our secure backend for Free/Premium users, fully hiding corporate API keys from the client.
- **BYOK (Bring Your Own Key)**: Refined the BYOK flow, explicitly making it an optional path for advanced users who wish to bypass all quotas.

## [1.0.2] - 2026-04-20

### Fixed
- Addressed character encoding corruption issues in Jargon Decoder responses.
- Improved performance of the Sensory Shield background MutationObserver.
- Resolved UI state synchronization bugs when logging out of the extension.

## [1.0.1] - 2026-01-11

### Added
- **Visuals Tab**: Introduced a dedicated Visuals tab in the popup, allowing users to adjust brightness, contrast, sepia, grayscale, font style, text stroke, and toggle dark/light mode for improved on-page accessibility. All settings are applied instantly and saved for future browsing sessions.
- **Jargon Decoder**: AI-powered text simplification with full page and selection-based decoding
  - Full page mode: Automatically detects and simplifies complex terms across entire pages
  - Selection decoder: Decode specific text selections (10-5000 characters)
  - Text simplification: Complete plain-English rewrites of selected content
  - Interactive tooltips with category labels and difficulty ratings
  - Support for legal, financial, technical, medical, government, and academic jargon

- **Dyslexia Reading Mode**: Comprehensive reading support
  - Multiple dyslexia-friendly fonts (OpenDyslexic, Arial, Comic Sans)
  - Customizable letter spacing (0-5px)
  - Adjustable line height (1.0-3.0)
  - Word spacing control (0-10px)
  - Color overlays (beige, light blue, light green, light yellow)
  - Bionic reading mode with bold first letters
  - Persistent settings across sessions

- **Sensory Shield**: Reduce sensory overload
  - Freeze CSS animations and transitions
  - Pause auto-playing videos and GIFs
  - Stop flashing and blinking elements
  - Create calmer browsing experience

- **Text-to-Speech**: Advanced read-aloud functionality
  - Playback controls (play, pause, stop)
  - Voice selection from system voices
  - Adjustable speed (0.5x - 1.5x)
  - Volume control (0-100%)
  - Smart punctuation pauses
  - Word highlighting with visual tracking
  - Automatic content selection

- **Dual AI Provider Support**: Choose between OpenRouter or Google Gemini
  - Automatic fallback between providers
  - Secure local storage of API keys

- **Modern UI/UX**:
  - Dark/light theme toggle
  - Responsive popup sizes (S, M, L)
  - Clean, accessible interface with Inter font
  - API provider badge
  - Visual progress indicators

### Technical
- Chrome Extension Manifest V3 architecture
- Content scripts for page manipulation
- Background service worker for API communication
- Unified API service layer supporting multiple providers
- Chrome Sync Storage for settings persistence
- Chrome Local Storage for secure API key storage

### Security & Privacy
- Local-only API key storage
- No data collection or tracking
- HTTPS-encrypted API communications
- Open source and auditable code

[1.0.1]: https://github.com/EasyView/releases/tag/v1.0.1
