---
api_specs:
- filename: epaypolicy-openapi-generated.yml
  format: yaml
  label: ePayPolicy API
  slug: epaypolicy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/epaypolicy/openapi/_ae-authored/epaypolicy-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: epaypolicy.com
  spf: true
hosts:
- cert_expires: Feb  4 21:22:35 2027 GMT
  host: epaypolicy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ePayPolicy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ePayPolicy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ePayPolicy
provider_slug: epaypolicy
slug: epaypolicy-domain-security
source_filename: epaypolicy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epaypolicy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 21:22:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: epaypolicy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/epaypolicy/security/epaypolicy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Payments
- Fintech
---
