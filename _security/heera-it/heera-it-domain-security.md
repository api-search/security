---
api_specs:
- filename: heera-it-openapi.json
  format: json
  label: Sheikh Heera Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heera-it/openapi/heera-it-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heera.it
  spf: true
hosts:
- cert_expires: Dec 26 14:49:35 2026 GMT
  host: heera.it
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heera It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for heera-it, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: heera-it
provider_slug: heera-it
slug: heera-it-domain-security
source_filename: heera-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heera.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 14:49:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: heera.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heera-it/security/heera-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software Development
- Personal Brand
- Technology
- Consulting
- Architecture
---
