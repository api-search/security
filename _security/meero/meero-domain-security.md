---
api_specs:
- filename: meero-asynchronous-api-openapi.yml
  format: yaml
  label: Meero Asynchronous API
  slug: meero-asynchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-asynchronous-api-openapi.yml
- filename: meero-feature-api-openapi.yml
  format: yaml
  label: Meero Feature API
  slug: meero-feature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-feature-api-openapi.yml
- filename: meero-synchronous-api-openapi.yml
  format: yaml
  label: Meero Synchronous API
  slug: meero-synchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-synchronous-api-openapi.yml
- filename: meero-vehicle-api-openapi.yml
  format: yaml
  label: Meero Vehicle API
  slug: meero-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-vehicle-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carcutter.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: car-cutter.com
  spf: true
hosts:
- cert_expires: Nov 10 21:46:54 2026 GMT
  host: www.carcutter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: cloud.car-cutter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.car-cutter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meero, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meero
provider_slug: meero
slug: meero-domain-security
source_filename: meero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carcutter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 21:46:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.car-cutter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\n- host: api.car-cutter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: carcutter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: car-cutter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/security/meero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Images
- Artificial Intelligence
- Computer Vision
- Photography
- Media Processing
- E-Commerce
- Vehicle Merchandising
- Company
---
