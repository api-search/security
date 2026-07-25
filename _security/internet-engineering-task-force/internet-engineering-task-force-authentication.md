---
api_key_in:
- query
api_specs:
- filename: internet-engineering-task-force-documents-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Documents API
  slug: internet-engineering-task-force-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-documents-api-openapi.yml
- filename: internet-engineering-task-force-framework-api-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Framework API API
  slug: internet-engineering-task-force-framework-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-framework-api-api-openapi.yml
- filename: internet-engineering-task-force-identity-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Identity API
  slug: internet-engineering-task-force-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-identity-api-openapi.yml
- filename: internet-engineering-task-force-iesg-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force IESG API
  slug: internet-engineering-task-force-iesg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-iesg-api-openapi.yml
- filename: internet-engineering-task-force-meetings-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Meetings API
  slug: internet-engineering-task-force-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-meetings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Internet Engineering Task Force Authentication
name_suffix: Authentication
oauth_flows: []
overview: Internet Engineering Task Force secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Internet Engineering Task Force
provider_slug: internet-engineering-task-force
scheme_count: 1
schemes:
- description: Endpoint-scoped Personal API Key. Each key is valid only for one endpoint.
  in: query
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/internet-engineering-task-force-openapi.yml
  type: apiKey
slug: internet-engineering-task-force-authentication
source_filename: internet-engineering-task-force-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/internet-engineering-task-force-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Endpoint-scoped Personal API Key. Each key is valid only for one endpoint.\n  sources:\n  - openapi/internet-engineering-task-force-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/authentication/internet-engineering-task-force-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Internet
- Protocols
- RFC
- Standards
- Working Groups
---
