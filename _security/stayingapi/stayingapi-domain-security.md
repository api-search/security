---
api_specs:
- filename: stayingapi-account-api-openapi.yml
  format: yaml
  label: StayingAPI Account API
  slug: stayingapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-account-api-openapi.yml
- filename: stayingapi-data-api-openapi.yml
  format: yaml
  label: StayingAPI Data API
  slug: stayingapi-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-data-api-openapi.yml
- filename: stayingapi-jobs-api-openapi.yml
  format: yaml
  label: StayingAPI Jobs API
  slug: stayingapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/openapi/stayingapi-jobs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stayingapi.com
  spf: false
hosts:
- cert_expires: Oct 18 12:53:44 2026 GMT
  host: stayingapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 12:53:44 2026 GMT
  host: api.stayingapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 12:53:44 2026 GMT
  host: mcp.stayingapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stayingapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StayingAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: StayingAPI
provider_slug: stayingapi
slug: stayingapi-domain-security
source_filename: stayingapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stayingapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:53:44 2026 GMT\n  hsts: false\n- host: api.stayingapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:53:44 2026 GMT\n  hsts: null\n- host: mcp.stayingapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:53:44 2026 GMT\n  hsts: null\ndomains:\n- domain: stayingapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stayingapi/refs/heads/main/security/stayingapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Hospitality
- accommodation-data
- hotel-api
- Vacation Rental
- Short-Term Rental
- Airbnb
- Booking.com
- Vrbo
- google-hotels
- cross-ota-price-comparison
- Availability
- Reviews
- REST
- MCP
- agent-native
- OpenAPI
---
