---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Cat Facts API
  slug: cat-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catfact/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: catfact.ninja
  spf: true
hosts:
- cert_expires: Aug 16 15:03:10 2026 GMT
  host: catfact.ninja
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catfact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cat Facts API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cat Facts API
provider_slug: catfact
slug: catfact-domain-security
source_filename: catfact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catfact.ninja\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 15:03:10 2026 GMT\n  hsts: false\ndomains:\n- domain: catfact.ninja\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catfact/refs/heads/main/security/catfact-domain-security.yml
summary_line: TLSv1.3
tags:
- Cat Facts
- Trivia
- Fun
- Learning
- Free
---
