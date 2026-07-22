---
api_specs:
- filename: paid-v2.json
  format: json
  label: Paid API v2
  slug: paid-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-v2.json
- filename: paid-v1.json
  format: json
  label: Paid API v1
  slug: paid-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/openapi/paid-v1.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentpaid.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: agentpaid.io
  spf: false
hosts:
- host: www.agentpaid.ai
  https: false
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.agentpaid.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paid, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Paid
provider_slug: paid
slug: paid-domain-security
source_filename: paid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agentpaid.ai\n  https: false\n- host: api.agentpaid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: agentpaid.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: agentpaid.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paid/refs/heads/main/security/paid-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Billing
- Monetization
- Payments
- Usage-Based Pricing
- AI Agents
- FinOps
---
