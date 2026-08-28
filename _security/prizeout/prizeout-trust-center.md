---
certifications: []
description: ''
kind: trust-center
layout: security
name: Prizeout Trust Center
name_suffix: Trust Center
overview: Prizeout maintains a public trust center covering its security and compliance posture.
provider_name: Prizeout
provider_slug: prizeout
slug: prizeout-trust-center
source_filename: prizeout-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.prizeout.com/\nname: Prizeout Trust Center\npresent: true\nurl: https://trust.prizeout.com/\nplatform: Vanta\nhttp_status: 200\nprobed: '2026-08-26'\nevidence:\n  canonical: https://trust.prizeout.com\n  title: Prizeout Trust Center\n  description: >-\n    \"The Prizeout application and related components provides users the ability to buy and use gift\n    cards purchased with funds held on our partners' platforms. The Prizeout application also\n    includes certain related rewards, cashback and shopping products, according to partner needs.\"\n  platform_markers:\n  - 'assets.vanta.com static bundles (index-trust-report-*.js)'\n  - 'og:image https://app.vanta.com/doc?s=fntlllx5b649e9zh8ppl8'\ncertifications: []\ncertifications_readable: false\ncertifications_note: >-\n  The trust center is a client-rendered Vanta single-page app. The HTML served to a non-JS client\n  contains the page title, canonical URL and description\
  \ and nothing else - no framework list, no\n  control list, no subprocessors, no document requests. Certifications therefore could NOT be read.\n  This is recorded as unreadable rather than absent: Prizeout may well publish SOC 2 or similar\n  behind the bundle, but no machine can see it, and no certification name is asserted here.\ndocuments_gated: unknown\nsubprocessors: unknown\ngaps:\n- 'Trust-center contents are invisible to any non-browser client, including the crawlers and agents\n  that increasingly do vendor pre-screening. A static fallback or a machine-readable summary would\n  make the certifications legible.'\n- 'No /.well-known/security.txt points at the trust center (probed 404 on all hosts).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prizeout/refs/heads/main/security/prizeout-trust-center.yml
summary_line: trust center published
tags:
- Company
- Advertising
- Rewards
- Gift Cards
- Payouts
- Financial Services
- Credit Unions
- Banking
- Loyalty
- Embedded Finance
- AdTech
- FinTech
trust_url: https://trust.prizeout.com/
---
