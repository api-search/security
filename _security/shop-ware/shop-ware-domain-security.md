---
api_specs:
- filename: shop-ware-v2-openapi-original.yml
  format: yaml
  label: Shop-Ware Partner API V2
  slug: shop-ware-partner-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shop-ware/refs/heads/main/openapi/shop-ware-v2-openapi-original.yml
- filename: shop-ware-v1-openapi-original.yml
  format: yaml
  label: Shop-Ware Partner API V1
  slug: shop-ware-partner-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shop-ware/refs/heads/main/openapi/shop-ware-v1-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shop-ware.com
  spf: true
hosts:
- cert_expires: Sep  1 06:03:31 2026 GMT
  host: www.shop-ware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:30:27 2026 GMT
  host: api.shop-ware.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shop Ware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shop-Ware, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shop-Ware
provider_slug: shop-ware
slug: shop-ware-domain-security
source_filename: shop-ware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shop-ware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:03:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.shop-ware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shop-ware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shop-ware/refs/heads/main/security/shop-ware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Auto Repair
- Shop Management
- Repair Orders
- Field Service
- SaaS
- Webhooks
- Payments
---
