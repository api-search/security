---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flashexpress.com
  spf: true
hosts:
- cert_expires: Nov 11 06:42:44 2026 GMT
  host: flashexpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 11 06:42:44 2026 GMT
  host: open-docs.flashexpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 06:42:44 2026 GMT
  host: open-api.flashexpress.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flash Express Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flash Express, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flash Express
provider_slug: flash-express
slug: flash-express-domain-security
source_filename: flash-express-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flashexpress.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 06:42:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open-docs.flashexpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 06:42:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open-api.flashexpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 06:42:44 2026 GMT\n  hsts: null\ndomains:\n- domain: flashexpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flash-express/refs/heads/main/security/flash-express-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Logistics
- Shipping
- Delivery
- Parcel Tracking
- E-Commerce
- Last Mile
- Courier
- Cash on Delivery
- Thailand
- Southeast Asia
- Webhooks
---
