# Security Policy

## Scope

This repository hosts the **public, high-level documentation and landing page** for Cognitum
MetaHarness-as-a-Service. It is a **static site** — plain HTML and CSS, with **no JavaScript, no
analytics, no trackers, no external CDNs, no cookies, and no application code**. The product's API,
source code, configuration, and credentials are **private and auth-gated** and are not part of this
repository.

## Reporting a vulnerability

If you believe you have found a vulnerability, an exposed secret, or any over-exposure in this
public site, please report it privately:

- **Email:** security@cognitum.one
- Please include the URL/path, a description, and (if relevant) reproduction steps.
- Please do **not** open a public issue for suspected secret exposure.

We aim to acknowledge reports promptly and will coordinate disclosure responsibly.

## What this site deliberately does NOT contain

- No API keys, tokens, HMAC/signing secrets, or secret-manager secret names.
- No internal service-account identities, project identifiers, or private hostnames beyond the
  already-public, auth-gated API endpoint name.
- No private API integration details, request/response payloads, or internal URLs.

The site is intentionally a high-level overview. The private code and private API stay private.

## Hardening applied to the published site

- Strict Content-Security-Policy meta tag (`default-src 'self'`, `script-src 'none'`, no inline or
  remote scripts; styles served from a self-hosted stylesheet only).
- `referrer: no-referrer` and `X-Content-Type-Options: nosniff` meta directives.
- HTTPS-only (enforced by GitHub Pages) with `upgrade-insecure-requests`.
- No cookies, no client-side fetches, no third-party origins of any kind.
- A machine-readable `/.well-known/security.txt` (RFC 9116).
