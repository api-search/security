---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: volusion.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: yourstore.com
  spf: true
hosts:
- cert_expires: Sep 25 22:19:44 2026 GMT
  host: www.volusion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 07:21:18 2026 GMT
  host: help.volusion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 14:52:39 2027 GMT
  host: yourstore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Volusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volusion, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Volusion
provider_slug: volusion
slug: volusion-domain-security
source_filename: volusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.volusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:19:44 2026 GMT\n  hsts: false\n- host: help.volusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:21:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourstore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 14:52:39 2027 GMT\n  hsts: null\ndomains:\n- domain: volusion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: yourstore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volusion/refs/heads/main/security/volusion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Commerce
- Online Store
- Products
- Orders
- Customers
- Inventory
- Shopping Cart
---
