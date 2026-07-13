---
api_specs:
- filename: zenrows-universal-scraper-openapi.yml
  format: yaml
  label: ZenRows Universal Scraper API
  slug: universal-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/openapi/zenrows-universal-scraper-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zenrows.com
  spf: true
hosts:
- cert_expires: Aug 25 09:28:51 2026 GMT
  host: www.zenrows.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:04:21 2026 GMT
  host: docs.zenrows.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.zenrows.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zenrows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZenRows, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ZenRows
provider_slug: zenrows
slug: zenrows-domain-security
source_filename: zenrows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zenrows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:28:51 2026 GMT\n  hsts: null\n- host: docs.zenrows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:04:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.zenrows.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zenrows.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/security/zenrows-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web Scraping
- Data Extraction
- Anti-Bot
- Proxies
- Residential Proxies
- Browser Automation
- Screenshots
- CAPTCHA
- AI
- MCP
- Spain
---
