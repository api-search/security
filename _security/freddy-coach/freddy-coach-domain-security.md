---
api_specs:
- filename: freddy-coach-openapi.yml
  format: yaml
  label: Personal API
  slug: personal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freddy-coach/openapi/freddy-coach-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freddy.coach
  spf: true
hosts:
- cert_expires: Feb  4 14:01:27 2027 GMT
  host: freddy.coach
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: freddy Health Data Server Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for freddy Health Data Server, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: freddy Health Data Server
provider_slug: freddy-coach
slug: freddy-coach-domain-security
source_filename: freddy-coach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freddy.coach\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 14:01:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freddy.coach\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/freddy-coach/security/freddy-coach-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Data
- Artificial Intelligence
- Integration
- Privacy
---
