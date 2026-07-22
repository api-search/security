---
api_specs:
- filename: metrobi-delivery-api-openapi.json
  format: json
  label: Metrobi Delivery API
  slug: metrobi-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrobi/refs/heads/main/openapi/metrobi-delivery-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: metrobi.com
  spf: true
hosts:
- cert_expires: Oct 15 20:12:27 2026 GMT
  host: metrobi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: delivery-api.metrobi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Metrobi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metrobi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Metrobi
provider_slug: metrobi
slug: metrobi-domain-security
source_filename: metrobi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metrobi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 20:12:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: delivery-api.metrobi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: metrobi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metrobi/refs/heads/main/security/metrobi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Delivery
- Logistics
- Courier
- Last Mile Delivery
- Route Optimization
- Fulfillment
- Local Delivery
- Webhooks
---
