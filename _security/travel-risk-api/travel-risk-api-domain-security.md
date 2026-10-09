---
api_specs:
- filename: travel-risk-api-adb-api-openapi.yml
  format: yaml
  label: Travel Risk API Adb API
  slug: travel-risk-api-adb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-adb-api-openapi.yml
- filename: travel-risk-api-auth-api-openapi.yml
  format: yaml
  label: Travel Risk API Auth API
  slug: travel-risk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-auth-api-openapi.yml
- filename: travel-risk-api-billing-api-openapi.yml
  format: yaml
  label: Travel Risk API Billing API
  slug: travel-risk-api-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-billing-api-openapi.yml
- filename: travel-risk-api-ext-api-openapi.yml
  format: yaml
  label: Travel Risk API Ext API
  slug: travel-risk-api-ext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-ext-api-openapi.yml
- filename: travel-risk-api-public-data-api-openapi.yml
  format: yaml
  label: Travel Risk API Public Data API
  slug: travel-risk-api-public-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-public-data-api-openapi.yml
- filename: travel-risk-api-system-api-openapi.yml
  format: yaml
  label: Travel Risk API System API
  slug: travel-risk-api-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-system-api-openapi.yml
- filename: travel-risk-api-usage-api-openapi.yml
  format: yaml
  label: Travel Risk API Usage API
  slug: travel-risk-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: travelriskapi.com
  spf: true
hosts:
- cert_expires: Jan  6 20:12:34 2027 GMT
  host: travelriskapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Travel Risk Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Travel Risk API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Travel Risk API
provider_slug: travel-risk-api
slug: travel-risk-api-domain-security
source_filename: travel-risk-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: travelriskapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 20:12:34 2027 GMT\n  hsts: null\ndomains:\n- domain: travelriskapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/security/travel-risk-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Travel Risk
- Travel Advisories
- Aviation
- Airports
- Risk Scoring
- Safety
- Disaster Alerts
---
