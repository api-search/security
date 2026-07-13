---
api_specs:
- filename: jito-block-engine-openapi.yml
  format: yaml
  label: Jito Block Engine JSON-RPC API
  slug: jito-block-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jito/refs/heads/main/openapi/jito-block-engine-openapi.yml
- filename: jito-bundles-tip-floor-openapi.yml
  format: yaml
  label: Jito Bundles Tip Floor API
  slug: jito-bundles-tip-floor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jito/refs/heads/main/openapi/jito-bundles-tip-floor-openapi.yml
- filename: jito-streaming-asyncapi.yml
  format: yaml
  label: Jito Streaming Surfaces
  slug: jito-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jito/refs/heads/main/asyncapi/jito-streaming-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jito.network
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jito.wtf
  spf: false
hosts:
- cert_expires: Aug 21 23:49:31 2026 GMT
  host: www.jito.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 07:10:13 2026 GMT
  host: docs.jito.wtf
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 14:30:17 2026 GMT
  host: mainnet.block-engine.jito.wtf
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jito Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Jito Labs
provider_slug: jito
slug: jito-domain-security
source_filename: jito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jito.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:49:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.jito.wtf\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:10:13 2026 GMT\n  hsts: false\n- host: mainnet.block-engine.jito.wtf\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:30:17 2026 GMT\n  hsts: null\ndomains:\n- domain: jito.network\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: jito.wtf\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jito/refs/heads/main/security/jito-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Solana
- MEV
- Block Engine
- Bundles
- Liquid Staking
- JitoSOL
- Restaking
- JTO
- DAO
- Validator
- Searcher
- ShredStream
- Crypto
- DeFi
---
