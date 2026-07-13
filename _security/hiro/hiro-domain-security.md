---
api_specs:
- filename: hiro-stacks-blockchain-api-openapi.yaml
  format: yaml
  label: Stacks Blockchain API
  slug: stacks-blockchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/openapi/hiro-stacks-blockchain-api-openapi.yaml
- filename: hiro-stacks-node-rpc-api-openapi.yaml
  format: yaml
  label: Stacks Node RPC API
  slug: stacks-node-rpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/openapi/hiro-stacks-node-rpc-api-openapi.yaml
- filename: hiro-token-metadata-api-openapi.yaml
  format: yaml
  label: Hiro Token Metadata API
  slug: token-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/openapi/hiro-token-metadata-api-openapi.yaml
- filename: hiro-signer-metrics-api-openapi.yaml
  format: yaml
  label: Hiro Signer Metrics API
  slug: signer-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/openapi/hiro-signer-metrics-api-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hiro.so
  spf: true
hosts:
- cert_expires: Aug 10 20:11:42 2026 GMT
  host: www.hiro.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 11:58:13 2026 GMT
  host: docs.hiro.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 04:15:59 2026 GMT
  host: api.mainnet.hiro.so
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hiro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hiro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hiro
provider_slug: hiro
slug: hiro-domain-security
source_filename: hiro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hiro.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 20:11:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hiro.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:58:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mainnet.hiro.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 04:15:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hiro.so\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiro/refs/heads/main/security/hiro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Blockchain
- Bitcoin
- Stacks
- sBTC
- Indexing
---
