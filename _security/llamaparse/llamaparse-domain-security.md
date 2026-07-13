---
api_specs:
- filename: llamaparse-llamacloud-openapi.yml
  format: yaml
  label: LlamaParse Parse API
  slug: llamaparse-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llamaparse/refs/heads/main/openapi/llamaparse-llamacloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: llamaindex.ai
  spf: true
hosts:
- cert_expires: Oct  3 16:27:10 2026 GMT
  host: www.llamaindex.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 06:16:36 2026 GMT
  host: developers.llamaindex.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: api.cloud.llamaindex.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Llamaparse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LlamaParse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LlamaParse
provider_slug: llamaparse
slug: llamaparse-domain-security
source_filename: llamaparse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.llamaindex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.llamaindex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:16:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cloud.llamaindex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: llamaindex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llamaparse/refs/heads/main/security/llamaparse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Parsing
- OCR
- PDF
- LLM
- RAG
- AI
- Document Intelligence
- Structured Data Extraction
---
