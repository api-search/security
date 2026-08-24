---
api_specs:
- filename: jobox-ai-kili-openapi.json
  format: json
  label: Jobox Kili API
  slug: kili
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobox-ai/refs/heads/main/openapi/jobox-ai-kili-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jobox.ai
  spf: true
hosts:
- cert_expires: Sep 29 10:12:18 2026 GMT
  host: www.jobox.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.jobox.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jobox Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JOBOX.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JOBOX.ai
provider_slug: jobox-ai
slug: jobox-ai-domain-security
source_filename: jobox-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jobox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:12:18 2026 GMT\n  hsts: false\n- host: api.jobox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jobox.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobox-ai/refs/heads/main/security/jobox-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Home Services
- Field Service Management
- Marketplace
- Payments
- Fintech
- Dispatching
- Skilled Trades
- KYC
- Wallet
---
