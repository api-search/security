---
api_specs:
- filename: hotelbeds-activities-api-openapi.yml
  format: yaml
  label: Hotelbeds Activities API
  slug: hotelbeds-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-activities-api-openapi.yml
- filename: hotelbeds-booking-api-openapi.yml
  format: yaml
  label: Hotelbeds Booking API
  slug: hotelbeds-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-booking-api-openapi.yml
- filename: hotelbeds-cache-api-openapi.yml
  format: yaml
  label: Hotelbeds Cache API
  slug: hotelbeds-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-cache-api-openapi.yml
- filename: hotelbeds-content-api-openapi.yml
  format: yaml
  label: Hotelbeds Content API
  slug: hotelbeds-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-content-api-openapi.yml
- filename: hotelbeds-transfers-api-openapi.yml
  format: yaml
  label: Hotelbeds Transfers API
  slug: hotelbeds-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hotelbeds.com
  spf: true
hosts:
- cert_expires: Aug 24 14:14:42 2026 GMT
  host: www.hotelbeds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: developer.hotelbeds.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.hotelbeds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hotelbeds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hotelbeds, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hotelbeds
provider_slug: hotelbeds
slug: hotelbeds-domain-security
source_filename: hotelbeds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hotelbeds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:14:42 2026 GMT\n  hsts: null\n- host: developer.hotelbeds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.hotelbeds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hotelbeds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/security/hotelbeds-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Hotels
- Bedbank
- Accommodation
- Booking
---
