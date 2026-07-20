---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: leo.app
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: aleorpc.com
  spf: false
hosts:
- cert_expires: Sep 16 18:44:51 2026 GMT
  host: docs.leo.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: testnetbeta.aleorpc.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Demox Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Demox Labs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Demox Labs
provider_slug: demox-labs
slug: demox-labs-domain-security
source_filename: demox-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.leo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:44:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: testnetbeta.aleorpc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: leo.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: aleorpc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demox-labs/refs/heads/main/security/demox-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Blockchain
- Zero Knowledge
- Cryptocurrency
- Wallet
- Privacy
- Web3
- Developer Tools
- SDK
- JSON-RPC
---
