---
api_specs:
- filename: astronomy-api-openapi.yml
  format: yaml
  label: Astronomy API
  slug: astronomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/openapi/astronomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: astronomyapi.com
  spf: false
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: astronomyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 00:41:56 2026 GMT
  host: docs.astronomyapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.astronomyapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astronomy Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astronomy API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Astronomy API
provider_slug: astronomy-api
slug: astronomy-api-domain-security
source_filename: astronomy-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astronomyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\n- host: docs.astronomyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:41:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.astronomyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: astronomyapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/security/astronomy-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Astronomy
- Celestial Data
- Space
- Moon Phases
- Star Charts
---
