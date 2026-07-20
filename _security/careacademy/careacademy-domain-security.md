---
api_specs:
- filename: careacademy-openapi-original.yml
  format: yaml
  label: CareAcademy API
  slug: careacademy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/careacademy/refs/heads/main/openapi/careacademy-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: careacademy.com
  spf: true
hosts:
- cert_expires: Sep 22 22:41:20 2026 GMT
  host: careacademy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 22:41:20 2026 GMT
  host: staging.careacademy.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Careacademy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareAcademy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CareAcademy
provider_slug: careacademy
slug: careacademy-domain-security
source_filename: careacademy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: careacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:41:20 2026 GMT\n  hsts: false\n- host: staging.careacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:41:20 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: careacademy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/careacademy/refs/heads/main/security/careacademy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Training
- Education
- Compliance
- Home Care
- Home Health
- Hospice
- Senior Living
- Healthcare
- Workforce Management
- Single Sign-On
- Caregivers
---
