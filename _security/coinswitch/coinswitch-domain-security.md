---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coinswitch.co
  spf: true
hosts:
- cert_expires: Aug 25 05:05:07 2026 GMT
  host: coinswitch.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinswitch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinSwitch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CoinSwitch
provider_slug: coinswitch
slug: coinswitch-domain-security
source_filename: coinswitch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinswitch.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:05:07 2026 GMT\n  hsts: false\ndomains:\n- domain: coinswitch.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinswitch/refs/heads/main/security/coinswitch-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Crypto Exchange
- Trading
- Fintech
- Futures
- Spot Trading
- WebSocket
- India
---
