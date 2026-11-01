---
api_specs:
- filename: apizone-io-status-api-openapi.yml
  format: yaml
  label: apizone-io Status API
  slug: apizone-io-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apizone-io/openapi/apizone-io-status-api-openapi.yml
- filename: apizone-io-uptime-api-openapi.yml
  format: yaml
  label: apizone-io Uptime API
  slug: apizone-io-uptime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apizone-io/openapi/apizone-io-uptime-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: apizone.io
  spf: false
hosts:
- cert_expires: Jan 17 02:51:05 2027 GMT
  host: apizone.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apizone Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apizone-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: apizone-io
provider_slug: apizone-io
slug: apizone-io-domain-security
source_filename: apizone-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apizone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 02:51:05 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apizone.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/apizone-io/security/apizone-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Monitoring
- Status
- Uptime
- Developer Tools
- MCP
---
