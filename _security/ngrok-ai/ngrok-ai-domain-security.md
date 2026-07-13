---
api_specs:
- filename: ngrok-ai-openapi.yml
  format: yaml
  label: ngrok AI Gateway
  slug: ai-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ngrok-ai/refs/heads/main/openapi/ngrok-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ngrok.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ngrok.app
  spf: false
hosts:
- cert_expires: Sep 30 16:16:57 2026 GMT
  host: ngrok.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 16:35:46 2026 GMT
  host: your-ai-gateway.ngrok.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ngrok Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ngrok AI Gateway, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ngrok AI Gateway
provider_slug: ngrok-ai
slug: ngrok-ai-domain-security
source_filename: ngrok-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ngrok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:16:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-ai-gateway.ngrok.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 16:35:46 2026 GMT\n  hsts: null\ndomains:\n- domain: ngrok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ngrok.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ngrok-ai/refs/heads/main/security/ngrok-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- AI Gateway
- API Gateway
- LLM
- OpenAI Compatible
- Routing
- Security
- Traffic Management
---
