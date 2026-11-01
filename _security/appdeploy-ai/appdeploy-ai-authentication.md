---
anonymous_access: false
api_key_in: []
api_specs:
- filename: appdeploy-ai-mcp-api-openapi.yml
  format: yaml
  label: appdeploy-ai MCP API
  slug: appdeploy-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appdeploy-ai/openapi/appdeploy-ai-mcp-api-openapi.yml
- filename: appdeploy-ai-oauth-discovery-api-openapi.yml
  format: yaml
  label: appdeploy-ai OAuth discovery API
  slug: appdeploy-ai-oauth-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appdeploy-ai/openapi/appdeploy-ai-oauth-discovery-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Appdeploy Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: appdeploy-ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: appdeploy-ai
provider_slug: appdeploy-ai
scheme_count: 2
schemes:
- description: OAuth 2.0 Authorization Code flow with PKCE and dynamic client registration. AppDeploy declares separate tool permission scopes for read, write, and delete operations.
  flows:
  - authorizationUrl: https://api-v2.appdeploy.ai/mcp/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api-v2.appdeploy.ai/mcp/token
  name: AppDeployOAuth
  sources:
  - openapi/appdeploy-ai-openapi.json
  type: oauth2
- description: Bearer access token issued by AppDeploy OAuth or an AppDeploy API key for clients that cannot complete OAuth. OAuth is preferred because it declares scopes.
  name: AppDeployBearerToken
  scheme: bearer
  sources:
  - openapi/appdeploy-ai-openapi.json
  type: http
slug: appdeploy-ai-authentication
source_filename: appdeploy-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/appdeploy-ai-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: AppDeployOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-v2.appdeploy.ai/mcp/authorize\n    tokenUrl: https://api-v2.appdeploy.ai/mcp/token\n    scopes: 3\n  description: OAuth 2.0 Authorization Code flow with PKCE and dynamic client registration.\n    AppDeploy declares separate tool permission scopes for read, write, and delete operations.\n  sources:\n  - openapi/appdeploy-ai-openapi.json\n- name: AppDeployBearerToken\n  type: http\n  scheme: bearer\n  description: Bearer access token issued by AppDeploy OAuth or an AppDeploy API key for clients\n    that cannot complete OAuth. OAuth is preferred because it declares scopes.\n  sources:\n  - openapi/appdeploy-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/appdeploy-ai/authentication/appdeploy-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- AI
- Deployment
- Platform
- LowCode
- Automation
---
