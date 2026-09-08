# Corresponding source

This is a customized Herdr Mobile Relay 0.20.9 frontend (assets 363).

Upstream: https://github.com/0cv/herdr-mobile-relay
Base commit: c6e24cc3f627ecc791db39d77b177a754c46501e
License: AGPL-3.0 (see LICENSE)

To reproduce: clone upstream, check out the base commit, apply customization.patch
from this site repository using git apply, then run in frontend/ with Bun 1.4.0:

    bun install --frozen-lockfile
    bun run build

The patch preserves conversation-first navigation, read-only pane subscriptions
without resizing the desktop terminal, adaptive history polling, and mobile
terminal Backspace/layout customization. No relay credentials are included.

0.20.x requires updated relays and freshly paired devices; old 0.19.x credentials
and transport are incompatible.
