---
api_specs:
- filename: m-0-orchestration-openapi.json
  format: json
  label: M0 Orchestration API
  slug: m0-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/m-0/refs/heads/main/openapi/m-0-orchestration-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: m0.xyz
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: gateway.m0.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: gateway.stage.m0.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: gateway.dev.m0.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: M 0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M 0, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: M 0
provider_slug: m-0
slug: m-0-domain-security
source_filename: m-0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gateway.m0.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\n- host: gateway.stage.m0.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\n- host: gateway.dev.m0.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: m0.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m-0/refs/heads/main/security/m-0-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Stablecoin
- Cryptocurrency
- Blockchain
- Payments
- DeFi
- Web3
- Cross-Chain
- Tokenization
- Infrastructure
---
