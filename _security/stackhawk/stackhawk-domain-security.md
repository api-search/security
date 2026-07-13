---
api_specs:
- filename: stackhawk-openapi.json
  format: json
  label: StackHawk API
  slug: stackhawk-api
  spec_type: OpenAPI
  url: https://download.stackhawk.com/openapi/stackhawk-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackhawk.com
  spf: true
hosts:
- cert_expires: Oct  4 02:36:05 2026 GMT
  host: www.stackhawk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 19:55:18 2026 GMT
  host: apidocs.stackhawk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: api.stackhawk.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stackhawk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackHawk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StackHawk
provider_slug: stackhawk
slug: stackhawk-domain-security
source_filename: stackhawk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stackhawk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:36:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.stackhawk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:55:18 2026 GMT\n  hsts: null\n- host: api.stackhawk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stackhawk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/security/stackhawk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Security
- Application Security
- DAST
- Security Testing
- Vulnerability Management
---
