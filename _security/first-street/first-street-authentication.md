---
api_key_in:
- query
api_specs:
- filename: first-street-enterprise-api-openapi.yml
  format: yaml
  label: First Street Enterprise API
  slug: first-street-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-enterprise-api-openapi.yml
- filename: first-street-graphql-api-openapi.yml
  format: yaml
  label: First Street Graphql API
  slug: first-street-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-graphql-api-openapi.yml
- filename: first-street-maps-api-openapi.yml
  format: yaml
  label: First Street Maps API
  slug: first-street-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-maps-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: First Street Authentication
name_suffix: Authentication
oauth_flows: []
overview: First Street secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: First Street
provider_slug: first-street
scheme_count: 2
schemes:
- in: query
  name: apiKeyQuery
  parameter: key
  sources:
  - openapi/first-street-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/first-street-openapi.yml
  type: http
slug: first-street-authentication
source_filename: first-street-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/first-street-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/first-street-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/first-street-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/authentication/first-street-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Environment
- Modeling
- Risk
- Climate
---
