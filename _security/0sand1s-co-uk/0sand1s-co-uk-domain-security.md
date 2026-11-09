---
api_specs:
- filename: 0sand1s-co-uk-cis-api-openapi.yml
  format: yaml
  label: 0s and 1s CIS API
  slug: 0sand1s-co-uk-cis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0sand1s-co-uk/openapi/0sand1s-co-uk-cis-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 0sand1s.co.uk
  spf: true
hosts:
- cert_expires: Jan  7 13:22:19 2027 GMT
  host: 0sand1s.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 0Sand1S Co Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 0s and 1s, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 0s and 1s
provider_slug: 0sand1s-co-uk
slug: 0sand1s-co-uk-domain-security
source_filename: 0sand1s-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 0sand1s.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 13:22:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 0sand1s.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/0sand1s-co-uk/security/0sand1s-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Construction
- Payroll
- Tax
- United Kingdom
- Software
- CIS
---
