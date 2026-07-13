---
api_key_in: []
api_specs:
- filename: opslevel-openapi.yml
  format: yaml
  label: OpsLevel GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opslevel/refs/heads/main/openapi/opslevel-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opslevel Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpsLevel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpsLevel
provider_slug: opslevel
scheme_count: 1
schemes:
- bearerFormat: Token
  description: 'OpsLevel API token created in the OpsLevel app. Supply as

    `Authorization: Bearer ${TOKEN}`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/opslevel-openapi.yml
  type: http
slug: opslevel-authentication
source_filename: opslevel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opslevel-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Token\n  description: |-\n    OpsLevel API token created in the OpsLevel app. Supply as\n    `Authorization: Bearer ${TOKEN}`.\n  sources:\n  - openapi/opslevel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opslevel/refs/heads/main/authentication/opslevel-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Portal
- DevOps
- Experience
- Internal Developer Portal
- Microservices
- Platform Engineering
- Service Catalog
- Service Maturity
---
