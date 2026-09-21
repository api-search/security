---
api_specs:
- filename: claix-dev-openapi.yml
  format: yaml
  label: Claix Document Intelligence API
  slug: claix-document-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claix-dev/refs/heads/main/openapi/claix-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: claix.dev
  spf: false
hosts:
- cert_expires: Nov  1 17:46:52 2026 GMT
  host: www.claix.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 17:46:50 2026 GMT
  host: claix.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Claix Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Claix
provider_slug: claix-dev
slug: claix-dev-domain-security
source_filename: claix-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.claix.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 17:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: claix.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 17:46:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: claix.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claix-dev/refs/heads/main/security/claix-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Document Processing
- Data Extraction
- Document Intelligence
- PDF
- Excel
- OCR
- Structured Data
- AI Agents
- MCP
- A2A
- Spain
- Company
---
