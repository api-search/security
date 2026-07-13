---
api_specs:
- filename: api-pulse-publish-openapi.yml
  format: yaml
  label: API Pulse Publish API
  slug: api-pulse-publish
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-pulse/refs/heads/main/openapi/api-pulse-publish-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theapipulse.com
  spf: false
hosts:
- cert_expires: Sep  4 06:05:16 2026 GMT
  host: theapipulse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 06:05:16 2026 GMT
  host: api.theapipulse.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Pulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Pulse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: API Pulse
provider_slug: api-pulse
slug: api-pulse-domain-security
source_filename: api-pulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theapipulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 06:05:16 2026 GMT\n  hsts: false\n- host: api.theapipulse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 06:05:16 2026 GMT\n  hsts: null\ndomains:\n- domain: theapipulse.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-pulse/refs/heads/main/security/api-pulse-domain-security.yml
summary_line: TLSv1.3
tags:
- API Benchmarking
- API Evangelist
- API Governance
- API Maturity
- Survey
---
