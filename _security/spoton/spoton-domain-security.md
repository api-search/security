---
api_specs:
- filename: spoton-restaurant-pos-export-openapi-original.yml
  format: yaml
  label: SpotOn Restaurant POS Export API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-restaurant-pos-export-openapi-original.yml
- filename: spoton-reserve-openapi-original.yml
  format: yaml
  label: SpotOn Reserve API
  slug: reserve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/openapi/spoton-reserve-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spoton.com
  spf: true
hosts:
- cert_expires: Oct  9 08:35:21 2026 GMT
  host: www.spoton.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 00:11:09 2026 GMT
  host: developers.spoton.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: restaurantapi.spoton.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spoton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpotOn, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SpotOn
provider_slug: spoton
slug: spoton-domain-security
source_filename: spoton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spoton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:35:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.spoton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:11:09 2026 GMT\n  hsts: null\n- host: restaurantapi.spoton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: spoton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spoton/refs/heads/main/security/spoton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Point of Sale
- Payments
- Online Ordering
- Reservations
- Reporting
---
