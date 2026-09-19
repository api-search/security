---
api_specs:
- filename: agl-agltosupplier-api-openapi.yml
  format: yaml
  label: AGL AGL To Supplier API
  slug: agl-agltosupplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-agltosupplier-api-openapi.yml
- filename: agl-codes-api-openapi.yml
  format: yaml
  label: AGL Codes API
  slug: agl-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-codes-api-openapi.yml
- filename: agl-golf-clubs-api-openapi.yml
  format: yaml
  label: AGL Golf Clubs API
  slug: agl-golf-clubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-golf-clubs-api-openapi.yml
- filename: agl-reservation-api-openapi.yml
  format: yaml
  label: AGL Reservation API
  slug: agl-reservation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-reservation-api-openapi.yml
- filename: agl-reservations-api-openapi.yml
  format: yaml
  label: AGL Reservations API
  slug: agl-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-reservations-api-openapi.yml
- filename: agl-static-packages-api-openapi.yml
  format: yaml
  label: AGL Static Packages API
  slug: agl-static-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-static-packages-api-openapi.yml
- filename: agl-suppliertoagl-api-openapi.yml
  format: yaml
  label: AGL Supplier To AGL API
  slug: agl-suppliertoagl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-suppliertoagl-api-openapi.yml
- filename: agl-tee-times-api-openapi.yml
  format: yaml
  label: AGL Tee Times API
  slug: agl-tee-times-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/openapi/agl-tee-times-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aglgw.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tigergds.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.aglgw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 13:33:21 2026 GMT
  host: api-doc.tigergds.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: gw-ota.tigergds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AGL, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AGL
provider_slug: agl
slug: agl-domain-security
source_filename: agl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aglgw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n- host: api-doc.tigergds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 13:33:21 2026 GMT\n  hsts: false\n- host: gw-ota.tigergds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aglgw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tigergds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agl/refs/heads/main/security/agl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Golf
- Travel
- Booking
- Reservations
- Distribution
- Tee Times
- GDS
- Hospitality
- Sports
- Leisure
- South Korea
---
