---
api_specs:
- filename: ship24-api-for-per-call-plans-api-openapi.yml
  format: yaml
  label: Ship24 ➕ API for per-call plans API
  slug: ship24-api-for-per-call-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ship24/refs/heads/main/openapi/ship24-api-for-per-call-plans-api-openapi.yml
- filename: ship24-couriers-api-openapi.yml
  format: yaml
  label: Ship24 🚚 Couriers API
  slug: ship24-couriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ship24/refs/heads/main/openapi/ship24-couriers-api-openapi.yml
- filename: ship24-trackers-api-openapi.yml
  format: yaml
  label: Ship24 📦 Trackers API
  slug: ship24-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ship24/refs/heads/main/openapi/ship24-trackers-api-openapi.yml
- filename: ship24-ship24-tracking-api-api-openapi.yml
  format: yaml
  label: Ship24 Ship24 Tracking API
  slug: ship24-ship24-tracking-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ship24/refs/heads/main/openapi/ship24-ship24-tracking-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ship24.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.ship24.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: docs.ship24.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: api.ship24.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ship24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ship24, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ship24
provider_slug: ship24
slug: ship24-domain-security
source_filename: ship24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ship24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ship24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\n- host: api.ship24.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ship24.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ship24/refs/heads/main/security/ship24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tracking
- Logistics
- Shipping
- Couriers
- Parcels
- Webhook
- E-Commerce
- Post-Purchase
---
