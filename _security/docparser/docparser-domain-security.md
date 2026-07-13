---
api_specs:
- filename: docparser-rest-api-openapi.yml
  format: yaml
  label: Docparser REST API
  slug: docparser-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docparser/refs/heads/main/openapi/docparser-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: docparser.com
  spf: true
hosts:
- cert_expires: Sep 13 08:12:46 2026 GMT
  host: docparser.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.docparser.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docparser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docparser, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Docparser
provider_slug: docparser
slug: docparser-domain-security
source_filename: docparser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docparser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:12:46 2026 GMT\n  hsts: false\n- host: api.docparser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docparser.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docparser/refs/heads/main/security/docparser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Parsing
- Data Extraction
- PDF
- OCR
- Document Automation
- Invoices
- Contracts
- REST API
---
