---
api_specs:
- filename: homejourney-sg-openapi-generated.yml
  format: yaml
  label: Homejourney API
  slug: homejourney-sg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homejourney-sg/openapi/_ae-authored/homejourney-sg-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: homejourney.sg
  spf: true
hosts:
- cert_expires: Dec 27 14:01:24 2026 GMT
  host: homejourney.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Homejourney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homejourney, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Homejourney
provider_slug: homejourney-sg
slug: homejourney-sg-domain-security
source_filename: homejourney-sg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homejourney.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 14:01:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: homejourney.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/homejourney-sg/security/homejourney-sg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Mortgage
- Home Services
- Singapore
- Platform
---
