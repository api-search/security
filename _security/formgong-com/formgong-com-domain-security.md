---
api_specs:
- filename: formgong-com-openapi-generated.yml
  format: yaml
  label: Formgong API
  slug: formgong-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formgong-com/openapi/_ae-authored/formgong-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formgong.com
  spf: true
hosts:
- cert_expires: Jan 27 10:58:59 2027 GMT
  host: formgong.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Formgong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formgong, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Formgong
provider_slug: formgong-com
slug: formgong-com-domain-security
source_filename: formgong-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formgong.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 10:58:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: formgong.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/formgong-com/security/formgong-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Form Builder
- No Backend
- Telegram Integration
- Email Integration
- EU Data Jurisdiction
- Software-as-a-Service
---
