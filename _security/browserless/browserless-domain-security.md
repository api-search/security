---
api_specs:
- filename: browserless-openapi.yml
  format: yaml
  label: Browserless Cloud API
  slug: browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserless/refs/heads/main/openapi/browserless-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: browserless.io
  spf: true
hosts:
- cert_expires: Aug 27 16:44:03 2026 GMT
  host: www.browserless.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 04:23:42 2026 GMT
  host: docs.browserless.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 10:42:13 2026 GMT
  host: production-sfo.browserless.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Browserless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Browserless, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Browserless
provider_slug: browserless
slug: browserless-domain-security
source_filename: browserless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.browserless.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:44:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.browserless.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:23:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: production-sfo.browserless.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 10:42:13 2026 GMT\n  hsts: null\ndomains:\n- domain: browserless.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browserless/refs/heads/main/security/browserless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Headless Browser
- Browser Infrastructure
- Web Automation
- AI Agents
- Web Scraping
- BrowserQL
- Puppeteer
- Playwright
- Selenium
- CDP
- Stealth
- CAPTCHA Solving
- Residential Proxy
- PDF Generation
- Screenshots
- Smart Scrape
- Crawl
- Search
- MCP
- Session Recording
- Hybrid Automation
---
