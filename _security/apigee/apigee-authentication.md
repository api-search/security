---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apigee-hybrid-api-openapi.yml
  format: yaml
  label: Apigee Hybrid API
  slug: apigee-hybrid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apigee/openapi/apigee-hybrid-api-openapi.yml
- filename: apigee-organizations-api-openapi.yml
  format: yaml
  label: Apigee Organizations API
  slug: apigee-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apigee/openapi/apigee-organizations-api-openapi.yml
- filename: apigee-projects-api-openapi.yml
  format: yaml
  label: Apigee Projects API
  slug: apigee-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apigee/openapi/apigee-projects-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/apigee/authentication/apigee-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Apigee
- Advanced API Security
- AI Agents
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Generative AI
- Hybrid
- Integration
- Microservices
- MCP
- Monetization
---
