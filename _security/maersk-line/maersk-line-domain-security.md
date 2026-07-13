---
api_specs:
- filename: maersk-track-and-trace-api-openapi.yml
  format: yaml
  label: Maersk Track and Trace API
  slug: maersk-track-and-trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-track-and-trace-api-openapi.yml
- filename: maersk-ocean-booking-api-openapi.yml
  format: yaml
  label: Maersk Ocean Booking API
  slug: maersk-ocean-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-ocean-booking-api-openapi.yml
- filename: maersk-schedules-api-openapi.yml
  format: yaml
  label: Maersk Schedules API
  slug: maersk-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-schedules-api-openapi.yml
- filename: maersk-product-offers-api-openapi.yml
  format: yaml
  label: Maersk Product Offers API
  slug: maersk-product-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-product-offers-api-openapi.yml
- filename: maersk-bill-of-lading-api-openapi.yml
  format: yaml
  label: Maersk Bill of Lading API
  slug: maersk-bill-of-lading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-bill-of-lading-api-openapi.yml
- filename: maersk-vgm-api-openapi.yml
  format: yaml
  label: Maersk Verified Gross Mass API
  slug: maersk-vgm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-vgm-api-openapi.yml
- filename: maersk-demurrage-detention-api-openapi.yml
  format: yaml
  label: Maersk Import Demurrage and Detention API
  slug: maersk-demurrage-detention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-demurrage-detention-api-openapi.yml
- filename: maersk-air-booking-api-openapi.yml
  format: yaml
  label: Maersk Air Booking API
  slug: maersk-air-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-air-booking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maersk.com
  spf: true
hosts:
- cert_expires: Aug 28 02:24:27 2026 GMT
  host: developer.maersk.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 02:20:42 2026 GMT
  host: www.maersk.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- host: api.productmanagement.maersk.com
  https: false
kind: domain-security
layout: security
method: probed
name: Maersk Line Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maersk, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Maersk
provider_slug: maersk-line
slug: maersk-line-domain-security
source_filename: maersk-line-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.maersk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:24:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.maersk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:20:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.productmanagement.maersk.com\n  https: false\ndomains:\n- domain: maersk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/security/maersk-line-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Logistics
- Container Shipping
- Ocean Freight
- Air Freight
- Supply Chain
- DCSA
- Maritime
---
