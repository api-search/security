---
api_specs:
- filename: noyo-fulfillment-openapi.json
  format: json
  label: Noyo Fulfillment API
  slug: noyo-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noyo/refs/heads/main/openapi/noyo-fulfillment-openapi.json
- filename: noyo-tracking-openapi.json
  format: json
  label: Noyo Tracking API
  slug: noyo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noyo/refs/heads/main/openapi/noyo-tracking-openapi.json
- filename: noyo-carrier-openapi.json
  format: json
  label: Noyo Carrier API
  slug: noyo-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noyo/refs/heads/main/openapi/noyo-carrier-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: noyo.com
  spf: true
hosts:
- cert_expires: Sep 21 03:08:40 2026 GMT
  host: www.noyo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 04:04:32 2026 GMT
  host: docs.noyo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:20:45 2026 GMT
  host: fulfillment.noyo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noyo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noyo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Noyo
provider_slug: noyo
slug: noyo-domain-security
source_filename: noyo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:08:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.noyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:04:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: fulfillment.noyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:20:45 2026 GMT\n  hsts: null\ndomains:\n- domain: noyo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noyo/refs/heads/main/security/noyo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Insurance
- Employee Benefits
- Enrollment
- Benefits Administration
- Insurance Carriers
- Data Exchange
- Webhooks
- Health Insurance
---
