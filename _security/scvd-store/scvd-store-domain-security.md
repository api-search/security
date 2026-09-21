---
api_specs:
- filename: scvd-store-openapi.json
  format: json
  label: SCVD General Store API
  slug: scvd-general-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scvd-store/refs/heads/main/openapi/scvd-store-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scvd.store
  spf: true
hosts:
- cert_expires: Dec 18 17:55:20 2026 GMT
  host: scvd.store
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scvd Store Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Record Creative Co. LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Record Creative Co. LLC
provider_slug: scvd-store
slug: scvd-store-domain-security
source_filename: scvd-store-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scvd.store\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 17:55:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scvd.store\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scvd-store/refs/heads/main/security/scvd-store-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agents
- Agentic Commerce
- x402
- Payments
- Micropayments
- Stablecoins
- USDC
- Verification
- Conformance
- Attestation
- Observability
- MCP
- A2A
- Universal Commerce Protocol
- Signatures
- agent-native
- United States
---
