---
api_specs:
- filename: workwae-com-v1-openapi.json
  format: json
  label: Workwae API V1 API
  slug: workwae-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/workwae-com/openapi/_original/workwae-com-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workwae.com
  spf: true
hosts:
- cert_expires: Jan 26 17:14:37 2027 GMT
  host: workwae.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: workwae-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for workwae-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: workwae-com
provider_slug: workwae-com
slug: workwae-com-domain-security
source_filename: workwae-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workwae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 17:14:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workwae.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/workwae-com/security/workwae-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Calendar
- Contacts
- Scheduling
- Artificial Intelligence
---
