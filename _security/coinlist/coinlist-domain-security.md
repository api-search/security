---
api_specs:
- filename: coinlist-passage-openapi-original.json
  format: json
  label: CoinList Passage (Frontline API)
  slug: coinlist-passage-frontline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-passage-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coinlist.co
  spf: true
hosts:
- cert_expires: Sep 16 15:16:34 2026 GMT
  host: coinlist.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:16:34 2026 GMT
  host: api.coinlist.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinlist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinList, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CoinList
provider_slug: coinlist
slug: coinlist-domain-security
source_filename: coinlist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinlist.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:16:34 2026 GMT\n  hsts: false\n- host: api.coinlist.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:16:34 2026 GMT\n  hsts: null\ndomains:\n- domain: coinlist.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/security/coinlist-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- Token Sales
- Tokenized Equities
- KYC
- OAuth
- Blockchain
- Digital Assets
- Embedded Finance
---
