# Privacy Policy for LinkedIn Message Manager

Last updated: 17 June 2026

> Canonical copy also at [linkedin-extension-config/privacy/linkedin-message-manager.md](https://github.com/abaddion/linkedin-extension-config/blob/main/privacy/linkedin-message-manager.md)

## Introduction

LinkedIn Message Manager is a browser extension that helps users manage LinkedIn messages with AI-assisted summaries and replies. We are committed to protecting your privacy.

## Data collection and use

Our extension:

- Does **not** collect personal information on our servers
- Does **not** store message content on our servers
- Does **not** track user behavior for advertising
- Does **not** sell or share data with third parties

Optional **local diagnostics** (off by default): if you enable “Store local diagnostic events” in Options, the extension saves URL path, selector strategy index, and element counts in Chrome local storage on your device only. No message text is logged.

## API key

- You provide your own **Anthropic API key**
- The key is stored in Chrome sync/local storage on your device
- Requests go from your browser directly to Anthropic’s API
- We do not have access to your API key

## Message processing

- Thread text is read from the LinkedIn page in your browser to generate summaries and drafts
- That text is sent to **Anthropic** only when you trigger summary or reply generation, using your key
- Nothing is sent to our servers
- Generated text is shown in the sidebar; sending to LinkedIn only happens when you click **Send**

## Third-party services

The extension may contact:

- **Anthropic API** (your key, when you generate text)
- **Google Fonts** / Adobe Fonts (UI styling in Options)
- **raw.githubusercontent.com** (remote selector config for reliability when LinkedIn updates its site)

## Data storage

Chrome storage is used for:

- API key and sign-off name
- UI preferences (e.g. sidebar hidden)
- Cached remote selector config
- Optional local diagnostic log (opt-in)

## Changes

We may update this policy. Changes will be posted at this URL.

## Contact

Questions: **barbora@recberry.com**
