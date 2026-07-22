---
api_specs:
- filename: valora-api-openapi.yml
  format: yaml
  label: Valora API
  slug: valora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valora/refs/heads/main/openapi/valora-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: valora.xyz
  spf: true
hosts:
- cert_expires: Sep 12 04:02:08 2026 GMT
  host: valora.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 17:04:00 2026 GMT
  host: api.mainnet.valora.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.alfajores.valora.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: Valora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valora, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Valora
provider_slug: valora
slug: valora-domain-security
source_filename: valora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valora.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:02:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mainnet.valora.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:04:00 2026 GMT\n  hsts: null\n- host: api.alfajores.valora.xyz\n  https: false\ndomains:\n- domain: valora.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valora/refs/heads/main/security/valora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Cryptocurrency
- Wallet
- Payments
- DeFi
- Blockchain
- Celo
- Mobile
---
