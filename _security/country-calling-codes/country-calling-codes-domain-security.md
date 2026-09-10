---
api_specs:
- filename: openapi.json
  format: json
  label: Country Calling Codes API
  slug: country-calling-codes-api
  spec_type: OpenAPI
  url: https://www.countrycalling.codes/api/calling-codes/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: countrycalling.codes
  spf: false
hosts:
- cert_expires: Oct 20 08:00:19 2026 GMT
  host: www.countrycalling.codes
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Country Calling Codes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Country Calling Codes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Country Calling Codes
provider_slug: country-calling-codes
slug: country-calling-codes-domain-security
source_filename: country-calling-codes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.countrycalling.codes\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 08:00:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: countrycalling.codes\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/country-calling-codes/refs/heads/main/security/country-calling-codes-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- data
- reference
- telecom
- phone
- openapi
- mcp
---
