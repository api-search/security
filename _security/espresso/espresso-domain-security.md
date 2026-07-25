---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: espressosys.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: espresso.network
  spf: false
hosts:
- cert_expires: Aug 20 14:31:50 2026 GMT
  host: www.espressosys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 09:14:01 2026 GMT
  host: docs.espressosys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: query.main.net.espresso.network
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Espresso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Espresso, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Espresso
provider_slug: espresso
slug: espresso-domain-security
source_filename: espresso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.espressosys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.espressosys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:14:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: query.main.net.espresso.network\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: espressosys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: espresso.network\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/espresso/refs/heads/main/security/espresso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Web3
- Infrastructure
- Consensus
- Sequencer
- Rollup
- Data Availability
- Ethereum
- DeFi
- REST API
- Cryptography
---
