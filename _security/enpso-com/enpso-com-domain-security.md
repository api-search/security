---
api_specs:
- filename: enpso-com-openapi.yml
  format: yaml
  label: Enpso API
  slug: enpso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enpso-com/openapi/enpso-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: enpso.com
  spf: true
hosts:
- cert_expires: Feb  1 02:11:45 2027 GMT
  host: enpso.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Enpso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enpso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Enpso
provider_slug: enpso-com
slug: enpso-com-domain-security
source_filename: enpso-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enpso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 02:11:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: enpso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/enpso-com/security/enpso-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Employee Engagement
- Survey Tool
- Human Resources
- Software-as-a-Service
- US
---
