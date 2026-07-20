---
api_specs:
- filename: enso-openapi-original.json
  format: json
  label: Enso API
  slug: enso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/openapi/enso-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enso.build
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enso.finance
  spf: true
hosts:
- cert_expires: Sep 26 12:04:31 2026 GMT
  host: enso.build
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 12 00:49:37 2026 GMT
  host: docs.enso.build
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  9 23:14:39 2026 GMT
  host: api.enso.finance
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Enso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enso, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Enso
provider_slug: enso
slug: enso-domain-security
source_filename: enso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enso.build\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 12:04:31 2026 GMT\n  hsts: null\n- host: docs.enso.build\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 00:49:37 2026 GMT\n  hsts: null\n- host: api.enso.finance\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 23:14:39 2026 GMT\n  hsts: null\ndomains:\n- domain: enso.build\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: enso.finance\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enso/refs/heads/main/security/enso-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Crypto Web3
- DeFi
- Blockchain
- Cross-chain
- Smart Contracts
- Transaction Routing
- Web3 Infrastructure
- Onchain
---
