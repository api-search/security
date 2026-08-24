---
api_specs:
- filename: kontaktio-device-management-openapi.yml
  format: yaml
  label: Kontakt.io Device Management API
  slug: kontaktio-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-device-management-openapi.yml
- filename: kontaktio-location-occupancy-openapi.yml
  format: yaml
  label: Kontakt.io Location & Occupancy API
  slug: kontaktio-location-occupancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-location-occupancy-openapi.yml
- filename: kontaktio-spaces-openapi.yml
  format: yaml
  label: Kontakt.io Spaces API
  slug: kontaktio-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-spaces-openapi.yml
- filename: kontaktio-entity-management-openapi.yml
  format: yaml
  label: Kontakt.io Entity Management Integration API
  slug: kontaktio-entity-management-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-entity-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kontakt.io
  spf: true
hosts:
- cert_expires: Nov 11 18:38:35 2026 GMT
  host: kontakt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 04:14:07 2026 GMT
  host: developer.kontakt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: dm-api.cloud.us.kontakt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kontaktio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kontakt.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kontakt.io
provider_slug: kontaktio
slug: kontaktio-domain-security
source_filename: kontaktio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kontakt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 18:38:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.kontakt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 04:14:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dm-api.cloud.us.kontakt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: kontakt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/security/kontaktio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IoT
- RTLS
- Healthcare
- Asset Tracking
- Location
- Occupancy
- Bluetooth
- Device Management
- Telemetry
- Sensors
- Streaming
---
