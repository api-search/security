---
api_specs:
- filename: dtn-weather-conditions-openapi.yml
  format: yaml
  label: DTN Weather Conditions API
  slug: dtn-weather-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dtn/refs/heads/main/openapi/dtn-weather-conditions-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dtn.com
  spf: true
hosts:
- cert_expires: Aug 20 07:42:07 2026 GMT
  host: www.dtn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: devportal.dtn.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: weather.api.dtn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dtn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dtn, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: dtn
provider_slug: dtn
slug: dtn-domain-security
source_filename: dtn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dtn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:42:07 2026 GMT\n  hsts: false\n- host: devportal.dtn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: weather.api.dtn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dtn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dtn/refs/heads/main/security/dtn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
