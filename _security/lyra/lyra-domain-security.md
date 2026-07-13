---
api_specs:
- filename: llms.txt
  format: yaml
  label: Lyra Public REST API
  slug: lyra-public-rest-api
  spec_type: OpenAPI
  url: https://docs.derive.xyz/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: derive.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lyra.finance
  spf: true
hosts:
- cert_expires: Oct  7 00:48:15 2026 GMT
  host: docs.derive.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 01:38:05 2026 GMT
  host: api.lyra.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lyra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lyra, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lyra
provider_slug: lyra
slug: lyra-domain-security
source_filename: lyra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.derive.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:48:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lyra.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:38:05 2026 GMT\n  hsts: null\ndomains:\n- domain: derive.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lyra.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyra/refs/heads/main/security/lyra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Options
- AMM
- DeFi
- Derivatives
- Implied Volatility
- Perpetuals
- Crypto
- Finance
---
