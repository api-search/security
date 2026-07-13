---
api_specs:
- filename: 01-ai-openapi.yml
  format: yaml
  label: Lingyiwanwu Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/01-ai/refs/heads/main/openapi/01-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 01.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lingyiwanwu.com
  spf: false
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.01.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: platform.lingyiwanwu.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.lingyiwanwu.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: 01 Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 01.AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 01.AI
provider_slug: 01-ai
slug: 01-ai-domain-security
source_filename: 01-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.01.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: platform.lingyiwanwu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: api.lingyiwanwu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 01.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: lingyiwanwu.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/01-ai/refs/heads/main/security/01-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- LLM
- Yi
- Open Source
- Foundation Models
- Inference
---
