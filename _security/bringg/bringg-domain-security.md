---
api_specs:
- filename: bringg-delivery-hub-api-openapi.yml
  format: yaml
  label: Bringg Delivery Hub API
  slug: bringg-delivery-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/openapi/bringg-delivery-hub-api-openapi.yml
- filename: bringg-drivers-shifts-api-openapi.yml
  format: yaml
  label: Bringg Drivers And Shifts API
  slug: bringg-drivers-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/openapi/bringg-drivers-shifts-api-openapi.yml
- filename: bringg-fleet-partners-api-openapi.yml
  format: yaml
  label: Bringg Fleet Partners API
  slug: bringg-fleet-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/openapi/bringg-fleet-partners-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bringg.com
  spf: true
hosts:
- cert_expires: Oct  4 05:54:23 2026 GMT
  host: www.bringg.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 00:11:51 2026 GMT
  host: developers.bringg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: us2-admin-api.bringg.com
  hsts: true
  hsts_max_age: 2419200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bringg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bringg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bringg
provider_slug: bringg
slug: bringg-domain-security
source_filename: bringg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bringg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:54:23 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developers.bringg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 00:11:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us2-admin-api.bringg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2419200\ndomains:\n- domain: bringg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/security/bringg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Last-Mile Delivery
- Delivery Orchestration
- Fulfillment
- Logistics
- Retail
- Dispatch
- Routing
- Driver App
- Carrier Network
- Fleet Management
- Supply Chain
- E-commerce
- Same-Day Delivery
- Curbside Pickup
- Returns
---
