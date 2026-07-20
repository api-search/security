---
api_specs:
- filename: exponential-protocol-openapi.yml
  format: yaml
  label: YO Protocol API
  slug: yo-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/openapi/exponential-protocol-openapi.yml
- filename: exponential-risk-graph-openapi.yml
  format: yaml
  label: YO Risk Graph API
  slug: yo-risk-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/openapi/exponential-risk-graph-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: exponential.fi
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yo.xyz
  spf: true
hosts:
- cert_expires: Sep  8 20:37:07 2026 GMT
  host: exponential.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 18:03:27 2026 GMT
  host: docs.yo.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 13:56:57 2026 GMT
  host: api.yo.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exponential Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exponential, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Exponential
provider_slug: exponential
slug: exponential-domain-security
source_filename: exponential-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exponential.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:37:07 2026 GMT\n  hsts: null\n- host: docs.yo.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:03:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.yo.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 13:56:57 2026 GMT\n  hsts: null\ndomains:\n- domain: exponential.fi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: yo.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/security/exponential-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DeFi
- Decentralized Finance
- Yield
- Yield Optimizer
- Vaults
- ERC-4626
- Cross-chain
- Blockchain
- Crypto
- Risk
- Risk Ratings
- Agents
- x402
- Web3
---
