---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xrpl.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: xrplcluster.com
  spf: false
hosts:
- cert_expires: Aug 21 11:11:44 2026 GMT
  host: xrpl.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 03:27:15 2026 GMT
  host: xrplcluster.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- host: s.altnet.rippletest.net
  https: false
kind: domain-security
layout: security
method: probed
name: Xrpl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XRP Ledger, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: XRP Ledger
provider_slug: xrpl
slug: xrpl-domain-security
source_filename: xrpl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xrpl.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:11:44 2026 GMT\n  hsts: false\n- host: xrplcluster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:27:15 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: s.altnet.rippletest.net\n  https: false\ndomains:\n- domain: xrpl.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: xrplcluster.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xrpl/refs/heads/main/security/xrpl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- XRP
- Cryptocurrency
- DeFi
- Ledger
- Web3
---
