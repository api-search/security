---
api_specs:
- filename: trieve-openapi.yml
  format: yaml
  label: Trieve REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trieve/refs/heads/main/openapi/trieve-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trieve.ai
  spf: true
hosts:
- host: trieve.ai
  https: false
- cert_expires: Sep 14 19:33:50 2026 GMT
  host: docs.trieve.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.trieve.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Trieve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trieve, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trieve
provider_slug: trieve
slug: trieve-domain-security
source_filename: trieve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trieve.ai\n  https: false\n- host: docs.trieve.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.trieve.ai\n  https: false\ndomains:\n- domain: trieve.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trieve/refs/heads/main/security/trieve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- RAG
- Vector Search
- Hybrid Search
- Recommendations
- Analytics
- Open Source
---
