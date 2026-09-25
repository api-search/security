---
api_specs:
- filename: lastdatabase-openapi.yml
  format: yaml
  label: LastDatabase Lead Search API
  slug: lead-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lastdatabase/refs/heads/main/openapi/lastdatabase-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lastdatabase.com
  spf: true
hosts:
- cert_expires: Nov 30 08:19:01 2026 GMT
  host: lastdatabase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lastdatabase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LastDatabase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LastDatabase
provider_slug: lastdatabase
slug: lastdatabase-domain-security
source_filename: lastdatabase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lastdatabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 08:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lastdatabase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lastdatabase/refs/heads/main/security/lastdatabase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contact Data
- Lead Generation
- B2B Data
- Email Verification
- Data Enrichment
- Sales Prospecting
- MCP
---
