---
api_specs:
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Web Scraper API
  slug: oxylabs-web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Residential Public API
  slug: oxylabs-residential-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
- filename: oxylabs-openapi.yml
  format: yaml
  label: Oxylabs Dashboard API
  slug: oxylabs-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/openapi/oxylabs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oxylabs.io
  spf: true
hosts:
- cert_expires: Sep  7 12:46:06 2026 GMT
  host: oxylabs.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:15:15 2026 GMT
  host: developers.oxylabs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 15:21:00 2026 GMT
  host: realtime.oxylabs.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oxylabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oxylabs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oxylabs
provider_slug: oxylabs
slug: oxylabs-domain-security
source_filename: oxylabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oxylabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:46:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.oxylabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:15:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: realtime.oxylabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 15:21:00 2026 GMT\n  hsts: null\ndomains:\n- domain: oxylabs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxylabs/refs/heads/main/security/oxylabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Web Scraping
- Bot Mitigation Bypass
- CAPTCHA Solving
- Data Extraction
- Datacenter Proxies
- Datasets
- E-Commerce Data
- Headless Browser
- ISP Proxies
- Mobile Proxies
- Proxies
- Residential Proxies
- SERP
- Scraper API
- Scraping
- Web Data
- Web Intelligence
- Web Unblocker
---
