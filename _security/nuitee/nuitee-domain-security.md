---
api_specs:
- filename: nuitee-booking-api-openapi.yml
  format: yaml
  label: Nuitée (LiteAPI) Booking API
  slug: nuitee-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-booking-api-openapi.yml
- filename: nuitee-hotel-data-api-openapi.yml
  format: yaml
  label: Nuitée (LiteAPI) Hotel Data API
  slug: nuitee-hotel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-hotel-data-api-openapi.yml
- filename: nuitee-loyalty-api-openapi.yml
  format: yaml
  label: Nuitée (LiteAPI) Loyalty API
  slug: nuitee-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-loyalty-api-openapi.yml
- filename: nuitee-rates-api-openapi.yml
  format: yaml
  label: Nuitée (LiteAPI) Rates API
  slug: nuitee-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-rates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liteapi.travel
  spf: false
hosts:
- cert_expires: Aug 23 06:05:26 2026 GMT
  host: www.liteapi.travel
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 22:16:54 2026 GMT
  host: docs.liteapi.travel
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 18:21:42 2026 GMT
  host: api.liteapi.travel
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuitee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuitée (LiteAPI), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Nuitée (LiteAPI)
provider_slug: nuitee
slug: nuitee-domain-security
source_filename: nuitee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liteapi.travel\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:05:26 2026 GMT\n  hsts: false\n- host: docs.liteapi.travel\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:16:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.liteapi.travel\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:21:42 2026 GMT\n  hsts: null\ndomains:\n- domain: liteapi.travel\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/security/nuitee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Hotels
- Booking
- Distribution
- Hospitality
---
