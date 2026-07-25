---
api_key_in: []
api_specs:
- filename: unum-authentication-api-openapi.yml
  format: yaml
  label: Unum Authentication API
  slug: unum-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-authentication-api-openapi.yml
- filename: unum-billing-api-openapi.yml
  format: yaml
  label: Unum Billing API
  slug: unum-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-billing-api-openapi.yml
- filename: unum-eligibility-api-openapi.yml
  format: yaml
  label: Unum Eligibility API
  slug: unum-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-eligibility-api-openapi.yml
- filename: unum-enrollment-api-openapi.yml
  format: yaml
  label: Unum Enrollment API
  slug: unum-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-enrollment-api-openapi.yml
- filename: unum-evidence-of-insurability-api-openapi.yml
  format: yaml
  label: Unum Evidence of Insurability API
  slug: unum-evidence-of-insurability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-evidence-of-insurability-api-openapi.yml
- filename: unum-leave-management-api-openapi.yml
  format: yaml
  label: Unum Leave Management API
  slug: unum-leave-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-leave-management-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Unum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Unum secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Unum
provider_slug: unum
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://api.unum.com/v1/oauth/token
  name: OAuth2
  sources:
  - openapi/unum-hr-connect-openapi.yml
  type: oauth2
slug: unum-authentication
source_filename: unum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unum-hr-connect-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.unum.com/v1/oauth/token\n    scopes: 9\n  sources:\n  - openapi/unum-hr-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/authentication/unum-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Insurance
- Benefits Administration
- HR Integration
- Disability Insurance
- Life Insurance
- Fortune 500
---
