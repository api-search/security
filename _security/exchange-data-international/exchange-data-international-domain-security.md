---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exchange-data.com
  spf: true
hosts:
- cert_expires: Sep  4 10:16:49 2026 GMT
  host: www.exchange-data.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 13:18:07 2026 GMT
  host: developer.exchange-data.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 13:18:07 2026 GMT
  host: api3.exchange-data.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exchange Data International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exchange Data International, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Exchange Data International
provider_slug: exchange-data-international
slug: exchange-data-international-domain-security
source_filename: exchange-data-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exchange-data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 10:16:49 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.exchange-data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 13:18:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api3.exchange-data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 13:18:07 2026 GMT\n  hsts: null\ndomains:\n- domain: exchange-data.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exchange-data-international/refs/heads/main/security/exchange-data-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Market Data
- Corporate Actions
- Reference Data
- End of Day Pricing
- Fixed Income
- Derivatives
- Economic Data
- Stocks
- Exchange
---
