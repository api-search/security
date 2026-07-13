---
api_key_in:
- header
api_specs:
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Patients API
  slug: opendental-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Appointments API
  slug: opendental-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Providers API
  slug: opendental-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Procedures API
  slug: opendental-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Insurance & Claims API
  slug: opendental-insurance-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Payments API
  slug: opendental-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Accounts & Ledger API
  slug: opendental-accounts-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Fees & Fee Schedules API
  slug: opendental-fees-feeschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Recalls API
  slug: opendental-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Documents API
  slug: opendental-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Medications & Prescriptions API
  slug: opendental-medications-rx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Referrals API
  slug: opendental-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Sheets API
  slug: opendental-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opendental Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Dental secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Dental
provider_slug: opendental
scheme_count: 1
schemes:
- description: Send "ODFHIR {DeveloperKey}/{CustomerKey}" - the per-application Developer Key issued by Open Dental Vendor Relations combined with the per-customer Customer Key. Some endpoints also accept HTTP Basic auth with the Developer Key as username and the Customer Key as password.
  in: header
  name: odfhirAuth
  parameter: Authorization
  sources:
  - openapi/opendental-openapi.yml
  type: apiKey
slug: opendental-authentication
source_filename: opendental-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opendental-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: odfhirAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Send \"ODFHIR {DeveloperKey}/{CustomerKey}\" - the per-application Developer Key\n    issued by Open Dental Vendor Relations combined with the per-customer Customer Key. Some\n    endpoints also accept HTTP Basic auth with the Developer Key as username and the Customer\n    Key as password.\n  sources:\n  - openapi/opendental-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/authentication/opendental-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Dental
- Practice Management
- Healthcare
- EHR
- Patient Records
- REST
---
