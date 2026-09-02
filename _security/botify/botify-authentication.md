---
api_key_in:
- header
api_specs:
- filename: botify-analysis-api-openapi.yml
  format: yaml
  label: Botify Analysis API
  slug: botify-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-analysis-api-openapi.yml
- filename: botify-collections-api-openapi.yml
  format: yaml
  label: Botify Collections API
  slug: botify-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-collections-api-openapi.yml
- filename: botify-datasource-api-openapi.yml
  format: yaml
  label: Botify Datasource API
  slug: botify-datasource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-datasource-api-openapi.yml
- filename: botify-job-api-openapi.yml
  format: yaml
  label: Botify Job API
  slug: botify-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-job-api-openapi.yml
- filename: botify-keywordsgroups-api-openapi.yml
  format: yaml
  label: Botify Keywords Groups API
  slug: botify-keywordsgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-keywordsgroups-api-openapi.yml
- filename: botify-project-api-openapi.yml
  format: yaml
  label: Botify Project API
  slug: botify-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-project-api-openapi.yml
- filename: botify-projectquery-api-openapi.yml
  format: yaml
  label: Botify Project Query API
  slug: botify-projectquery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-projectquery-api-openapi.yml
- filename: botify-user-api-openapi.yml
  format: yaml
  label: Botify User API
  slug: botify-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/openapi/botify-user-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Botify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Botify secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Botify
provider_slug: botify
scheme_count: 2
schemes:
- applies_to: https://api.botify.com/v1
  in: header
  name: DjangoRestToken
  parameter: Authorization
  rotation: A token can be regenerated from the account page; regenerating immediately invalidates the previous token, so clients must be updated on rotation. Botify publishes no expiry or forced-rotation policy.
  scheme_format: 'Authorization: Token <YOUR_TOKEN>'
  scopes: none
  sources:
  - openapi/botify-api-swagger.json
  - https://developers.botify.com/docs/getting-started
  - https://developers.botify.com/docs/querying-seo-data
  token_source: Botify application account page (https://app.botify.com/<username>/account). API access may need to be enabled on the account by Botify.
  type: apiKey
- applies_to: https://mcp.botify.com/
  bearer_methods:
  - header
  dynamic_client_registration: https://app.botify.com/oauth/register/
  flows:
    authorizationCode:
      authorizationUrl: https://app.botify.com/oauth/authorize
      refreshUrl: https://app.botify.com/oauth/token/
      scopes:
        mcp_read_write: Read and write access to the Botify Agents MCP surface.
      tokenUrl: https://app.botify.com/oauth/token/
  introspection: https://app.botify.com/oauth/introspect/
  name: BotifyMCPOAuth
  pkce: S256
  revocation: https://app.botify.com/oauth/revoke/
  sources:
  - https://app.botify.com/.well-known/oauth-authorization-server
  - https://mcp.botify.com/.well-known/oauth-protected-resource
  type: oauth2
slug: botify-authentication
source_filename: botify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: openapi/botify-api-swagger.json\ndocs: https://developers.botify.com/docs/getting-started\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    Two independent auth systems. The REST API uses one long-lived, per-user API token with no scopes, no\n    expiry and no rotation policy published beyond \"regenerating immediately invalidates the previous token\".\n    The MCP server uses a full OAuth 2.1 stack (authorization code + PKCE S256 + dynamic client registration)\n    on a separate authorization server. Nothing bridges the two.\nschemes:\n- name: DjangoRestToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_format: 'Authorization: Token <YOUR_TOKEN>'\n  applies_to: https://api.botify.com/v1\n  scopes: none\n  token_source: >-\n    Botify application account page (https://app.botify.com/<username>/account). API access may need to be\n    enabled on the account by Botify.\n\
  \  rotation: >-\n    A token can be regenerated from the account page; regenerating immediately invalidates the previous token,\n    so clients must be updated on rotation. Botify publishes no expiry or forced-rotation policy.\n  sources:\n  - openapi/botify-api-swagger.json\n  - https://developers.botify.com/docs/getting-started\n  - https://developers.botify.com/docs/querying-seo-data\n- name: BotifyMCPOAuth\n  type: oauth2\n  applies_to: https://mcp.botify.com/\n  flows:\n    authorizationCode:\n      authorizationUrl: https://app.botify.com/oauth/authorize\n      tokenUrl: https://app.botify.com/oauth/token/\n      refreshUrl: https://app.botify.com/oauth/token/\n      scopes:\n        mcp_read_write: Read and write access to the Botify Agents MCP surface.\n  pkce: S256\n  dynamic_client_registration: https://app.botify.com/oauth/register/\n  revocation: https://app.botify.com/oauth/revoke/\n  introspection: https://app.botify.com/oauth/introspect/\n  bearer_methods:\n  - header\n\
  \  sources:\n  - https://app.botify.com/.well-known/oauth-authorization-server\n  - https://mcp.botify.com/.well-known/oauth-protected-resource\ngaps:\n- No OpenID Connect discovery document is published (app.botify.com/.well-known/openid-configuration returns the SPA HTML shell, not OIDC metadata).\n- The REST API token is unscoped and long-lived; there is no read-only credential for the REST surface.\n- No mTLS, no signed-request scheme, no IP allow-listing documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botify/refs/heads/main/authentication/botify-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- SEO
- Organic search
- Web Crawling
- Log Analysis
- search-console
- Marketing Analytics
- AI Search
- Data Export
- MCP
- agent-native
---
