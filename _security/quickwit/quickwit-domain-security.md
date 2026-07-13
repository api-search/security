---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Quickwit REST API
  slug: quickwit-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quickwit/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quickwit.io
  spf: false
hosts:
- cert_expires: Sep 16 17:07:23 2026 GMT
  host: quickwit.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quickwit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quickwit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Quickwit
provider_slug: quickwit
slug: quickwit-domain-security
source_filename: quickwit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quickwit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 17:07:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: quickwit.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quickwit/refs/heads/main/security/quickwit-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Search
- Log Management
- Observability
- Full-Text Search
- Cloud Native
- Open Source
- Distributed Tracing
- Analytics
---
