---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coinsuper.com
  spf: false
hosts:
- cert_expires: Aug 23 08:04:19 2026 GMT
  host: www.coinsuper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinsuper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinsuper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Coinsuper
provider_slug: coinsuper
slug: coinsuper-domain-security
source_filename: coinsuper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coinsuper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:04:19 2026 GMT\n  hsts: false\ndomains:\n- domain: coinsuper.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinsuper/refs/heads/main/security/coinsuper-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Bitcoin
---
