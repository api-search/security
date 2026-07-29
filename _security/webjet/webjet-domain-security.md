---
api_specs:
- filename: webjet-tripninja-smartflights-get-searches-openapi.yml
  format: yaml
  label: Trip Ninja SmartFlights API
  slug: tripninja-smartflights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-smartflights-get-searches-openapi.yml
- filename: webjet-tripninja-adminpanel-refresh-token-openapi.yml
  format: yaml
  label: Trip Ninja Admin Panel API
  slug: tripninja-admin-panel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-adminpanel-refresh-token-openapi.yml
- filename: webjet-tripninja-farestructure-get-searches-openapi.yml
  format: yaml
  label: Trip Ninja FareStructure API (deprecated)
  slug: tripninja-farestructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-farestructure-get-searches-openapi.yml
- filename: webjet-tripninja-virtual-interlining-get-searches-openapi.yml
  format: yaml
  label: Trip Ninja Virtual Interlining API (deprecated)
  slug: tripninja-virtual-interlining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-virtual-interlining-get-searches-openapi.yml
- filename: 20885222-5fccfe6e-479a-429f-a497-d42a0bb859c9
  format: yaml
  label: Trip Ninja DataStream API
  slug: tripninja-datastream-api
  spec_type: Postman
  url: https://www.postman.com/tripninjadevteam/workspace/trip-ninja-public/collection/20885222-5fccfe6e-479a-429f-a497-d42a0bb859c9
- filename: webjet-tripninja-flights-core-openapi.yml
  format: yaml
  label: Trip Ninja Flights Core API
  slug: tripninja-flights-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-flights-core-openapi.yml
- filename: webjet-tripninja-pricing-booking-openapi.yml
  format: yaml
  label: Trip Ninja Pricing & Booking API
  slug: tripninja-pricing-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-pricing-booking-openapi.yml
- filename: webjet-tripninja-hotels-openapi.yml
  format: yaml
  label: Trip Ninja Hotels API
  slug: tripninja-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-hotels-openapi.yml
- filename: webjet-tripninja-msdp-openapi.yml
  format: yaml
  label: Trip Ninja MSDP (Dynamic Packaging) API
  slug: tripninja-msdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-msdp-openapi.yml
- filename: webjet-tripninja-v2-core-openapi.yml
  format: yaml
  label: Trip Ninja v2 Legacy API
  slug: tripninja-v2-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-v2-core-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webjetgroup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tripninja.io
  spf: true
hosts:
- cert_expires: Sep 28 11:46:10 2026 GMT
  host: www.webjetgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: app.tripninja.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 17:42:09 2026 GMT
  host: www.tripninja.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Webjet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webjet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Webjet
provider_slug: webjet
slug: webjet-domain-security
source_filename: webjet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.webjetgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:46:10 2026 GMT\n  hsts: false\n- host: app.tripninja.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\n- host: www.tripninja.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 17:42:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: webjetgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tripninja.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/security/webjet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Australia
- OTA
- Aviation
- Booking
- Distribution
- Flight Search
- Car Rental
- New Zealand
- Travel Technology
---
