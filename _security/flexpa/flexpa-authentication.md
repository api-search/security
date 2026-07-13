---
api_key_in: []
api_specs:
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Link / Connect API
  slug: flexpa-link-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Access Tokens API
  slug: flexpa-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa FHIR Resources API
  slug: flexpa-fhir-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Claims Data API
  slug: flexpa-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Flexpa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flexpa secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flexpa
provider_slug: flexpa
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'A Patient Access Token (from the authorization_code flow) or an Application Access Token (from the client_credentials flow), sent as Authorization: Bearer {access_token}.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flexpa-openapi.yml
  type: http
slug: flexpa-authentication
source_filename: flexpa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flexpa-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'A Patient Access Token (from the authorization_code flow) or an Application\n    Access Token (from the client_credentials flow), sent as Authorization: Bearer {access_token}.'\n  sources:\n  - openapi/flexpa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/authentication/flexpa-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- FHIR
- Patient Access
- Claims Data
- Health Insurance
---
