---
api_key_in: []
api_specs:
- filename: napkinai-openapi.yml
  format: yaml
  label: Napkin AI API
  slug: napkin-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/napkinai/refs/heads/main/openapi/napkinai-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Napkinai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Napkin.AI secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Napkin.AI
provider_slug: napkinai
scheme_count: 2
schemes:
- description: Bearer token authentication required for all endpoints. Use a Napkin AI account API token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/napkinai-openapi.yml
  type: http
- description: OAuth 2.0 authorization code flow (beta). Your application must be approved by the Napkin AI team to obtain client credentials.
  flows:
  - authorizationUrl: https://api.napkin.ai/v1/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.napkin.ai/v1/oauth/token
  name: oauth2
  sources:
  - openapi/napkinai-openapi.yml
  type: oauth2
slug: napkinai-authentication
source_filename: napkinai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/napkinai-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication required for all endpoints. Use a Napkin AI account\n    API token in the Authorization header.\n  sources:\n  - openapi/napkinai-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.napkin.ai/v1/oauth/authorize\n    tokenUrl: https://api.napkin.ai/v1/oauth/token\n    scopes: 2\n  description: OAuth 2.0 authorization code flow (beta). Your application must be approved by\n    the Napkin AI team to obtain client credentials.\n  sources:\n  - openapi/napkinai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/napkinai/refs/heads/main/authentication/napkinai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Ai
- Visualization
- Diagrams
- Charts
- Infographics
- Presentations
- Content Generation
- Design
- Developer API
---
