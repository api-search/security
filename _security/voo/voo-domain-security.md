---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sideup.co
  spf: true
hosts:
- cert_expires: Oct  7 15:10:30 2026 GMT
  host: sa.sideup.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VOO (now SideUp), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VOO (now SideUp)
provider_slug: voo
slug: voo-domain-security
source_filename: voo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sa.sideup.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:10:30 2026 GMT\n  hsts: false\ndomains:\n- domain: sideup.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voo/refs/heads/main/security/voo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Logistics
- Shipping
- eCommerce
- Delivery
- Fulfillment
- Couriers
- Saudi Arabia
- Egypt
---
