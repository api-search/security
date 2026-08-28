---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shiphawk.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: shiphawk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: docs.shiphawk.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shiphawk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipHawk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShipHawk
provider_slug: shiphawk
slug: shiphawk-domain-security
source_filename: shiphawk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shiphawk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.shiphawk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: shiphawk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiphawk/refs/heads/main/security/shiphawk-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Shipping
- Logistics
- Transportation Management
- Warehouse Management
- Freight
- Parcel
- Fulfillment
- eCommerce
- Supply Chain
- Carriers
- Rate Shopping
- Tracking
- Webhooks
---
