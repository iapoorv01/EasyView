# Changelog

All notable changes to EasyView will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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
