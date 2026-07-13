---
api_specs:
- filename: llms.txt
  format: yaml
  label: HiBob Bob API
  slug: bob-api
  spec_type: OpenAPI
  url: https://apidocs.hibob.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hibob.com
  spf: true
hosts:
- cert_expires: Nov  9 11:27:00 2026 GMT
  host: www.hibob.com
  hsts: true
  hsts_max_age: 6
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 21:36:06 2026 GMT
  host: apidocs.hibob.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 11:05:12 2026 GMT
  host: api.hibob.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiBob, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HiBob
provider_slug: bob
slug: bob-domain-security
source_filename: bob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hibob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 11:27:00 2026 GMT\n  hsts: true\n  hsts_max_age: 6\n- host: apidocs.hibob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:36:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hibob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 11:05:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hibob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bob/refs/heads/main/security/bob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Human Resources
- HRIS
- Employee Management
- Time Off
- Attendance
- Payroll
- Workforce Planning
- Onboarding
- Goals
- OKR
---
