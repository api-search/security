---
api_specs:
- filename: lootrush-openapi-original.json
  format: json
  label: LootRush Partner API
  slug: lootrush-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lootrush/refs/heads/main/openapi/lootrush-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lootrush.com
  spf: false
hosts:
- cert_expires: Aug 31 15:09:44 2026 GMT
  host: www.lootrush.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lootrush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LootRush, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: LootRush
provider_slug: lootrush
slug: lootrush-domain-security
source_filename: lootrush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lootrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:09:44 2026 GMT\n  hsts: null\ndomains:\n- domain: lootrush.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lootrush/refs/heads/main/security/lootrush-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Crypto
- Cryptocurrency
- Payments
- Withdrawals
- MCP
- API
---
