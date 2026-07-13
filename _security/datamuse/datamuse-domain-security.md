---
api_specs:
- filename: datamuse-openapi.yml
  format: yaml
  label: Datamuse API
  slug: datamuse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datamuse/refs/heads/main/openapi/datamuse-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datamuse.com
  spf: false
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.datamuse.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.datamuse.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datamuse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datamuse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Datamuse
provider_slug: datamuse
slug: datamuse-domain-security
source_filename: datamuse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datamuse.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.datamuse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: datamuse.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datamuse/refs/heads/main/security/datamuse-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Word Finding
- Lexical Search
- Natural Language
- Vocabulary
- Synonyms
- Antonyms
- Rhymes
- Phonetics
- Semantic Search
- Reverse Dictionary
- Autocomplete
- Wordplay
- Creative Writing
- Vocabulary Apps
- Word Games
- Linguistics
- Open Source Projects
- Public APIs
---
