---
api_specs:
- filename: hamla-io-openapi-generated.yml
  format: yaml
  label: Hamla API
  slug: hamla-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamla-io/openapi/_ae-authored/hamla-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hamla.io
  spf: false
hosts:
- cert_expires: Feb  2 04:14:36 2027 GMT
  host: hamla.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hamla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hamla, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Hamla
provider_slug: hamla-io
slug: hamla-io-domain-security
source_filename: hamla-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hamla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 04:14:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hamla.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hamla-io/security/hamla-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Artificial Intelligence
- Automation
- E-Commerce
- Software-as-a-Service
- Customer Engagement
---
