---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lazada.com
  spf: true
hosts:
- cert_expires: Dec 25 06:36:26 2026 GMT
  host: open.lazada.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 25 06:36:26 2026 GMT
  host: auth.lazada.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 25 06:36:26 2026 GMT
  host: api.lazada.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lazada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lazada, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lazada
provider_slug: lazada
slug: lazada-domain-security
source_filename: lazada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.lazada.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 06:36:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.lazada.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 06:36:26 2026 GMT\n  hsts: null\n- host: api.lazada.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 06:36:26 2026 GMT\n  hsts: null\ndomains:\n- domain: lazada.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lazada/refs/heads/main/security/lazada-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- E-commerce
- Marketplace
- Southeast Asia
- Alibaba
- Orders
- Products
- Logistics
- Lazada
---
