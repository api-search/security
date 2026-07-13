---
api_specs:
- filename: ukg-pro-hcm-openapi.yml
  format: yaml
  label: UKG Pro HCM API
  slug: ukg-pro-hcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg/refs/heads/main/openapi/ukg-pro-hcm-openapi.yml
- filename: ukg-pro-wfm-openapi.yml
  format: yaml
  label: UKG Pro Workforce Management API
  slug: ukg-pro-wfm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukg/refs/heads/main/openapi/ukg-pro-wfm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ukg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ultipro.com
  spf: true
hosts:
- cert_expires: Sep 17 16:56:11 2026 GMT
  host: www.ukg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:39:15 2026 GMT
  host: developer.ukg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: service.ultipro.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ukg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UKG, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UKG
provider_slug: ukg
slug: ukg-domain-security
source_filename: ukg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ukg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:56:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ukg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:39:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: service.ultipro.com\n  https: false\ndomains:\n- domain: ukg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ultipro.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukg/refs/heads/main/security/ukg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Human Capital Management
- HCM
- Workforce Management
- HR
- Payroll
- Time and Attendance
- Benefits
- Scheduling
---
