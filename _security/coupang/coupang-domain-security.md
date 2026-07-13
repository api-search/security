---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coupang.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: coupangcorp.com
  spf: false
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.coupang.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:42:30 2026 GMT
  host: developers.coupangcorp.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api-gateway.coupang.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coupang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coupang, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coupang
provider_slug: coupang
slug: coupang-domain-security
source_filename: coupang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coupang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: developers.coupangcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:42:30 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api-gateway.coupang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coupang.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: coupangcorp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coupang/refs/heads/main/security/coupang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cancellations
- E-commerce
- Korea
- Marketplace
- Open API
- Orders
- Products
- Returns
- Sellers
- Settlement
- Vendors
---
