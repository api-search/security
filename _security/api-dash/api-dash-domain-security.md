---
api_specs:
- filename: api-dash-api-dash-apis-api-openapi.yml
  format: yaml
  label: API Dash API Dash APIs API
  slug: api-dash-api-dash-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-api-dash-apis-api-openapi.yml
- filename: api-dash-case-conversion-api-openapi.yml
  format: yaml
  label: API Dash Case Conversion API
  slug: api-dash-case-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-case-conversion-api-openapi.yml
- filename: api-dash-country-data-api-openapi.yml
  format: yaml
  label: API Dash Country Data API
  slug: api-dash-country-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-country-data-api-openapi.yml
- filename: api-dash-humanize-api-openapi.yml
  format: yaml
  label: API Dash Humanize API
  slug: api-dash-humanize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-humanize-api-openapi.yml
- filename: api-dash-i-o-api-openapi.yml
  format: yaml
  label: API Dash I/O API
  slug: api-dash-i-o-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-i-o-api-openapi.yml
- filename: api-dash-sse-api-openapi.yml
  format: yaml
  label: API Dash SSE API
  slug: api-dash-sse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-sse-api-openapi.yml
- filename: api-dash-text-conversion-api-openapi.yml
  format: yaml
  label: API Dash Text Conversion API
  slug: api-dash-text-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-text-conversion-api-openapi.yml
- filename: api-dash-user-authentication-api-openapi.yml
  format: yaml
  label: API Dash User Authentication API
  slug: api-dash-user-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-user-authentication-api-openapi.yml
- filename: api-dash-user-data-api-openapi.yml
  format: yaml
  label: API Dash User Data API
  slug: api-dash-user-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-user-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apidash.dev
  spf: true
hosts:
- cert_expires: Oct 17 23:02:46 2026 GMT
  host: apidash.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:02:46 2026 GMT
  host: api.apidash.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Api Dash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Dash, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: API Dash
provider_slug: api-dash
slug: api-dash-domain-security
source_filename: api-dash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidash.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:02:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.apidash.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:02:46 2026 GMT\n  hsts: null\ndomains:\n- domain: apidash.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/security/api-dash-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Client
- Open-Source
- Flutter
- Desktop
- Mobile
---
