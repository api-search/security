---
api_specs:
- filename: intelex-openapi-generated.yml
  format: yaml
  label: Intelex API
  slug: intelex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intelex/openapi/_ae-authored/intelex-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intelex.com
  spf: true
hosts:
- cert_expires: Jan 10 13:30:04 2027 GMT
  host: www.intelex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intelex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intelex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Intelex
provider_slug: intelex
slug: intelex-domain-security
source_filename: intelex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intelex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 13:30:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: intelex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/intelex/security/intelex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EHS
- Quality Management
- Software
- Compliance
- ESG
---
