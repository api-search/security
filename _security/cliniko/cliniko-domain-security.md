---
api_specs:
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Patients API
  slug: cliniko-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Appointments API
  slug: cliniko-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Practitioners and Businesses API
  slug: cliniko-practitioners-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Appointment Types API
  slug: cliniko-appointment-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Invoices API
  slug: cliniko-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
- filename: cliniko-openapi.yml
  format: yaml
  label: Cliniko Treatment Notes API
  slug: cliniko-treatment-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/openapi/cliniko-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cliniko.com
  spf: true
  spf_record: v=spf1 include:spf0.cliniko.com -all
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: cliniko.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  cert_issuer: Amazon RSA 2048 M03
  host: api.au1.cliniko.com
  hsts: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cliniko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cliniko, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cliniko
provider_slug: cliniko
slug: cliniko-domain-security
source_filename: cliniko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cliniko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon RSA 2048 M04\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n- host: api.au1.cliniko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon RSA 2048 M03\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_preload: true\ndomains:\n- domain: cliniko.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf0.cliniko.com -all'\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cliniko/refs/heads/main/security/cliniko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Practice Management
- Healthcare
- Allied Health
- Appointments
- Scheduling
- Patients
- EHR
- Clinics
- Bookings
- SaaS
---
