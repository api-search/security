---
anonymous_access: false
api_key_in: []
api_specs:
- filename: casatoo-pt-account-api-openapi.yml
  format: yaml
  label: Casatoo Account API
  slug: casatoo-pt-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-account-api-openapi.yml
- filename: casatoo-pt-likes-api-openapi.yml
  format: yaml
  label: Casatoo Likes API
  slug: casatoo-pt-likes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-likes-api-openapi.yml
- filename: casatoo-pt-listings-api-openapi.yml
  format: yaml
  label: Casatoo Listings API
  slug: casatoo-pt-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-listings-api-openapi.yml
- filename: casatoo-pt-locations-api-openapi.yml
  format: yaml
  label: Casatoo Locations API
  slug: casatoo-pt-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-locations-api-openapi.yml
- filename: casatoo-pt-saved-searches-api-openapi.yml
  format: yaml
  label: Casatoo Saved searches API
  slug: casatoo-pt-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-saved-searches-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Casatoo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Casatoo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Casatoo
provider_slug: casatoo-pt
scheme_count: 1
schemes:
- description: Authorization code grants delegated human access.
  flows:
  - authorizationUrl: https://oauth.casatoo.pt/oauth2/auth
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://oauth.casatoo.pt/oauth2/token
  name: casatooOAuth
  sources:
  - openapi/casatoo-pt-openapi.yml
  type: oauth2
slug: casatoo-pt-authentication
source_filename: casatoo-pt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://casatoo.pt/developers/agents\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: casatooOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.casatoo.pt/oauth2/auth\n    tokenUrl: https://oauth.casatoo.pt/oauth2/token\n    scopes: 8\n  description: Authorization code grants delegated human access.\n  sources:\n  - openapi/casatoo-pt-openapi.yml\ndocs: https://casatoo.pt/developers/agents\nderived_from: openapi/casatoo-pt-openapi.yml\nanonymous_access: Public reads need no account, key, or approval.\ndiscovery:\n  authorization_server: https://oauth.casatoo.pt/.well-known/oauth-authorization-server\n  openid_configuration: https://oauth.casatoo.pt/.well-known/openid-configuration\n  protected_resource_mcp: https://api.casatoo.pt/.well-known/oauth-protected-resource/mcp\nauthorization_server_metadata:\n  grant_types_supported:\n  - authorization_code\n\
  \  - implicit\n  - client_credentials\n  - refresh_token\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - none\n  registration_endpoint: https://api.casatoo.pt/api/v1/oauth/register\n  fetched: '2026-11-03'\nnotes: The user approves scopes in their browser; the agent never handles their password.\n  MCP clients follow the advertised protected-resource and authorization-server metadata\n  (e.g. codex mcp login casatoo --scopes listings:read,locations:read).\n"
source_yaml_url: https://artifacts.apis.io/casatoo-pt/authentication/casatoo-pt-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Real Estate
- Property Search
- Portugal
- Price-Tracking
- Mortgage
- MCP
- AI Agents
---
