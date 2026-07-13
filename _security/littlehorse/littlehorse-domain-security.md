---
api_specs:
- filename: littlehorse-api.yml
  format: yaml
  label: LittleHorse
  slug: littlehorse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/littlehorse/refs/heads/main/openapi/littlehorse-api.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: littlehorse.dev
  spf: false
hosts:
- cert_expires: Aug 11 05:54:36 2026 GMT
  host: littlehorse.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Littlehorse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LittleHorse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LittleHorse
provider_slug: littlehorse
slug: littlehorse-domain-security
source_filename: littlehorse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: littlehorse.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 05:54:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: littlehorse.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/littlehorse/refs/heads/main/security/littlehorse-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Microservices
---
