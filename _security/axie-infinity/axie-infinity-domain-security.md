---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axieinfinity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: skymavis.com
  spf: true
hosts:
- cert_expires: Sep 24 02:34:03 2026 GMT
  host: axieinfinity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 09:09:05 2026 GMT
  host: docs.skymavis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 09:54:04 2026 GMT
  host: api-gateway.skymavis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axie Infinity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axie Infinity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axie Infinity
provider_slug: axie-infinity
slug: axie-infinity-domain-security
source_filename: axie-infinity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axieinfinity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:34:03 2026 GMT\n  hsts: null\n- host: docs.skymavis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:09:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-gateway.skymavis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 09:54:04 2026 GMT\n  hsts: null\ndomains:\n- domain: axieinfinity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: skymavis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axie-infinity/refs/heads/main/security/axie-infinity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Blockchain
- Web3
- NFT
- Game Data
- Leaderboards
- Ronin
- Play to Earn
---
