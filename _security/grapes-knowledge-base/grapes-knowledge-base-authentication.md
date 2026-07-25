---
api_key_in: []
api_specs:
- filename: grapes-knowledge-base-agents-api-openapi.yml
  format: yaml
  label: Grapes Knowledge Base Agents API
  slug: grapes-knowledge-base-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-knowledge-base/refs/heads/main/openapi/grapes-knowledge-base-agents-api-openapi.yml
- filename: grapes-knowledge-base-datasets-api-openapi.yml
  format: yaml
  label: Grapes Knowledge Base Datasets API
  slug: grapes-knowledge-base-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-knowledge-base/refs/heads/main/openapi/grapes-knowledge-base-datasets-api-openapi.yml
- filename: grapes-knowledge-base-projects-api-openapi.yml
  format: yaml
  label: Grapes Knowledge Base Projects API
  slug: grapes-knowledge-base-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-knowledge-base/refs/heads/main/openapi/grapes-knowledge-base-projects-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Grapes Knowledge Base Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grapes Knowledge Base secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Grapes Knowledge Base
provider_slug: grapes-knowledge-base
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/grapes-knowledge-base-openapi.yml
  type: http
slug: grapes-knowledge-base-authentication
source_filename: grapes-knowledge-base-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/grapes-knowledge-base-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/grapes-knowledge-base-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grapes-knowledge-base/refs/heads/main/authentication/grapes-knowledge-base-authentication.yml
summary_line: http · 1 scheme
tags:
- Knowledge Management
- Knowledge Base
- Data Management
- Automation
- HATEOAS
---
