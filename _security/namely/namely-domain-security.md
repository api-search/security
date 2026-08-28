---
api_specs:
- filename: namely-api-openapi.json
  format: json
  label: Namely API
  slug: namely-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/openapi/namely-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: namely.com
  spf: true
hosts:
- cert_expires: Sep 29 18:37:47 2026 GMT
  host: namely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 04:06:44 2026 GMT
  host: developers.namely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Namely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Namely, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Namely
provider_slug: namely
slug: namely-domain-security
source_filename: namely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:37:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.namely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 04:06:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: namely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namely/refs/heads/main/security/namely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Human Capital Management
- Payroll
- Employee Data
- Onboarding
- Benefits
- Applicant Tracking
- Performance Management
- SCIM
- Single Sign-On
- Identity Provisioning
- Workforce Management
---
