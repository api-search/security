---
api_specs:
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Employees API
  slug: workmotion-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Contracts API
  slug: workmotion-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Onboarding API
  slug: workmotion-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Absences API
  slug: workmotion-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Documents API
  slug: workmotion-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Cost Calculator API
  slug: workmotion-cost-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Webhooks API
  slug: workmotion-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workmotion.com
  spf: true
hosts:
- cert_expires: Oct  2 07:58:56 2026 GMT
  host: www.workmotion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 10:29:35 2026 GMT
  host: workmotion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 14:18:58 2026 GMT
  host: api.workmotion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workmotion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorkMotion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WorkMotion
provider_slug: workmotion
slug: workmotion-domain-security
source_filename: workmotion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workmotion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:58:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: workmotion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:29:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.workmotion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 14:18:58 2026 GMT\n  hsts: null\ndomains:\n- domain: workmotion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/security/workmotion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Employer of Record
- EOR
- Global Employment
- HR
- Payroll
- Onboarding
- Contractors
- Compliance
---
