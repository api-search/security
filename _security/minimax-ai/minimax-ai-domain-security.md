---
api_specs:
- filename: minimax-ai-openapi.json
  format: json
  label: MiniMax Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/openapi/minimax-ai-openapi.json
description: ''
domains:
- caa:
  - alb-5wxesx27onoewtiobw.us-east-1.alb.aliyuncsslbintl.com.
  dmarc: false
  dnssec: true
  domain: minimax.io
  spf: true
hosts:
- cert_expires: Sep  6 08:21:43 2026 GMT
  host: www.minimax.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: platform.minimax.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.minimax.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Minimax Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MiniMax, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: MiniMax
provider_slug: minimax-ai
slug: minimax-ai-domain-security
source_filename: minimax-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.minimax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:21:43 2026 GMT\n  hsts: false\n- host: platform.minimax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.minimax.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: minimax.io\n  dnssec: true\n  caa:\n  - alb-5wxesx27onoewtiobw.us-east-1.alb.aliyuncsslbintl.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minimax-ai/refs/heads/main/security/minimax-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- AI
- LLM
- Inference
- Multimodal
- Voice
- Video
- Music
- Image
---
