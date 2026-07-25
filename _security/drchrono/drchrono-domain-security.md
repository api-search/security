---
api_specs:
- filename: drchrono-administrative-api-openapi.yml
  format: yaml
  label: drchrono Administrative API
  slug: drchrono-administrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-administrative-api-openapi.yml
- filename: drchrono-audit-api-openapi.yml
  format: yaml
  label: drchrono Audit API
  slug: drchrono-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-audit-api-openapi.yml
- filename: drchrono-availability-api-openapi.yml
  format: yaml
  label: drchrono Availability API
  slug: drchrono-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-availability-api-openapi.yml
- filename: drchrono-billing-api-openapi.yml
  format: yaml
  label: drchrono Billing API
  slug: drchrono-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-billing-api-openapi.yml
- filename: drchrono-clinical-api-openapi.yml
  format: yaml
  label: drchrono Clinical API
  slug: drchrono-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-clinical-api-openapi.yml
- filename: drchrono-practice-management-api-openapi.yml
  format: yaml
  label: drchrono Practice Management API
  slug: drchrono-practice-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-practice-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drchrono.com
  spf: true
hosts:
- cert_expires: Oct  7 00:48:42 2026 GMT
  host: www.drchrono.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: app.drchrono.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drchrono Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for drchrono, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: drchrono
provider_slug: drchrono
slug: drchrono-domain-security
source_filename: drchrono-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drchrono.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:48:42 2026 GMT\n  hsts: false\n- host: app.drchrono.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: drchrono.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/security/drchrono-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EHR
- Electronic Health Records
- Healthcare
- Medical Records
- Practice Management
- HIPAA
- Appointments
- Billing
- Prescriptions
- Lab Integration
- FHIR
---
