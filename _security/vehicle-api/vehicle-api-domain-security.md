---
api_specs:
- filename: vehicle-api-inventory-api-openapi.yml
  format: yaml
  label: Vehicle API Inventory API
  slug: vehicle-api-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-inventory-api-openapi.yml
- filename: vehicle-api-makes-api-openapi.yml
  format: yaml
  label: Vehicle API Makes API
  slug: vehicle-api-makes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-makes-api-openapi.yml
- filename: vehicle-api-media-api-openapi.yml
  format: yaml
  label: Vehicle API Media API
  slug: vehicle-api-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-media-api-openapi.yml
- filename: vehicle-api-models-api-openapi.yml
  format: yaml
  label: Vehicle API Models API
  slug: vehicle-api-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-models-api-openapi.yml
- filename: vehicle-api-pricing-api-openapi.yml
  format: yaml
  label: Vehicle API Pricing API
  slug: vehicle-api-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-pricing-api-openapi.yml
- filename: vehicle-api-specs-api-openapi.yml
  format: yaml
  label: Vehicle API Specs API
  slug: vehicle-api-specs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-specs-api-openapi.yml
- filename: vehicle-api-styles-api-openapi.yml
  format: yaml
  label: Vehicle API Styles API
  slug: vehicle-api-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/openapi/vehicle-api-styles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edmunds.com
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: developer.edmunds.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: api.edmunds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vehicle Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vehicle API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vehicle API
provider_slug: vehicle-api
slug: vehicle-api-domain-security
source_filename: vehicle-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.edmunds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.edmunds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: edmunds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vehicle-api/refs/heads/main/security/vehicle-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Cars
- Edmunds
- Pricing
- Vehicles
---
