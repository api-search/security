---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: crawlee.dev
  spf: false
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: crawlee.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crawlee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crawlee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Crawlee
provider_slug: crawlee
slug: crawlee-domain-security
source_filename: crawlee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crawlee.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: crawlee.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawlee/refs/heads/main/security/crawlee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Apache 2.0
- Apify
- Browser Automation
- Crawlers
- Harvesting
- JavaScript
- Node.js
- Open Source
- Playwright
- Puppeteer
- Python
- Scraping
- Web
---
