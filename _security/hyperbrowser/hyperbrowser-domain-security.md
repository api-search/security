---
api_specs:
- filename: hyperbrowser-sessions-api-openapi.yml
  format: yaml
  label: Hyperbrowser Sessions API
  slug: sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-sessions-api-openapi.yml
- filename: hyperbrowser-profiles-api-openapi.yml
  format: yaml
  label: Hyperbrowser Profiles API
  slug: profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-profiles-api-openapi.yml
- filename: hyperbrowser-scrape-api-openapi.yml
  format: yaml
  label: Hyperbrowser Scrape API
  slug: scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-scrape-api-openapi.yml
- filename: hyperbrowser-crawl-api-openapi.yml
  format: yaml
  label: Hyperbrowser Crawl API
  slug: crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-crawl-api-openapi.yml
- filename: hyperbrowser-extract-api-openapi.yml
  format: yaml
  label: Hyperbrowser Extract API
  slug: extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-extract-api-openapi.yml
- filename: hyperbrowser-agents-api-openapi.yml
  format: yaml
  label: Hyperbrowser Agents API
  slug: agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-agents-api-openapi.yml
- filename: hyperbrowser-extensions-api-openapi.yml
  format: yaml
  label: Hyperbrowser Extensions API
  slug: extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-extensions-api-openapi.yml
- filename: hyperbrowser-web-api-openapi.yml
  format: yaml
  label: Hyperbrowser Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyperbrowser.ai
  spf: false
hosts:
- cert_expires: Sep  6 00:28:59 2026 GMT
  host: hyperbrowser.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 19:10:28 2026 GMT
  host: docs.hyperbrowser.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 21:43:57 2026 GMT
  host: api.hyperbrowser.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperbrowser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperbrowser, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Hyperbrowser
provider_slug: hyperbrowser
slug: hyperbrowser-domain-security
source_filename: hyperbrowser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyperbrowser.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:28:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hyperbrowser.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:10:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hyperbrowser.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:43:57 2026 GMT\n  hsts: null\ndomains:\n- domain: hyperbrowser.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/security/hyperbrowser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Headless Browser
- Browser Infrastructure
- Web Scraping
- Web Crawling
- Data Extraction
- AI Agents
- Browser Automation
- Computer Use
- Stealth
- Proxies
- CAPTCHA Solving
- MCP
- HyperAgent
- X402
---
