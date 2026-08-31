---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: logiwa.com
  spf: true
hosts:
- cert_expires: Jan  2 11:39:20 2027 GMT
  host: www.logiwa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 11:39:20 2027 GMT
  host: developer.logiwa.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 12 15:01:57 2026 GMT
  host: app.logiwa.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Logiwa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logiwa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Logiwa
provider_slug: logiwa
slug: logiwa-domain-security
source_filename: logiwa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.logiwa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 11:39:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.logiwa.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 11:39:20 2027 GMT\n  hsts: false\n- host: app.logiwa.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 15:01:57 2026 GMT\n  hsts: null\ndomains:\n- domain: logiwa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logiwa/refs/heads/main/security/logiwa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Warehouse Management
- Fulfillment
- Logistics
- Supply Chain
- Inventory Management
- Order Management
- Third Party Logistics
- E-Commerce
- Shipping
- Webhook
- Software-as-a-Service
---
