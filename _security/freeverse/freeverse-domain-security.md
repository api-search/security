---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: laosnetwork.io
  spf: true
hosts:
- cert_expires: Sep  3 23:49:53 2026 GMT
  host: laosnetwork.io
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 18:17:38 2026 GMT
  host: docs.laosnetwork.io
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 10:02:38 2026 GMT
  host: api.laosnetwork.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freeverse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freeverse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Freeverse
provider_slug: freeverse
slug: freeverse-domain-security
source_filename: freeverse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laosnetwork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:49:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: docs.laosnetwork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 18:17:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.laosnetwork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:02:38 2026 GMT\n  hsts: null\ndomains:\n- domain: laosnetwork.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeverse/refs/heads/main/security/freeverse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- NFT
- Web3
- Digital Assets
- Gaming
- GraphQL
- Polkadot
- Ethereum
- Tokenization
---
