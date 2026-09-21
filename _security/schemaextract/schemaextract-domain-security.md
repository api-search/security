---
api_specs:
- filename: schemaextract-openapi.yml
  format: yaml
  label: SchemaExtract API
  slug: schemaextract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schemaextract/refs/heads/main/openapi/schemaextract-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: schemaextract.shop
  spf: false
hosts:
- cert_expires: Dec 18 04:16:29 2026 GMT
  host: schemaextract.shop
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Schemaextract Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SchemaExtract, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SchemaExtract
provider_slug: schemaextract
slug: schemaextract-domain-security
source_filename: schemaextract-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: schemaextract.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 04:16:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: schemaextract.shop\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schemaextract/refs/heads/main/security/schemaextract-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Document AI
- IDP
- Data Extraction
- PDF/OCR-to-JSON
- Invoice & AP automation
- Logistics/freight
- Fintech
- Developer API
---
