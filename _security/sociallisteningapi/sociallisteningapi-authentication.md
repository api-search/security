---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: sociallisteningapi-openapi.yml
  format: yaml
  label: SocialListeningAPI
  slug: sociallisteningapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sociallisteningapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: SocialListeningAPI secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SocialListeningAPI
provider_slug: sociallisteningapi
scheme_count: 2
schemes:
- applies_to: REST API (https://api.sociallisteningapi.com/api/v1/*)
  description: Your SocialListeningAPI key.
  errors:
    '401': A missing or invalid key returns 401.
    '402': If the workspace has no credits left, the API returns 402.
    '403': An account that has not been activated returns 403.
  guidance: Do not put it in the URL. Keep it out of browser code, mobile apps, public repositories, screenshots, and logs. Call SocialListeningAPI from your server so the key stays private.
  in: header
  key_prefix: slapi_
  name: ApiKeyAuth
  obtain: Create an account, activate it from the email, then copy the key from the dashboard or Settings > API key.
  parameter: x-api-key
  sources:
  - openapi/sociallisteningapi-openapi.yml
  - https://sociallisteningapi.com/docs/authentication
  type: apiKey
- applies_to: Remote MCP server https://api.sociallisteningapi.com/mcp
  bearer_methods:
  - header
  flows:
    authorizationCode:
      authorizationUrl: https://api.sociallisteningapi.com/authorize
      pkce: S256
      revocationUrl: https://api.sociallisteningapi.com/revoke
      scopes:
      - mcp
      - mcp:search
      tokenUrl: https://api.sociallisteningapi.com/token
  grant_types:
  - authorization_code
  - refresh_token
  name: MCP OAuth
  sources:
  - https://api.sociallisteningapi.com/.well-known/oauth-authorization-server (200)
  - https://api.sociallisteningapi.com/.well-known/oauth-protected-resource/mcp (200)
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: sociallisteningapi-authentication
source_filename: sociallisteningapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: searched\nsource: https://sociallisteningapi.com/docs/authentication\ndocs: https://sociallisteningapi.com/docs/authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Your SocialListeningAPI key.\n  key_prefix: slapi_\n  applies_to: REST API (https://api.sociallisteningapi.com/api/v1/*)\n  obtain: Create an account, activate it from the email, then copy the key from the dashboard or Settings > API\n    key.\n  errors:\n    '401': A missing or invalid key returns 401.\n    '403': An account that has not been activated returns 403.\n    '402': If the workspace has no credits left, the API returns 402.\n  guidance: Do not put it in the URL. Keep it out of browser code, mobile apps, public repositories, screenshots,\n    and logs. Call SocialListeningAPI from your server so the key stays private.\n  sources:\n  - openapi/sociallisteningapi-openapi.yml\n\
  \  - https://sociallisteningapi.com/docs/authentication\n- name: MCP OAuth\n  type: oauth2\n  applies_to: Remote MCP server https://api.sociallisteningapi.com/mcp\n  flows:\n    authorizationCode:\n      authorizationUrl: https://api.sociallisteningapi.com/authorize\n      tokenUrl: https://api.sociallisteningapi.com/token\n      revocationUrl: https://api.sociallisteningapi.com/revoke\n      pkce: S256\n      scopes:\n      - mcp\n      - mcp:search\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - none\n  bearer_methods:\n  - header\n  sources:\n  - https://api.sociallisteningapi.com/.well-known/oauth-authorization-server (200)\n  - https://api.sociallisteningapi.com/.well-known/oauth-protected-resource/mcp (200)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/authentication/sociallisteningapi-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Social Listening
- Social Media
- Search
- Brand Monitoring
- Market Research
- MCP
- Reddit
- LinkedIn
---
