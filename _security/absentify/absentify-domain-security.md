---
api_specs:
- filename: absentify-openapi.yml
  format: yaml
  label: Absentify API
  slug: absentify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/openapi/absentify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: absentify.com
  spf: true
hosts:
- cert_expires: Sep 13 09:13:37 2026 GMT
  host: absentify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.absentify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Absentify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Absentify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Absentify
provider_slug: absentify
slug: absentify-domain-security
source_filename: absentify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: absentify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 09:13:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.absentify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: absentify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/security/absentify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
---
