---
api_specs:
- filename: doctly-ai-openapi.yml
  format: yaml
  label: Doctly Documents Parse API
  slug: doctly-documents-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doctly-ai/refs/heads/main/openapi/doctly-ai-openapi.yml
- filename: doctly-ai-openapi.yml
  format: yaml
  label: Doctly Extract API
  slug: doctly-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doctly-ai/refs/heads/main/openapi/doctly-ai-openapi.yml
- filename: doctly-ai-openapi.yml
  format: yaml
  label: Doctly Status and Results API
  slug: doctly-status-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doctly-ai/refs/heads/main/openapi/doctly-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doctly.ai
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: doctly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 11:50:50 2026 GMT
  host: docs.doctly.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: api.doctly.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Doctly Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doctly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Doctly
provider_slug: doctly-ai
slug: doctly-ai-domain-security
source_filename: doctly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doctly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\n- host: docs.doctly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 11:50:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.doctly.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: doctly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctly-ai/refs/heads/main/security/doctly-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Document Parsing
- PDF
- Markdown
- Data Extraction
- OCR
---
