---
api_key_in: []
api_specs:
- filename: cnh-equipment-api-openapi.yml
  format: yaml
  label: CNH Equipment API
  slug: cnh-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-equipment-api-openapi.yml
- filename: cnh-farm-setup-api-openapi.yml
  format: yaml
  label: CNH Farm Setup API
  slug: cnh-farm-setup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-farm-setup-api-openapi.yml
- filename: cnh-operations-api-openapi.yml
  format: yaml
  label: CNH Operations API
  slug: cnh-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-operations-api-openapi.yml
- filename: cnh-prescriptions-api-openapi.yml
  format: yaml
  label: CNH Prescriptions API
  slug: cnh-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-prescriptions-api-openapi.yml
- filename: cnh-tokens-api-openapi.yml
  format: yaml
  label: CNH Tokens API
  slug: cnh-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-tokens-api-openapi.yml
- filename: cnh-vehicle-telemetry-api-openapi.yml
  format: yaml
  label: CNH Vehicle Telemetry API
  slug: cnh-vehicle-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-vehicle-telemetry-api-openapi.yml
- filename: cnh-webhooks-api-openapi.yml
  format: yaml
  label: CNH Webhooks API
  slug: cnh-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/openapi/cnh-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cnh Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CNH secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CNH
provider_slug: cnh
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://develop.cnh.com/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://develop.cnh.com/oauth/token
  name: oauth2
  sources:
  - openapi/cnh-fieldops-openapi.yml
  type: oauth2
slug: cnh-authentication
source_filename: cnh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cnh-fieldops-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://develop.cnh.com/oauth/authorize\n    tokenUrl: https://develop.cnh.com/oauth/token\n    scopes: 5\n  sources:\n  - openapi/cnh-fieldops-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cnh/refs/heads/main/authentication/cnh-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Agriculture
- Construction
- Telematics
- Equipment
- FieldOps
---
