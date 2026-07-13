---
api_specs:
- filename: filecoin-http-api
  format: yaml
  label: Filecoin HTTP REST API
  slug: filecoin-http-rest-api
  spec_type: OpenAPI
  url: https://github.com/filecoin-project/filecoin-http-api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: filecoin.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: glif.io
  spf: true
hosts:
- cert_expires: Sep  5 02:17:17 2026 GMT
  host: docs.filecoin.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 07:47:39 2026 GMT
  host: api.node.glif.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 07:47:39 2026 GMT
  host: api.calibration.node.glif.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Filecoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Filecoin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Filecoin
provider_slug: filecoin
slug: filecoin-domain-security
source_filename: filecoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.filecoin.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 02:17:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.node.glif.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:47:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.calibration.node.glif.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:47:39 2026 GMT\n  hsts: null\ndomains:\n- domain: filecoin.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: glif.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filecoin/refs/heads/main/security/filecoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Decentralized Storage
- Web3
- IPFS
- Blockchain
- Storage Deals
- Filecoin+
- FVM
---
