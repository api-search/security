---
api_specs:
- filename: open-trivia-openapi.yml
  format: yaml
  label: Open Trivia Database API
  slug: open-trivia-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-trivia/refs/heads/main/openapi/open-trivia-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opentdb.com
  spf: false
hosts:
- cert_expires: Aug 27 10:32:56 2026 GMT
  host: opentdb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Trivia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Trivia Database, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Trivia Database
provider_slug: open-trivia
slug: open-trivia-domain-security
source_filename: open-trivia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 10:32:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opentdb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-trivia/refs/heads/main/security/open-trivia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Trivia
- Games And Comics
- Quiz
- Open Data
- Public APIs
- Open Source
---
