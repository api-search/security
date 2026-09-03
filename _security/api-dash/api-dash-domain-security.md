---
api_specs:
- filename: api-dash-openapi.yml
  format: yaml
  label: API Dash
  slug: api-dash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-openapi.yml
- filename: api-dash-openapi.yml
  format: yaml
  label: API Dash APIs
  slug: api-dash-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-dash/refs/heads/main/openapi/api-dash-openapi.yml
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
