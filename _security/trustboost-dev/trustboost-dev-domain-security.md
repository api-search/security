---
api_specs:
- filename: trustboost-dev-openapi.json
  format: json
  label: TrustBoost PII Sanitizer API
  slug: trustboost-pii-sanitizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustboost-dev/refs/heads/main/openapi/trustboost-dev-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trustboost.dev
  spf: true
hosts:
- cert_expires: Nov 22 07:52:49 2026 GMT
  host: api.trustboost.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trustboost Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrustBoost PII Sanitizer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TrustBoost PII Sanitizer
provider_slug: trustboost-dev
slug: trustboost-dev-domain-security
source_filename: trustboost-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.trustboost.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 07:52:49 2026 GMT\n  hsts: null\ndomains:\n- domain: trustboost.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustboost-dev/refs/heads/main/security/trustboost-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Privacy
- PII Redaction
- Data Protection
- LLM Security
- AI Safety
- Agents
- A2A
- MCP
- x402
- Agentic Commerce
- Solana
- Compliance
- agent-native
---
