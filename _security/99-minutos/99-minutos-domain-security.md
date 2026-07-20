---
api_specs:
- filename: 99minutos-api-v3-openapi.json
  format: json
  label: 99minutos API v3
  slug: 99minutos-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/openapi/99minutos-api-v3-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 99minutos.com
  spf: true
hosts:
- cert_expires: Oct 12 16:00:02 2026 GMT
  host: 99minutos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 20:20:14 2026 GMT
  host: delivery.99minutos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 03:07:28 2026 GMT
  host: sandbox.99minutos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 99 Minutos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 99 Minutos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 99 Minutos
provider_slug: 99-minutos
slug: 99-minutos-domain-security
source_filename: 99-minutos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 99minutos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 16:00:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: delivery.99minutos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:20:14 2026 GMT\n  hsts: false\n- host: sandbox.99minutos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 03:07:28 2026 GMT\n  hsts: false\ndomains:\n- domain: 99minutos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99-minutos/refs/heads/main/security/99-minutos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Last Mile Delivery
- Shipping
- Ecommerce
- Fulfillment
- Freight
- Tracking
- Webhooks
- Latin America
- Mexico
---
