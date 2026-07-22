---
api_specs:
- filename: sommelier-api-openapi.yml
  format: yaml
  label: Sommelier Finance API
  slug: sommelier-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sommelier/refs/heads/main/openapi/sommelier-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: sommelier.finance
  spf: true
hosts:
- cert_expires: Oct 12 17:59:30 2026 GMT
  host: sommelier.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:11:39 2026 GMT
  host: api.sommelier.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sommelier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sommelier, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Sommelier
provider_slug: sommelier
slug: sommelier-domain-security
source_filename: sommelier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sommelier.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 17:59:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sommelier.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:11:39 2026 GMT\n  hsts: false\ndomains:\n- domain: sommelier.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sommelier/refs/heads/main/security/sommelier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Crypto Web3
- DeFi
- Blockchain
- Ethereum
- Vaults
- Yield
- Analytics
---
