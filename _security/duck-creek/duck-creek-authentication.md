---
api_key_in: []
api_specs:
- filename: duck-creek-billing-api-openapi.yml
  format: yaml
  label: Duck Creek Billing API
  slug: duck-creek-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-billing-api-openapi.yml
- filename: duck-creek-claims-api-openapi.yml
  format: yaml
  label: Duck Creek Claims API
  slug: duck-creek-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-claims-api-openapi.yml
- filename: duck-creek-billing-api-openapi.yml
  format: yaml
  label: duck-creek Billing API
  slug: duck-creek-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-billing-api-openapi.yml
- filename: duck-creek-claims-api-openapi.yml
  format: yaml
  label: duck-creek Claims API
  slug: duck-creek-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-claims-api-openapi.yml
- filename: duck-creek-policies-api-openapi.yml
  format: yaml
  label: duck-creek Policies API
  slug: duck-creek-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-policies-api-openapi.yml
- filename: duck-creek-products-api-openapi.yml
  format: yaml
  label: duck-creek Products API
  slug: duck-creek-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-products-api-openapi.yml
- filename: duck-creek-quotes-api-openapi.yml
  format: yaml
  label: duck-creek Quotes API
  slug: duck-creek-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/openapi/duck-creek-quotes-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Duck Creek Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Duck Creek secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Duck Creek
provider_slug: duck-creek
scheme_count: 1
schemes:
- description: OAuth 2.0 for Duck Creek Anywhere API authentication
  flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://api.duckcreek.com/oauth/token
  name: oauth2
  sources:
  - openapi/duck-creek-policy-openapi.yml
  type: oauth2
slug: duck-creek-authentication
source_filename: duck-creek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/duck-creek-policy-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.duckcreek.com/oauth/token\n    scopes: 5\n  description: OAuth 2.0 for Duck Creek Anywhere API authentication\n  sources:\n  - openapi/duck-creek-policy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/authentication/duck-creek-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
