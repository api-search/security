---
api_specs:
- filename: readwise-openapi-generated.yml
  format: yaml
  label: Readwise API
  slug: readwise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/readwise/openapi/_ae-authored/readwise-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: readwise.io
  spf: true
hosts:
- cert_expires: Jan 15 12:21:47 2027 GMT
  host: readwise.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Readwise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Readwise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Readwise
provider_slug: readwise
slug: readwise-domain-security
source_filename: readwise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: readwise.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 12:21:47 2027 GMT\n  hsts: false\ndomains:\n- domain: readwise.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/readwise/security/readwise-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Reading
- Productivity
- Knowledge Management
- SaaS
- API
---
