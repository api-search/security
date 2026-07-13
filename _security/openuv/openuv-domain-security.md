---
api_specs:
- filename: openuv-openapi.yml
  format: yaml
  label: OpenUV
  slug: openuv
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openuv/refs/heads/main/openapi/openuv-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openuv.io
  spf: true
hosts:
- cert_expires: Aug 18 23:32:42 2026 GMT
  host: www.openuv.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:51:22 2026 GMT
  host: api.openuv.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openuv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenUV, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenUV
provider_slug: openuv
slug: openuv-domain-security
source_filename: openuv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openuv.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:32:42 2026 GMT\n  hsts: false\n- host: api.openuv.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:51:22 2026 GMT\n  hsts: null\ndomains:\n- domain: openuv.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openuv/refs/heads/main/security/openuv-domain-security.yml
summary_line: TLSv1.3
tags:
- Weather
- UV Index
- Sun
- Solar
- Geolocation
- Forecast
- Public APIs
---
