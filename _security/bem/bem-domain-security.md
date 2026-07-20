---
api_specs:
- filename: bem-openapi-original.yml
  format: yaml
  label: Bem API v3
  slug: bem-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bem/refs/heads/main/openapi/bem-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bem.ai
  spf: true
hosts:
- cert_expires: Aug 28 11:20:28 2026 GMT
  host: api.bem.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 18:24:53 2026 GMT
  host: api.eu1.bem.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bem, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bem
provider_slug: bem
slug: bem-domain-security
source_filename: bem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.bem.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:20:28 2026 GMT\n  hsts: null\n- host: api.eu1.bem.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 18:24:53 2026 GMT\n  hsts: null\ndomains:\n- domain: bem.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bem/refs/heads/main/security/bem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Document Processing
- Unstructured Data
- Data Extraction
- Artificial Intelligence
- LLM
- ETL
- Schema Inference
- Webhooks
---
