---
api_specs:
- filename: httpie-httpie-openapi.yml
  format: yaml
  label: HTTPie
  slug: httpie
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/httpie/refs/heads/main/openapi/httpie-httpie-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: httpie.io
  spf: true
hosts:
- cert_expires: Sep 11 04:21:37 2026 GMT
  host: httpie.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Httpie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTTPie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HTTPie
provider_slug: httpie
slug: httpie-domain-security
source_filename: httpie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: httpie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:21:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: httpie.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/httpie/refs/heads/main/security/httpie-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Client
- API Testing
- CLI
- Client
- Command Line
- Developer Tools
- HTTP
- Open Source
- Sessions
---
