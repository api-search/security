---
api_specs:
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Clients API
  slug: intakeq-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Appointments API
  slug: intakeq-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Intake Forms API
  slug: intakeq-intake-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Treatment Notes API
  slug: intakeq-treatment-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Invoices API
  slug: intakeq-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
- filename: intakeq-openapi.yml
  format: yaml
  label: IntakeQ Files API
  slug: intakeq-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/openapi/intakeq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intakeq.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: intakeq.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 06:22:06 2026 GMT
  host: support.intakeq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intakeq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IntakeQ, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IntakeQ
provider_slug: intakeq
slug: intakeq-domain-security
source_filename: intakeq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intakeq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: false\n- host: support.intakeq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:22:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intakeq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intakeq/refs/heads/main/security/intakeq-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Practice Management
- Intake Forms
- Scheduling
- Health and Wellness
- EHR
- Telehealth
- HIPAA
---
