---
api_key_in: []
api_specs:
- filename: apigee-api-management-openapi.yml
  format: yaml
  label: Apigee API Management
  slug: apigee-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-api-management-openapi.yml
- filename: apigee-api-hub-openapi.yml
  format: yaml
  label: Apigee API Hub API
  slug: apigee-api-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-api-hub-openapi.yml
- filename: apigee-integrations-openapi.yml
  format: yaml
  label: Apigee Integrations API
  slug: apigee-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-integrations-openapi.yml
- filename: apigee-apim-openapi.yml
  format: yaml
  label: Apigee API Management API
  slug: apigee-api-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-apim-openapi.yml
- filename: apigee-registry-openapi.yml
  format: yaml
  label: Apigee Registry API
  slug: apigee-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/openapi/apigee-registry-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Apigee Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Apigee secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Apigee
provider_slug: apigee
scheme_count: 1
schemes:
- description: Google OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/apigee-api-hub-openapi.yml
  - openapi/apigee-api-management-openapi.yml
  - openapi/apigee-apim-openapi.yml
  - openapi/apigee-integrations-openapi.yml
  - openapi/apigee-registry-openapi.yml
  type: oauth2
slug: apigee-authentication
source_filename: apigee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apigee-api-hub-openapi.yml, openapi/apigee-api-management-openapi.yml, openapi/apigee-apim-openapi.yml,\n  openapi/apigee-integrations-openapi.yml, openapi/apigee-registry-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  description: Google OAuth 2.0 authentication\n  sources:\n  - openapi/apigee-api-hub-openapi.yml\n  - openapi/apigee-api-management-openapi.yml\n  - openapi/apigee-apim-openapi.yml\n  - openapi/apigee-integrations-openapi.yml\n  - openapi/apigee-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/authentication/apigee-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advanced API Security
- Agentic AI
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Generative AI
- Hybrid
- Integrations
- Microservices
- MCP
- Model Context Protocol
- Monetization
---
