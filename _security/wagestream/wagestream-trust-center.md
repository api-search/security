---
api_specs:
- filename: wagestream-absences-api-openapi.yml
  format: yaml
  label: Wagestream Absences API
  slug: wagestream-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-absences-api-openapi.yml
- filename: wagestream-employees-api-openapi.yml
  format: yaml
  label: Wagestream Employees API
  slug: wagestream-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-employees-api-openapi.yml
- filename: wagestream-enrollment-api-openapi.yml
  format: yaml
  label: Wagestream Enrollment API
  slug: wagestream-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-enrollment-api-openapi.yml
- filename: wagestream-off-cycle-payment-api-openapi.yml
  format: yaml
  label: Wagestream Off Cycle Payment API
  slug: wagestream-off-cycle-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-off-cycle-payment-api-openapi.yml
- filename: wagestream-shifts-api-openapi.yml
  format: yaml
  label: Wagestream Shifts API
  slug: wagestream-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/openapi/wagestream-shifts-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Wagestream Trust Center
name_suffix: Trust Center
overview: Wagestream maintains a public trust center covering its security and compliance posture.
provider_name: Wagestream
provider_slug: wagestream
slug: wagestream-trust-center
source_filename: wagestream-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nprobe: true\nurl: https://trust.stream.co/\naliases:\n- https://trust.wagestream.com/\nplatform: Hexafort Trust Center\ncertifications: []\nnote: >-\n  Stream (Wagestream) publishes a trust center at trust.stream.co, linked from the footer of stream.co,\n  and trust.wagestream.com 302s to it. The page is a client-side rendered single-page application\n  (Hexafort) whose content is loaded from https://secure.hexafort.io/api/v1/orbit after JavaScript\n  execution, so no certification names could be read from the served HTML. certifications[] is left\n  EMPTY deliberately rather than guessed — presence of the trust center is verified, its contents are\n  not machine-readable. Named regulatory licences ARE published in plain HTML at the separate licences\n  page captured in conformance/wagestream-conformance.yml.\nevidence:\n- source: https://trust.wagestream.com/\n  http_status: 200\n  final_url: https://trust.stream.co/\n  content_type:\
  \ text/html\n  title: Hexafort Trust Center\n- source: https://secure.hexafort.io/api/v1/orbit\n  http_status: 200\n  note: API root reachable; no anonymous per-tenant trust-center endpoint found\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wagestream/refs/heads/main/security/wagestream-trust-center.yml
summary_line: trust center published
tags:
- financial-wellbeing
- earned-wage-access
- Fintech
- payroll
- human-resources
- workforce-management
- time-and-attendance
- employee-benefits
- workplace-savings
- hr-integrations
- b-corp
- united-kingdom
trust_url: https://trust.stream.co/
---
