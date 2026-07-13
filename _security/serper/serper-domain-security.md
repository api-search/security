---
api_specs:
- filename: serper-google-search-api-openapi.yml
  format: yaml
  label: Serper Google Search API
  slug: google-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-google-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: serper.dev
  spf: true
hosts:
- cert_expires: Aug 30 16:07:43 2026 GMT
  host: serper.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:17:02 2026 GMT
  host: google.serper.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serper, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Serper
provider_slug: serper
slug: serper-domain-security
source_filename: serper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: serper.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 16:07:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: google.serper.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:17:02 2026 GMT\n  hsts: null\ndomains:\n- domain: serper.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/security/serper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- SERP
- Google Search
- AI
- LLM
- SEO
- Images
- News
- Maps
- Shopping
---
