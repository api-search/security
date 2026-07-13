---
api_specs:
- filename: zenscrape-openapi.yml
  format: yaml
  label: Zenscrape Scrape API
  slug: zenscrape-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/openapi/zenscrape-openapi.yml
- filename: zenscrape-openapi.yml
  format: yaml
  label: Zenscrape Account API
  slug: zenscrape-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/openapi/zenscrape-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zenscrape.com
  spf: true
hosts:
- cert_expires: Aug 29 18:28:29 2026 GMT
  host: zenscrape.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 18:28:29 2026 GMT
  host: app.zenscrape.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenscrape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenscrape, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zenscrape
provider_slug: zenscrape
slug: zenscrape-domain-security
source_filename: zenscrape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenscrape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:28:29 2026 GMT\n  hsts: false\n- host: app.zenscrape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:28:29 2026 GMT\n  hsts: false\ndomains:\n- domain: zenscrape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenscrape/refs/heads/main/security/zenscrape-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web Scraping
- Proxy
- HTML
- Data Extraction
- JavaScript Rendering
---
