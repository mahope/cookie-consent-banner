# Cookie Consent Banner

**Lightweight, GDPR-compliant cookie consent banner** — drop in one `<script>` tag, zero dependencies, no tracking, no build step. ~2.5 KB minified.

[![License](https://img.shields.io/badge/license-MIT-lightgrey)](LICENSE)
[![Size](https://img.shields.io/badge/size-2.5%20KB-blue)](banner.js)
[![Compliance](https://img.shields.io/badge/GDPR-ready-green)](https://hermes-passiv.pages.dev/books/cookie-consent-guide)

## Demo

→ [**Live demo on hermes-passiv.pages.dev**](https://hermes-passiv.pages.dev/cookie-consent-banner-demo)

## Quick start

```html
<script src="https://hermes-passiv.pages.dev/downloads/cookie-consent-banner.js"
        data-site-name="My Website"></script>
```

That's it. The banner shows once, sets a consent cookie, and hides for 365 days.

## Customisation

All options are `data-` attributes on the `<script>` tag.

| Attribute | Default | Description |
|-----------|---------|-------------|
| `data-site-name` | `"This website"` | Your site name |
| `data-position` | `"bottom"` | `"bottom"` or `"top"` |
| `data-accept-text` | `"Accept All"` | Button label |
| `data-necessary-text` | (none) | Show a "Necessary Only" button |
| `data-policy-url` | (none) | Link to your privacy policy |
| `data-cookie-name` | `"cc_consent"` | Consent cookie name |
| `data-storage-days` | `365` | How long consent lasts |

### Examples

**With privacy policy link and both buttons:**
```html
<script src="https://hermes-passiv.pages.dev/downloads/cookie-consent-banner.js"
        data-site-name="My Shop"
        data-policy-url="/privacy"
        data-necessary-text="Necessary Only"
        data-accept-text="Accept All"></script>
```

**Top-positioned banner with only accept:**
```html
<script src="https://hermes-passiv.pages.dev/downloads/cookie-consent-banner.js"
        data-site-name="Blog"
        data-position="top"></script>
```

## Features

- **Zero dependencies** — no jQuery, no external CSS, no CDN calls
- **No tracking** — the script never makes network requests; consent is stored in a cookie
- **GDPR-compliant** — sets a cookie with `SameSite=Lax`, respects user choice
- **Customisable** — position, labels, links, cookie name and duration
- **Accessible** — ARIA role `dialog` with `aria-label`
- **Portable** — works on any site: static HTML, WordPress, Shopify, Next.js, plain PHP

## GDPR / ePrivacy context

The EU ePrivacy Directive requires websites to obtain consent before storing non-essential cookies. This banner is a lightweight way to meet that requirement for compliance-conscious site owners.

For a deeper guide on cookie consent, EU compliance requirements, and how to audit your site, download the free e-book: [**Cookie Consent & GDPR Compliance for Web Agencies**](https://hermes-passiv.pages.dev/books/cookie-consent-guide).

## Related tools

- [**Compliance Site Check**](https://github.com/mahope/compliance-site-check) — GitHub Action that checks any site for privacy policy, terms, cookie banner, imprint, DPA, security headers, meta tags and hreflang
- [**EUcomply Scanner**](https://github.com/mahope/eucomply-scanner) — CLI scanner for website compliance (GDPR, DSA, ePrivacy, security headers)
- [**Free E-Books**](https://hermes-passiv.pages.dev/books) — NIS2, GDPR, EAA, and cookie consent guides in EPUB format

## License

MIT — use it anywhere, free and unrestricted.
