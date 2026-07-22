---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: walletstudio.com
  mx: google (smtp.google.com)
  spf: false
hosts:
- cert_not_after: '2026-10-04'
  host: www.walletstudio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: cloudflare (Webflow)
  tls_version: TLSv1.3
- host: walletstudio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: cloudflare (Webflow)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wallet Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wallet Studio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Wallet Studio
provider_slug: wallet-studio
slug: wallet-studio-domain-security
source_filename: wallet-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dns + tls probe of walletstudio.com (Website)\nhosts:\n  - host: www.walletstudio.com\n    https: true\n    tls_version: TLSv1.3\n    cert_not_after: '2026-10-04'\n    hsts: true\n    hsts_max_age: 31536000\n    server: cloudflare (Webflow)\n  - host: walletstudio.com\n    https: true\n    tls_version: TLSv1.3\n    hsts: true\n    hsts_max_age: 31536000\n    server: cloudflare (Webflow)\ndomains:\n  - domain: walletstudio.com\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    mx: google (smtp.google.com)\nnotes: >-\n  Website is hosted on Webflow behind Cloudflare with TLS 1.3 and a one-year\n  HSTS max-age. Email runs on Google Workspace. No CAA record, no SPF TXT\n  record (only google-site-verification and ACME challenge TXT present), no\n  DMARC record, and the zone is not DNSSEC-signed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallet-studio/refs/heads/main/security/wallet-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Digital Wallet
- Apple Wallet
- Google Wallet
- Passes
- Insurance
- Insurtech
- SaaS
- No-Code
- Fintech
- REST API
- Webhooks
- Customer Engagement
- GDPR
---
