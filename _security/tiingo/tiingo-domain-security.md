---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tiingo.com
  spf: true
hosts:
- cert_expires: Sep 24 02:59:33 2026 GMT
  host: www.tiingo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:21:41 2026 GMT
  host: api.tiingo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiingo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tiingo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Tiingo
provider_slug: tiingo
slug: tiingo-domain-security
source_filename: tiingo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiingo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:59:33 2026 GMT\n  hsts: false\n- host: api.tiingo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:21:41 2026 GMT\n  hsts: false\ndomains:\n- domain: tiingo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/security/tiingo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fintech
- Market Data
- Stocks
- Crypto
- FX
- News
- Fundamentals
- WebSockets
---
