---
api_key_in: []
api_specs:
- filename: utilityapi-accounting-api-openapi.yml
  format: yaml
  label: UtilityAPI Accounting API
  slug: utilityapi-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-accounting-api-openapi.yml
- filename: utilityapi-authorizations-api-openapi.yml
  format: yaml
  label: UtilityAPI Authorizations API
  slug: utilityapi-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-authorizations-api-openapi.yml
- filename: utilityapi-bills-api-openapi.yml
  format: yaml
  label: UtilityAPI Bills API
  slug: utilityapi-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-bills-api-openapi.yml
- filename: utilityapi-events-api-openapi.yml
  format: yaml
  label: UtilityAPI Events API
  slug: utilityapi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-events-api-openapi.yml
- filename: utilityapi-files-api-openapi.yml
  format: yaml
  label: UtilityAPI Files API
  slug: utilityapi-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-files-api-openapi.yml
- filename: utilityapi-forms-api-openapi.yml
  format: yaml
  label: UtilityAPI Forms API
  slug: utilityapi-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-forms-api-openapi.yml
- filename: utilityapi-intervals-api-openapi.yml
  format: yaml
  label: UtilityAPI Intervals API
  slug: utilityapi-intervals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-intervals-api-openapi.yml
- filename: utilityapi-meters-api-openapi.yml
  format: yaml
  label: UtilityAPI Meters API
  slug: utilityapi-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-meters-api-openapi.yml
- filename: utilityapi-templates-api-openapi.yml
  format: yaml
  label: UtilityAPI Templates API
  slug: utilityapi-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-templates-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Utilityapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: UtilityAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UtilityAPI
provider_slug: utilityapi
scheme_count: 1
schemes:
- description: API token from the UtilityAPI dashboard
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/utilityapi-openapi.yml
  type: http
slug: utilityapi-authentication
source_filename: utilityapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/utilityapi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API token from the UtilityAPI dashboard\n  sources:\n  - openapi/utilityapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/authentication/utilityapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Utilities
- Green Button
- Billing Data
- Meter Data
- Clean Energy
---
