---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sidelineswap.com
  spf: true
hosts:
- cert_expires: Sep 12 21:33:08 2026 GMT
  host: sidelineswap.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: developer.sidelineswap.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api.sidelineswap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sidelineswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SidelineSwap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SidelineSwap
provider_slug: sidelineswap
slug: sidelineswap-domain-security
source_filename: sidelineswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sidelineswap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:33:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.sidelineswap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.sidelineswap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sidelineswap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidelineswap/refs/heads/main/security/sidelineswap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Sports
- Sporting Goods
- Ecommerce
- Commerce
- Inventory
- Resale
- Consignment
---
