---
api_specs:
- filename: httpstat-httpstat-api-openapi.yml
  format: yaml
  label: Httpstat.us Httpstat API
  slug: httpstat-httpstat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/httpstat/refs/heads/main/openapi/httpstat-httpstat-api-openapi.yml
- filename: httpstat-random-api-openapi.yml
  format: yaml
  label: Httpstat.us Random API
  slug: httpstat-random-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/httpstat/refs/heads/main/openapi/httpstat-random-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: httpstat.us
  spf: false
hosts:
- cert_expires: Sep 22 01:39:21 2026 GMT
  host: httpstat.us
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Httpstat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Httpstat.us, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Httpstat.us
provider_slug: httpstat
slug: httpstat-domain-security
source_filename: httpstat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: httpstat.us\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 01:39:21 2026 GMT\n  hsts: null\ndomains:\n- domain: httpstat.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/httpstat/refs/heads/main/security/httpstat-domain-security.yml
summary_line: TLSv1.2
tags:
- HTTP
- Status Codes
- Testing
- Utilities
---
