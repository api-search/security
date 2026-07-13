---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bandprotocol.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bandchain.org
  spf: false
hosts:
- cert_expires: Aug 30 22:37:32 2026 GMT
  host: bandprotocol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 20:33:24 2026 GMT
  host: docs.bandchain.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 06:36:05 2026 GMT
  host: laozi1.bandchain.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Band Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Band Protocol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Band Protocol
provider_slug: band-protocol
slug: band-protocol-domain-security
source_filename: band-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bandprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 22:37:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bandchain.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: laozi1.bandchain.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:36:05 2026 GMT\n  hsts: null\ndomains:\n- domain: bandprotocol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bandchain.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/band-protocol/refs/heads/main/security/band-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Oracle
- Data Feeds
- Price Feeds
- Cross-Chain
- DeFi
- Cosmos
---
