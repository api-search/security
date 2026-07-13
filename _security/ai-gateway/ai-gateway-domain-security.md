---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: portkey.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openrouter.ai
  spf: true
hosts:
- cert_expires: Oct  6 08:44:14 2026 GMT
  host: portkey.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:14:05 2026 GMT
  host: api.portkey.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:49:33 2026 GMT
  host: openrouter.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ai Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Gateway, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AI Gateway
provider_slug: ai-gateway
slug: ai-gateway-domain-security
source_filename: ai-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portkey.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:44:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.portkey.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:14:05 2026 GMT\n  hsts: null\n- host: openrouter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:49:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: portkey.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: openrouter.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-gateway/refs/heads/main/security/ai-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Gateway
- LLM Router
- LLM Proxy
- Model Routing
- Prompt Firewall
- Guardrails
- AI Observability
- Cost Controls
- AI Governance
- API Gateway
---
