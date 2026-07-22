---
api_specs:
- filename: seismic-systems-src20-factory-openapi.yml
  format: yaml
  label: Seismic
  slug: seismic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic-systems/refs/heads/main/openapi/seismic-systems-src20-factory-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seismic.systems
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: seismictest.net
  spf: false
hosts:
- cert_expires: Aug 28 05:19:42 2026 GMT
  host: docs.seismic.systems
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:58:33 2026 GMT
  host: testnet-1.seismictest.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seismic Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seismic Systems, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seismic Systems
provider_slug: seismic-systems
slug: seismic-systems-domain-security
source_filename: seismic-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.seismic.systems\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 05:19:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: testnet-1.seismictest.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:58:33 2026 GMT\n  hsts: null\ndomains:\n- domain: seismic.systems\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: seismictest.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seismic-systems/refs/heads/main/security/seismic-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Privacy
- Encryption
- Stablecoins
- Fintech
- Web3
- Smart Contracts
- EVM
- Cryptography
- Developer Tools
---
