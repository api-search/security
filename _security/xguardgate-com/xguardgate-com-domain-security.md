---
api_specs:
- filename: xguardgate-com-openapi.json
  format: json
  label: XGuard Universal Paid AI Agent + Secretless Gateway API
  slug: xguard-universal-paid-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xguardgate-com/refs/heads/main/openapi/xguardgate-com-openapi.json
- filename: xguardgate-com-reconcile-openapi.json
  format: json
  label: XGuard Reconcile API
  slug: xguard-reconcile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xguardgate-com/refs/heads/main/openapi/xguardgate-com-reconcile-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xguardgate.com
  spf: false
hosts:
- cert_expires: Nov 23 16:36:25 2026 GMT
  host: xguardgate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 10:21:23 2026 GMT
  host: api.xguardgate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 23 16:36:25 2026 GMT
  host: reconcile.xguardgate.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Xguardgate Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XGuard, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: XGuard
provider_slug: xguardgate-com
slug: xguardgate-com-domain-security
source_filename: xguardgate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xguardgate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 16:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.xguardgate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 10:21:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: reconcile.xguardgate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 16:36:25 2026 GMT\n  hsts: false\ndomains:\n- domain: xguardgate.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xguardgate-com/refs/heads/main/security/xguardgate-com-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Agents
- Agentic Commerce
- x402
- MCP
- A2A
- Micropayments
- Web Extraction
- Feed Aggregation
- Credential Broker
- API Gateway
- Agent Security
- agent-native
---
