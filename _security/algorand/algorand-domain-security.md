---
api_specs:
- filename: algod.oas3.yml
  format: yaml
  label: Algorand Algod REST API
  slug: algorand-algod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/algorand/go-algorand/master/daemon/algod/api/algod.oas3.yml
- filename: indexer.oas3.yml
  format: yaml
  label: Algorand Indexer REST API
  slug: algorand-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/algorand/indexer/main/api/indexer.oas3.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: algorand.co
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: nodely.dev
  spf: false
hosts:
- cert_expires: Aug 29 18:41:32 2026 GMT
  host: algorand.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 21:19:56 2026 GMT
  host: dev.algorand.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 16:09:24 2026 GMT
  host: mainnet-api.4160.nodely.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Algorand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Algorand, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Algorand
provider_slug: algorand
slug: algorand-domain-security
source_filename: algorand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: algorand.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:41:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.algorand.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:19:56 2026 GMT\n  hsts: false\n- host: mainnet-api.4160.nodely.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:09:24 2026 GMT\n  hsts: false\ndomains:\n- domain: algorand.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nodely.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algorand/refs/heads/main/security/algorand-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- Proof-of-Stake
- DeFi
- Smart Contracts
---
