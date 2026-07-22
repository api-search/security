---
api_specs:
- filename: wonderment-openapi.json
  format: json
  label: Wonderment API
  slug: wonderment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wonderment/refs/heads/main/openapi/wonderment-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wonderment.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.wonderment.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wonderment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wonderment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wonderment
provider_slug: wonderment
slug: wonderment-domain-security
source_filename: wonderment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wonderment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wonderment.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wonderment/refs/heads/main/security/wonderment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Order Tracking
- Post-Purchase
- Shipping
- Logistics
- Shopify
- Webhooks
---
