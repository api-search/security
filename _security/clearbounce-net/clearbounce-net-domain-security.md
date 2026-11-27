---
api_specs:
- filename: clearbounce-net-openapi-generated.yml
  format: yaml
  label: ClearBounce API
  slug: clearbounce-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearbounce-net/openapi/_ae-authored/clearbounce-net-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clearbounce.net
  spf: true
hosts:
- cert_expires: Jan 23 19:35:40 2027 GMT
  host: clearbounce.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ClearBounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearBounce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ClearBounce
provider_slug: clearbounce-net
slug: clearbounce-net-domain-security
source_filename: clearbounce-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearbounce.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 19:35:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clearbounce.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clearbounce-net/security/clearbounce-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Verification
- List Cleaning
- Form Validation
- Deliverability
- Marketing Tools
---
