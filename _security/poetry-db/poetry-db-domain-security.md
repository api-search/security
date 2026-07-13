---
api_specs:
- filename: openapi.yml
  format: yaml
  label: PoetryDB API
  slug: poetry-db
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poetry-db/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: poetrydb.org
  spf: false
hosts:
- cert_expires: Sep  9 00:38:35 2026 GMT
  host: poetrydb.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poetry Db Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PoetryDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PoetryDB
provider_slug: poetry-db
slug: poetry-db-domain-security
source_filename: poetry-db-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poetrydb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:38:35 2026 GMT\n  hsts: false\ndomains:\n- domain: poetrydb.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poetry-db/refs/heads/main/security/poetry-db-domain-security.yml
summary_line: TLSv1.3
tags:
- Poetry
- Literature
- Public Domain
- English Language
- Search
- Open Data
---
