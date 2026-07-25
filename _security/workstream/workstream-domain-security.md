---
api_specs:
- filename: workstream-applicants-api-openapi.yml
  format: yaml
  label: Workstream Applicants API
  slug: workstream-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-applicants-api-openapi.yml
- filename: workstream-authorization-api-openapi.yml
  format: yaml
  label: Workstream Authorization API
  slug: workstream-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-authorization-api-openapi.yml
- filename: workstream-company-roles-api-openapi.yml
  format: yaml
  label: Workstream Company Roles API
  slug: workstream-company-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-company-roles-api-openapi.yml
- filename: workstream-company-users-api-openapi.yml
  format: yaml
  label: Workstream Company Users API
  slug: workstream-company-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-company-users-api-openapi.yml
- filename: workstream-custom-field-api-openapi.yml
  format: yaml
  label: Workstream Custom Field API
  slug: workstream-custom-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-custom-field-api-openapi.yml
- filename: workstream-departments-api-openapi.yml
  format: yaml
  label: Workstream Departments API
  slug: workstream-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-departments-api-openapi.yml
- filename: workstream-employee-documents-api-openapi.yml
  format: yaml
  label: Workstream Employee Documents API
  slug: workstream-employee-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-employee-documents-api-openapi.yml
- filename: workstream-employees-api-openapi.yml
  format: yaml
  label: Workstream Employees API
  slug: workstream-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-employees-api-openapi.yml
- filename: workstream-imported-employee-infos-api-openapi.yml
  format: yaml
  label: Workstream Imported Employee Infos API
  slug: workstream-imported-employee-infos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-imported-employee-infos-api-openapi.yml
- filename: workstream-locations-api-openapi.yml
  format: yaml
  label: Workstream Locations API
  slug: workstream-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-locations-api-openapi.yml
- filename: workstream-positions-api-openapi.yml
  format: yaml
  label: Workstream Positions API
  slug: workstream-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-positions-api-openapi.yml
- filename: workstream-team-members-api-openapi.yml
  format: yaml
  label: Workstream Team Members API
  slug: workstream-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-team-members-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workstream.us
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: workstream.us
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 19:06:01 2026 GMT
  host: docs.workstream.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: public-api.workstream.us
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workstream, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workstream
provider_slug: workstream
slug: workstream-domain-security
source_filename: workstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workstream.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\n- host: docs.workstream.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 19:06:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.workstream.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: workstream.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/security/workstream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hr Tech
- Hiring
- Payroll
- Onboarding
- Applicant Tracking
- Hourly Workforce
- Restaurants
---
