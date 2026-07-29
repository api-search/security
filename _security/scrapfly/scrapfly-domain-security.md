---
api_specs:
- filename: scrapfly-scrape-openapi.yml
  format: yaml
  label: Scrapfly Scrape API
  slug: scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapfly/refs/heads/main/openapi/scrapfly-scrape-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scrapfly.io
  spf: true
hosts:
- cert_expires: Aug 18 23:38:41 2026 GMT
  host: scrapfly.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:38:41 2026 GMT
  host: api.scrapfly.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrapfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scrapfly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Scrapfly
provider_slug: scrapfly
slug: scrapfly-domain-security
source_filename: scrapfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scrapfly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:38:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.scrapfly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:38:41 2026 GMT\n  hsts: null\ndomains:\n- domain: scrapfly.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapfly/refs/heads/main/security/scrapfly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Data Extraction
- Screenshots
- Web Scraping
- Proxies
- Browser Automation
---
