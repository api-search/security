---
api_key_in: []
api_specs:
- filename: kolayik-approval-process-api-openapi.yml
  format: yaml
  label: KolayIK Approval Process API
  slug: kolayik-approval-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-approval-process-api-openapi.yml
- filename: kolayik-calendar-api-openapi.yml
  format: yaml
  label: KolayIK Calendar API
  slug: kolayik-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-calendar-api-openapi.yml
- filename: kolayik-expense-api-openapi.yml
  format: yaml
  label: KolayIK Expense API
  slug: kolayik-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-expense-api-openapi.yml
- filename: kolayik-leave-api-openapi.yml
  format: yaml
  label: KolayIK Leave API
  slug: kolayik-leave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-leave-api-openapi.yml
- filename: kolayik-payroll-api-openapi.yml
  format: yaml
  label: KolayIK Payroll API
  slug: kolayik-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-payroll-api-openapi.yml
- filename: kolayik-person-api-openapi.yml
  format: yaml
  label: KolayIK Person API
  slug: kolayik-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-person-api-openapi.yml
- filename: kolayik-profile-api-openapi.yml
  format: yaml
  label: KolayIK Profile API
  slug: kolayik-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-profile-api-openapi.yml
- filename: kolayik-timelog-api-openapi.yml
  format: yaml
  label: KolayIK Timelog API
  slug: kolayik-timelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-timelog-api-openapi.yml
- filename: kolayik-training-api-openapi.yml
  format: yaml
  label: KolayIK Training API
  slug: kolayik-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-training-api-openapi.yml
- filename: kolayik-transaction-api-openapi.yml
  format: yaml
  label: KolayIK Transaction API
  slug: kolayik-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-transaction-api-openapi.yml
- filename: kolayik-unit-api-openapi.yml
  format: yaml
  label: KolayIK Unit API
  slug: kolayik-unit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/openapi/kolayik-unit-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kolayik Authentication
name_suffix: Authentication
oauth_flows: []
overview: KolayIK secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KolayIK
provider_slug: kolayik
scheme_count: 1
schemes:
- description: 'Kolay Public API requests are authenticated with a personal API token sent as `Authorization: Bearer <TOKEN>`. The collection-level auth in the official Postman collection is declared as bearer.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kolayik-public-api-openapi.yml
  - postman/kolayik-public-api-postman.json
  token_issuance: https://app.kolayik.com/settings/developer-settings
  type: http
slug: kolayik-authentication
source_filename: kolayik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apidocs.kolayik.com/\ndocs: https://apidocs.kolayik.com/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Kolay Public API requests are authenticated with a personal API token\n    sent as `Authorization: Bearer <TOKEN>`. The collection-level auth in the official\n    Postman collection is declared as bearer.'\n  token_issuance: https://app.kolayik.com/settings/developer-settings\n  sources:\n  - openapi/kolayik-public-api-openapi.yml\n  - postman/kolayik-public-api-postman.json\nnotes:\n- 'Tokens are self-service: the API documentation instructs developers to create an\n  API token from the in-product developer settings screen at https://app.kolayik.com/settings/developer-settings.'\n- No OAuth 2.0, OpenID Connect, mutualTLS or api-key-in-query scheme is documented\n  for the public API; bearer token is the only published\
  \ mechanism.\n- 'Authorization is bounded by the Kolay person access type of the account the token\n  belongs to (documented in the collection''s \"Additional Information\" section): owner\n  = full read/write on all employees; manager = same as owner except adding/removing\n  payment and tax details; employee = own information only. Kolay publishes no OAuth\n  scope surface, so scopes/ is intentionally absent.'\nsupport_contact: apisupport@kolay.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kolayik/refs/heads/main/authentication/kolayik-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Human Resources
- HR
- Payroll
- Human Capital Management
- Employee Management
- Time and Attendance
- Applicant Tracking
- SaaS
- Turkey
---
