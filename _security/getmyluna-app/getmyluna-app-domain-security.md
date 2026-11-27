---
api_specs:
- filename: getmyluna-app-account-api-openapi.yml
  format: yaml
  label: Luna Account API
  slug: getmyluna-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-account-api-openapi.yml
- filename: getmyluna-app-analytics-api-openapi.yml
  format: yaml
  label: Luna Analytics API
  slug: getmyluna-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-analytics-api-openapi.yml
- filename: getmyluna-app-ask-luna-api-openapi.yml
  format: yaml
  label: Luna Ask Luna API
  slug: getmyluna-app-ask-luna-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-ask-luna-api-openapi.yml
- filename: getmyluna-app-discovery-api-openapi.yml
  format: yaml
  label: Luna Discovery API
  slug: getmyluna-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-discovery-api-openapi.yml
- filename: getmyluna-app-insights-api-openapi.yml
  format: yaml
  label: Luna Insights API
  slug: getmyluna-app-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-insights-api-openapi.yml
- filename: getmyluna-app-profile-api-openapi.yml
  format: yaml
  label: Luna Profile API
  slug: getmyluna-app-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-profile-api-openapi.yml
- filename: getmyluna-app-tokens-api-openapi.yml
  format: yaml
  label: Luna Tokens API
  slug: getmyluna-app-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-tokens-api-openapi.yml
- filename: getmyluna-app-tracker-api-openapi.yml
  format: yaml
  label: Luna Tracker API
  slug: getmyluna-app-tracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getmyluna-app/openapi/getmyluna-app-tracker-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getmyluna.app
  spf: true
hosts:
- cert_expires: Dec 26 12:12:26 2026 GMT
  host: getmyluna.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Luna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Luna
provider_slug: getmyluna-app
slug: getmyluna-app-domain-security
source_filename: getmyluna-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getmyluna.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 12:12:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getmyluna.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getmyluna-app/security/getmyluna-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Baby Tracker
- Shared Log
- Health Tracking
- Family Care
---
