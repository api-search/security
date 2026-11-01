---
api_specs:
- filename: transcapi-airports-api-openapi.yml
  format: yaml
  label: TransCAPI Airports API
  slug: transcapi-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-airports-api-openapi.yml
- filename: transcapi-alerts-api-openapi.yml
  format: yaml
  label: TransCAPI Alerts API
  slug: transcapi-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-alerts-api-openapi.yml
- filename: transcapi-bus-api-openapi.yml
  format: yaml
  label: TransCAPI Bus API
  slug: transcapi-bus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-bus-api-openapi.yml
- filename: transcapi-disruptions-api-openapi.yml
  format: yaml
  label: TransCAPI Disruptions API
  slug: transcapi-disruptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-disruptions-api-openapi.yml
- filename: transcapi-journey-api-openapi.yml
  format: yaml
  label: TransCAPI Journey API
  slug: transcapi-journey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-journey-api-openapi.yml
- filename: transcapi-places-api-openapi.yml
  format: yaml
  label: TransCAPI Places API
  slug: transcapi-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-places-api-openapi.yml
- filename: transcapi-rail-api-openapi.yml
  format: yaml
  label: TransCAPI Rail API
  slug: transcapi-rail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcapi/openapi/transcapi-rail-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: transcapi.com
  spf: true
hosts:
- cert_expires: Dec 26 04:58:16 2026 GMT
  host: www.transcapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Transcapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TransCAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TransCAPI
provider_slug: transcapi
slug: transcapi-domain-security
source_filename: transcapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transcapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 04:58:16 2026 GMT\n  hsts: false\ndomains:\n- domain: transcapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/transcapi/security/transcapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Transport
- API
- UK
- Ireland
---
