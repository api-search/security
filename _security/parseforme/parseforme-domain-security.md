---
api_specs:
- filename: openapi.json
  format: json
  label: ParseForMe API
  slug: parseforme-api
  spec_type: OpenAPI
  url: https://api.parseforme.com/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parseforme.com
  spf: true
hosts:
- cert_expires: Oct 12 09:29:29 2026 GMT
  host: parseforme.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 09:29:29 2026 GMT
  host: api.parseforme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Parseforme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParseForMe, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ParseForMe
provider_slug: parseforme
slug: parseforme-domain-security
source_filename: parseforme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parseforme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 09:29:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.parseforme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 09:29:29 2026 GMT\n  hsts: null\ndomains:\n- domain: parseforme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parseforme/refs/heads/main/security/parseforme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Parsing
- OCR
- Data Extraction
- Document AI
- IDP
- Invoices
- Bank Statements
- Receipts
- Resumes
- PDF
- Webhooks
- REST
---
