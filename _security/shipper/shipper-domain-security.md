---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shipper.id
  spf: true
hosts:
- cert_expires: Sep  8 10:24:02 2026 GMT
  host: shipper.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 17:36:07 2026 GMT
  host: logistics-docs.shipper.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: merchant-api.shipper.id
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shipper, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shipper
provider_slug: shipper
slug: shipper-domain-security
source_filename: shipper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shipper.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:24:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: logistics-docs.shipper.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:36:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: merchant-api.shipper.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shipper.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipper/refs/heads/main/security/shipper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Shipping
- Fulfillment
- Supply Chain
- E-commerce
- Last Mile Delivery
- Courier
- Indonesia
---
