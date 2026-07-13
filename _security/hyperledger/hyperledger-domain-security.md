---
api_specs:
- filename: hyperledger-openapi.yml
  format: yaml
  label: Hyperledger Besu API
  slug: hyperledger-besu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperledger/refs/heads/main/openapi/hyperledger-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyperledger.org
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Aug  8 21:29:55 2026 GMT
  host: besu.hyperledger.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: hyperledger-fabric.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 08:43:14 2026 GMT
  host: www.hyperledger.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperledger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperledger, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hyperledger
provider_slug: hyperledger
slug: hyperledger-domain-security
source_filename: hyperledger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: besu.hyperledger.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 21:29:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: hyperledger-fabric.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.hyperledger.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hyperledger.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf:\
  \ false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperledger/refs/heads/main/security/hyperledger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Distributed Ledger
- Enterprise
- Linux Foundation
- Smart Contracts
---
