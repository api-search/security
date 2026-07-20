---
api_specs:
- filename: infstones-bnb-chain-openapi.json
  format: json
  label: InfStones RPC API
  slug: infstones-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infstones/refs/heads/main/openapi/infstones-bnb-chain-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: infstones.com
  spf: true
hosts:
- cert_expires: Oct 16 23:27:52 2026 GMT
  host: infstones.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 01:49:16 2026 GMT
  host: docs.infstones.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 00:43:10 2026 GMT
  host: api.infstones.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infstones Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InfStones, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: InfStones
provider_slug: infstones
slug: infstones-domain-security
source_filename: infstones-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infstones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:27:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.infstones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:49:16 2026 GMT\n  hsts: null\n- host: api.infstones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:43:10 2026 GMT\n  hsts: null\ndomains:\n- domain: infstones.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infstones/refs/heads/main/security/infstones-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Node Infrastructure
- Staking
- Web3
- JSON-RPC
- RPC
- Ethereum
- BNB Chain
- Cosmos
- Cryptocurrency
- API
---
