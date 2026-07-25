---
api_specs:
- filename: parade-available-trucks-api-openapi.yml
  format: yaml
  label: Parade Available Trucks API
  slug: parade-available-trucks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-available-trucks-api-openapi.yml
- filename: parade-bookings-api-openapi.yml
  format: yaml
  label: Parade Bookings API
  slug: parade-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-bookings-api-openapi.yml
- filename: parade-carrier-onboarding-status-api-openapi.yml
  format: yaml
  label: Parade Carrier Onboarding Status API
  slug: parade-carrier-onboarding-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-carrier-onboarding-status-api-openapi.yml
- filename: parade-carrier-synchronization-api-openapi.yml
  format: yaml
  label: Parade Carrier Synchronization API
  slug: parade-carrier-synchronization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-carrier-synchronization-api-openapi.yml
- filename: parade-digital-conversion-api-openapi.yml
  format: yaml
  label: Parade Digital Conversion API
  slug: parade-digital-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-digital-conversion-api-openapi.yml
- filename: parade-load-synchronization-api-openapi.yml
  format: yaml
  label: Parade Load Synchronization API
  slug: parade-load-synchronization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-load-synchronization-api-openapi.yml
- filename: parade-quotes-api-openapi.yml
  format: yaml
  label: Parade Quotes API
  slug: parade-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-quotes-api-openapi.yml
- filename: parade-search-api-openapi.yml
  format: yaml
  label: Parade Search API
  slug: parade-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parade.ai
  spf: true
hosts:
- cert_expires: Sep 25 23:53:34 2026 GMT
  host: parade.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 11:21:37 2026 GMT
  host: api.capacity.stage.parade.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 15:09:01 2026 GMT
  host: api.syndication.stage.parade.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Parade
provider_slug: parade
slug: parade-domain-security
source_filename: parade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parade.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:53:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.capacity.stage.parade.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:21:37 2026 GMT\n  hsts: false\n- host: api.syndication.stage.parade.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 15:09:01 2026 GMT\n  hsts: null\ndomains:\n- domain: parade.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/security/parade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Freight
- Logistics
- Trucking
- Supply Chain
- Capacity Management
- Freight Brokerage
- Transportation
- Load Board
- Artificial Intelligence
---
