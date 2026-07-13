---
api_specs:
- filename: scrapingant-openapi.yml
  format: yaml
  label: ScrapingAnt
  slug: scrapingant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/openapi/scrapingant-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scrapingant.com
  spf: true
hosts:
- cert_expires: Sep  2 00:11:25 2026 GMT
  host: scrapingant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 08:39:52 2026 GMT
  host: api.scrapingant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrapingant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScrapingAnt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ScrapingAnt
provider_slug: scrapingant
slug: scrapingant-domain-security
source_filename: scrapingant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scrapingant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:11:25 2026 GMT\n  hsts: false\n- host: api.scrapingant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:39:52 2026 GMT\n  hsts: null\ndomains:\n- domain: scrapingant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/security/scrapingant-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Extraction
- Proxies
- Scraping
---
