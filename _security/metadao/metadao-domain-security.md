---
api_specs:
- filename: metadao-futarchy-dex-openapi.yml
  format: yaml
  label: MetaDAO Futarchy DEX API
  slug: metadao-futarchy-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metadao/refs/heads/main/openapi/metadao-futarchy-dex-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: metadao.fi
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- host: metadao.fi
  hsts: false
  hsts_max_age: null
  https: true
  note: Behind rate limiting (HTTP 429 observed on automated GET); TLS handshake succeeded.
  tls_issuer: Let's Encrypt
  tls_not_after: '2026-09-20'
- host: market-api.metadao.fi
  hsts: null
  https: true
  note: Live public API host (GET /health returned 200 with a browser User-Agent). Cloudflare-fronted; returns 403 to non-browser clients. TLS reachable.
- host: api-docs.metadao.fi
  https: true
  note: Documentation host (Mintlify); reachable over HTTPS.
kind: domain-security
layout: security
method: probed
name: Metadao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MetaDAO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MetaDAO
provider_slug: metadao
slug: metadao-domain-security
source_filename: metadao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: 'dig + openssl s_client + curl HEAD (manual probe)'\nhosts:\n  - host: metadao.fi\n    https: true\n    tls_issuer: \"Let's Encrypt\"\n    tls_not_after: '2026-09-20'\n    hsts: false\n    hsts_max_age: null\n    note: Behind rate limiting (HTTP 429 observed on automated GET); TLS handshake succeeded.\n  - host: market-api.metadao.fi\n    https: true\n    hsts: null\n    note: >-\n      Live public API host (GET /health returned 200 with a browser User-Agent).\n      Cloudflare-fronted; returns 403 to non-browser clients. TLS reachable.\n  - host: api-docs.metadao.fi\n    https: true\n    note: Documentation host (Mintlify); reachable over HTTPS.\ndomains:\n  - domain: metadao.fi\n    dnssec: true\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 include:_spf.google.com ~all'\n    dmarc: true\n    dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metadao/refs/heads/main/security/metadao-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Crypto Tools
- DeFi
- Solana
- DEX
- Governance
- Market Data
- Futarchy
- API
---
