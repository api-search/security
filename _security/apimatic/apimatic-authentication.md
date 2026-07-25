---
api_key_in:
- header
api_specs:
- filename: apimatic-apis-api-openapi.yml
  format: yaml
  label: APIMatic APIs API
  slug: apimatic-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-apis-api-openapi.yml
- filename: apimatic-portals-api-openapi.yml
  format: yaml
  label: APIMatic Portals API
  slug: apimatic-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-portals-api-openapi.yml
- filename: apimatic-sdk-generation-api-openapi.yml
  format: yaml
  label: APIMatic SDK Generation API
  slug: apimatic-sdk-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-sdk-generation-api-openapi.yml
- filename: apimatic-transformation-api-openapi.yml
  format: yaml
  label: APIMatic Transformation API
  slug: apimatic-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-transformation-api-openapi.yml
- filename: apimatic-validation-api-openapi.yml
  format: yaml
  label: APIMatic Validation API
  slug: apimatic-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-validation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apimatic Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIMatic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIMatic
provider_slug: apimatic
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/apimatic-platform-api.yaml
  type: apiKey
slug: apimatic-authentication
source_filename: apimatic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apimatic-platform-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/apimatic-platform-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/authentication/apimatic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Transformation
- Code Generation
- Developer Experience
- Documentation
- SDK Generation
---
