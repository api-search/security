---
api_specs:
- filename: wordnik-openapi.yml
  format: yaml
  label: Wordnik
  slug: wordnik
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordnik/refs/heads/main/openapi/wordnik-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wordnik.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: wordnik.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: developer.wordnik.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: api.wordnik.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wordnik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wordnik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wordnik
provider_slug: wordnik
slug: wordnik-domain-security
source_filename: wordnik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wordnik.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.wordnik.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.wordnik.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wordnik.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordnik/refs/heads/main/security/wordnik-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Dictionaries
- Dictionary
- Word Data
- English
- Lexicography
- Public APIs
---
