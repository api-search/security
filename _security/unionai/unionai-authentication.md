---
api_key_in: []
api_specs:
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Projects API
  slug: flyteadmin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Workflows API
  slug: flyteadmin-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Tasks API
  slug: flyteadmin-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Launch Plans API
  slug: flyteadmin-launch-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Executions API
  slug: flyteadmin-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union Serverless
  slug: union-serverless
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Unionai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Union.ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Union.ai
provider_slug: unionai
scheme_count: 2
schemes:
- description: FlyteAdmin secures client connections with OAuth2. Interactive CLI/UI clients use the Authorization Code + PKCE flow; machine clients use the Client Credentials flow. User authentication to the console is via OpenID Connect. Tokens are presented as a Bearer access token.
  flows:
  - authorizationUrl: https://{org}.app.union.ai/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://{org}.app.union.ai/oauth2/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{org}.app.union.ai/oauth2/token
  name: OAuth2
  sources:
  - openapi/unionai-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/unionai-openapi.yml
  type: http
slug: unionai-authentication
source_filename: unionai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unionai-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{org}.app.union.ai/oauth2/authorize\n    tokenUrl: https://{org}.app.union.ai/oauth2/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://{org}.app.union.ai/oauth2/token\n    scopes: 1\n  description: FlyteAdmin secures client connections with OAuth2. Interactive CLI/UI clients\n    use the Authorization Code + PKCE flow; machine clients use the Client Credentials flow.\n    User authentication to the console is via OpenID Connect. Tokens are presented as a Bearer\n    access token.\n  sources:\n  - openapi/unionai-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/unionai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/authentication/unionai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AI
- ML
- Orchestration
- Workflows
- MLOps
- Flyte
- Serverless
---
