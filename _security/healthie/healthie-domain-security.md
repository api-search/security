---
api_specs:
- filename: healthie-webhooks-asyncapi.yml
  format: yaml
  label: Healthie GraphQL API
  slug: healthie-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthie/refs/heads/main/asyncapi/healthie-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gethealthie.com
  spf: true
hosts:
- cert_expires: Aug 16 07:27:27 2026 GMT
  host: www.gethealthie.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 05:33:44 2026 GMT
  host: docs.gethealthie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.gethealthie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Healthie, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Healthie
provider_slug: healthie
slug: healthie-domain-security
source_filename: healthie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gethealthie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:27:27 2026 GMT\n  hsts: false\n- host: docs.gethealthie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:33:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gethealthie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gethealthie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthie/refs/heads/main/security/healthie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API-First
- Appointments
- Billing
- Care Plans
- Charting
- Claims
- Clinical
- Digital Health
- EHR
- EMR
- Forms
- GraphQL
- Health Tech
- Healthcare
- Insurance
- Intake
- Online Programs
- Patient Engagement
- Patient Portal
- Practice Management
- Programs
- Scheduling
- Telehealth
- Wellness
- Webhooks
---
