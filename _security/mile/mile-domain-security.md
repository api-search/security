---
api_specs:
- filename: mile-partner-api-openapi-original.json
  format: json
  label: Mile Partner API
  slug: mile-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-partner-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: milenow.com
  spf: true
hosts:
- cert_expires: Sep 18 01:15:55 2026 GMT
  host: milenow.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 01:15:55 2026 GMT
  host: lastmile.milenow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mile, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Mile
provider_slug: mile
slug: mile-domain-security
source_filename: mile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: milenow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:15:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: lastmile.milenow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:15:55 2026 GMT\n  hsts: false\ndomains:\n- domain: milenow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/security/mile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Last Mile Delivery
- Order Management
- Warehouse Management
- Transportation Management
- Fulfillment
- Shipping
- Webhooks
- Route Optimization
---
