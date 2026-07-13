---
api_specs:
- filename: words-openapi.yml
  format: yaml
  label: Words API
  slug: words-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wordsapi.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Oct  4 21:58:58 2026 GMT
  host: www.wordsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: wordsapiv1.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Words Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Words API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Words API
provider_slug: words
slug: words-domain-security
source_filename: words-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wordsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:58:58 2026 GMT\n  hsts: false\n- host: wordsapiv1.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wordsapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/security/words-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Dictionaries
- Linguistics
- English
- Thesaurus
- Lexical Data
- Public APIs
---
