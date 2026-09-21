---
api_specs:
- filename: solvela-ai-openapi.json
  format: json
  label: Solvela Gateway API
  slug: solvela-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solvela-ai/refs/heads/main/openapi/solvela-ai-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: solvela.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fly.dev
  note: Platform domain of the OpenAPI servers[1] host, not a Solvela domain; its DNS posture is Fly.io's.
  spf: false
hosts:
- cert_expires: Nov 13 07:55:42 2026 GMT
  host: solvela.ai
  hsts: true
  hsts_header: max-age=63072000
  hsts_max_age: 63072000
  https: true
  note: 'hsts was recorded null by probe-domain-security.py; strict-transport-security: max-age=63072000 was observed on the 402 DEPLOYMENT_DISABLED response from Vercel on 2026-09-19 (curl -i), so the value is corrected from direct observation.'
  tls_version: TLSv1.3
- cert_expires: Nov 14 11:59:46 2026 GMT
  host: api.solvela.ai
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains
  hsts_max_age: 31536000
  https: true
  note: 'hsts was recorded null by probe-domain-security.py; strict-transport-security: max-age=31536000; includeSubDomains was observed on every response from the gateway on 2026-09-19 (curl -i), so the value is corrected from direct observation.'
  tls_version: TLSv1.3
- cert_expires: Nov 19 11:49:32 2026 GMT
  host: solvela-gateway.fly.dev
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains
  hsts_max_age: 31536000
  https: true
  note: 'hsts was recorded null by probe-domain-security.py; strict-transport-security: max-age=31536000; includeSubDomains was same gateway; observed on the agent-card response on 2026-09-19 (curl -i), so the value is corrected from direct observation.'
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Solvela Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solvela, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Solvela
provider_slug: solvela-ai
slug: solvela-ai-domain-security
source_filename: solvela-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solvela.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 07:55:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_header: max-age=63072000\n  note: 'hsts was recorded null by probe-domain-security.py; strict-transport-security: max-age=63072000 was observed on the\n    402 DEPLOYMENT_DISABLED response from Vercel on 2026-09-19 (curl -i), so the value is corrected from direct observation.'\n- host: api.solvela.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 11:59:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_header: max-age=31536000; includeSubDomains\n  note: 'hsts was recorded null by probe-domain-security.py; strict-transport-security: max-age=31536000; includeSubDomains\n    was observed on every response from the gateway on 2026-09-19 (curl -i), so the value is corrected from direct observation.'\n\
  - host: solvela-gateway.fly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 11:49:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_header: max-age=31536000; includeSubDomains\n  note: 'hsts was recorded null by probe-domain-security.py; strict-transport-security: max-age=31536000; includeSubDomains\n    was same gateway; observed on the agent-card response on 2026-09-19 (curl -i), so the value is corrected from direct observation.'\ndomains:\n- domain: solvela.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: fly.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: Platform domain of the OpenAPI servers[1] host, not a Solvela domain; its DNS posture is Fly.io's.\nnote: api.solvela.ai answers with content-security-policy default-src none, x-content-type-options nosniff, x-frame-options\n  DENY and referrer-policy no-referrer on every response (observed 2026-09-19). solvela.ai MX is Cloudflare Email Routing;\n  SPF v=spf1\
  \ include:_spf.mx.cloudflare.net ~all; no DMARC record; no CAA; DNSSEC not enabled.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solvela-ai/refs/heads/main/security/solvela-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Payments
- Artificial Intelligence
- LLM Gateway
- x402
- Solana
- Stablecoins
- AI Agents
- MCP
- A2A
- Agentic Commerce
---
