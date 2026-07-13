---
api_specs:
- filename: tibber-graphql-api-openapi.yml
  format: yaml
  label: Tibber GraphQL API
  slug: tibber-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/openapi/tibber-graphql-api-openapi.yml
- filename: tibber-data-api-openapi.yml
  format: yaml
  label: Tibber Data API
  slug: tibber-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/openapi/tibber-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tibber.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: tibber.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: developer.tibber.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.tibber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tibber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tibber, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tibber
provider_slug: tibber
slug: tibber-domain-security
source_filename: tibber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tibber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tibber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\n- host: api.tibber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tibber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tibber/refs/heads/main/security/tibber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- SmartHome
- SmartMeter
- ElectricityPricing
- ElectricVehicleCharging
- HeatPump
- SolarInverter
- HomeBattery
- GraphQL
- OAuth2
- Nordic
---
