---
api_key_in: []
api_specs:
- filename: blue-prism-enterprise-api-openapi.yml
  format: yaml
  label: Blue Prism API
  slug: blue-prism
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/openapi/blue-prism-enterprise-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Blue Prism Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Blue Prism secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Blue Prism
provider_slug: blue-prism
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token issued from Authentication Server.
  name: Bearer
  scheme: bearer
  sources:
  - openapi/blue-prism-enterprise-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth-server/connect/token
  name: OAuth2
  sources:
  - openapi/blue-prism-enterprise-api-openapi.yml
  type: oauth2
slug: blue-prism-authentication
source_filename: blue-prism-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/blue-prism-enterprise-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token issued from Authentication Server.\n  sources:\n  - openapi/blue-prism-enterprise-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth-server/connect/token\n    scopes: 2\n  sources:\n  - openapi/blue-prism-enterprise-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-prism/refs/heads/main/authentication/blue-prism-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AI Automation
- RPA
- Intelligent Automation
- Business Process Management
- Process Orchestration
- Agentic AI
- Workflow-Automation
- Enterprise Software
---
