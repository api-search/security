---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: htx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huobi.pro
  spf: true
hosts:
- cert_expires: Nov  4 08:41:35 2026 GMT
  host: htx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 08:32:28 2026 GMT
  host: www.htx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.huobi.pro
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Htx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HTX
provider_slug: htx
slug: htx-domain-security
source_filename: htx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: htx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 08:41:35 2026 GMT\n  hsts: false\n- host: www.htx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:32:28 2026 GMT\n  hsts: false\n- host: api.huobi.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: htx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: huobi.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/htx/refs/heads/main/security/htx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Cryptocurrency
- Crypto Exchange
- Trading
- Digital Assets
- Blockchain
- Financial Services
- Market Data
- WebSocket
---
