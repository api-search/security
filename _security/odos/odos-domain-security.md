---
api_specs:
- filename: openapi.json
  format: json
  label: Odos Smart Order Router API
  slug: odos-smart-order-router-api
  spec_type: OpenAPI
  url: https://api.odos.xyz/sor/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: odos.xyz
  spf: true
hosts:
- cert_expires: Sep 30 14:49:39 2026 GMT
  host: enterprise.odos.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:49:39 2026 GMT
  host: docs.odos.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:49:39 2026 GMT
  host: api.odos.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Odos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Odos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Odos
provider_slug: odos
slug: odos-domain-security
source_filename: odos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enterprise.odos.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:49:39 2026 GMT\n  hsts: false\n- host: docs.odos.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:49:39 2026 GMT\n  hsts: false\n- host: api.odos.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:49:39 2026 GMT\n  hsts: null\ndomains:\n- domain: odos.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odos/refs/heads/main/security/odos-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DEX
- Aggregator
- DeFi
- Token Swaps
- Liquidity
- Routing
- Blockchain
- EVM
- Web3
---
