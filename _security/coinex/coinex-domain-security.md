---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinex.com
  spf: true
hosts:
- cert_expires: Sep 18 13:02:24 2026 GMT
  host: docs.coinex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.coinex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: socket.coinex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinEx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoinEx
provider_slug: coinex
slug: coinex-domain-security
source_filename: coinex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.coinex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:02:24 2026 GMT\n  hsts: false\n- host: api.coinex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\n- host: socket.coinex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coinex.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinex/refs/heads/main/security/coinex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cryptocurrency
- Exchange
- Spot Trading
- Futures
- Perpetual Contracts
- Market Data
- WebSocket
- Finance
---
