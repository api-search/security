---
api_specs:
- filename: open-trivia-db-openapi.yml
  format: yaml
  label: Open Trivia DB
  slug: open-trivia-db
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-trivia-db/refs/heads/main/openapi/open-trivia-db-openapi.yml
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
name: Open Trivia Db Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Trivia DB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Trivia DB
provider_slug: open-trivia-db
slug: open-trivia-db-domain-security
source_filename: open-trivia-db-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 10:32:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opentdb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-trivia-db/refs/heads/main/security/open-trivia-db-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Free
- Games
- Questions
- Trivia
---
