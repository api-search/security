---
api_key_in: []
api_specs:
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Programs API
  slug: boost-insurance-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Quotes API
  slug: boost-insurance-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Policies API
  slug: boost-insurance-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Claims API
  slug: boost-insurance-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Endorsements API
  slug: boost-insurance-endorsements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Webhooks API
  slug: boost-insurance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Boost Insurance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Boost Insurance secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Boost Insurance
provider_slug: boost-insurance
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication endpoint and presented as a Bearer token.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.insurtech.dev/auth/oauth2/token
  name: boostOAuth
  sources:
  - openapi/boost-insurance-openapi.yml
  type: oauth2
slug: boost-insurance-authentication
source_filename: boost-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/boost-insurance-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: boostOAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.insurtech.dev/auth/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication\n    endpoint and presented as a Bearer token.\n  sources:\n  - openapi/boost-insurance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/authentication/boost-insurance-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Insurance
- Embedded Insurance
- Insurance-as-a-Service
- Policy Administration
- Claims
---
