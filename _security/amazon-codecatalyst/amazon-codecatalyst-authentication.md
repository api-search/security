---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-codecatalyst-session-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst Session API
  slug: amazon-codecatalyst-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-session-api-openapi.yml
- filename: amazon-codecatalyst-spaces-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst Spaces API
  slug: amazon-codecatalyst-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-spaces-api-openapi.yml
- filename: amazon-codecatalyst-access-tokens-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst Access Tokens API
  slug: amazon-codecatalyst-access-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-access-tokens-api-openapi.yml
- filename: amazon-codecatalyst-user-details-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst User Details API
  slug: amazon-codecatalyst-user-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-user-details-api-openapi.yml
- filename: amazon-codecatalyst-devenvironments-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst Codecatalyst Devenvironments API
  slug: amazon-codecatalyst-devenvironments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-devenvironments-api-openapi.yml
- filename: amazon-codecatalyst-operations-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst Codecatalyst Operations API
  slug: amazon-codecatalyst-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-operations-api-openapi.yml
- filename: amazon-codecatalyst-projects-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst Codecatalyst Projects API
  slug: amazon-codecatalyst-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-projects-api-openapi.yml
- filename: amazon-codecatalyst-sourcerepositories-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst Codecatalyst Sourcerepositories API
  slug: amazon-codecatalyst-sourcerepositories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-sourcerepositories-api-openapi.yml
- filename: amazon-codecatalyst-workflowruns-api-openapi.yml
  format: yaml
  label: Amazon CodeCatalyst Codecatalyst Workflowruns API
  slug: amazon-codecatalyst-workflowruns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecatalyst/openapi/amazon-codecatalyst-workflowruns-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Codecatalyst Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CodeCatalyst secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
scheme_count: 1
schemes:
- in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-codecatalyst-openapi-original.yaml
  type: apiKey
slug: amazon-codecatalyst-authentication
source_filename: amazon-codecatalyst-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-codecatalyst-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/amazon-codecatalyst-openapi-original.yaml\n"
source_yaml_url: https://artifacts.apis.io/amazon-codecatalyst/authentication/amazon-codecatalyst-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Version Control
---
