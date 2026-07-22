---
api_specs:
- filename: nace-ai-ndi-openapi.json
  format: json
  label: Nace Document Intelligence (NDI)
  slug: nace-document-intelligence-ndi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nace-ai/refs/heads/main/openapi/nace-ai-ndi-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nace.ai
  spf: true
hosts:
- cert_expires: Oct 17 17:59:08 2026 GMT
  host: nace.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:11:47 2026 GMT
  host: docs.ndi.nace.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: ndi-api.nace.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nace Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nace Ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nace Ai
provider_slug: nace-ai
slug: nace-ai-domain-security
source_filename: nace-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 17:59:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.ndi.nace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:11:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ndi-api.nace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nace.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nace-ai/refs/heads/main/security/nace-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Document Intelligence
- Document Processing
- Data Extraction
- OCR
- Machine Learning
- Enterprise Automation
- MCP
---
