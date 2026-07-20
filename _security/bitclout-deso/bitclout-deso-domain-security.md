---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deso.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: deso.org
  spf: true
hosts:
- cert_expires: Oct 10 12:37:44 2026 GMT
  host: www.deso.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 22:24:52 2026 GMT
  host: docs.deso.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:11:17 2026 GMT
  host: node.deso.org
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitclout Deso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitClout (DeSo), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BitClout (DeSo)
provider_slug: bitclout-deso
slug: bitclout-deso-domain-security
source_filename: bitclout-deso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 12:37:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.deso.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 22:24:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: node.deso.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:11:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: deso.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: deso.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitclout-deso/refs/heads/main/security/bitclout-deso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- Decentralized Social
- Web3
- Social Media
- NFT
- Creator Economy
---
