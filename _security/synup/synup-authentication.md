---
api_key_in: []
api_specs:
- filename: synup-automations-api-openapi.yml
  format: yaml
  label: Synup Automations API
  slug: synup-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-automations-api-openapi.yml
- filename: synup-connected-accounts-api-openapi.yml
  format: yaml
  label: Synup Connected Accounts API
  slug: synup-connected-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-connected-accounts-api-openapi.yml
- filename: synup-grid-rank-api-openapi.yml
  format: yaml
  label: Synup Grid Rank API
  slug: synup-grid-rank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-grid-rank-api-openapi.yml
- filename: synup-listings-api-openapi.yml
  format: yaml
  label: Synup Listings API
  slug: synup-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-listings-api-openapi.yml
- filename: synup-local-post-ideas-api-openapi.yml
  format: yaml
  label: Synup Local Post Ideas API
  slug: synup-local-post-ideas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-local-post-ideas-api-openapi.yml
- filename: synup-locations-api-openapi.yml
  format: yaml
  label: Synup Locations API
  slug: synup-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-locations-api-openapi.yml
- filename: synup-menus-api-openapi.yml
  format: yaml
  label: Synup Menus API
  slug: synup-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-menus-api-openapi.yml
- filename: synup-organizing-locations-api-openapi.yml
  format: yaml
  label: Synup Organizing locations API
  slug: synup-organizing-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-organizing-locations-api-openapi.yml
- filename: synup-posts-api-openapi.yml
  format: yaml
  label: Synup Posts API
  slug: synup-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-posts-api-openapi.yml
- filename: synup-profile-analytics-api-openapi.yml
  format: yaml
  label: Synup Profile Analytics API
  slug: synup-profile-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-profile-analytics-api-openapi.yml
- filename: synup-rankings-api-openapi.yml
  format: yaml
  label: Synup Rankings API
  slug: synup-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-rankings-api-openapi.yml
- filename: synup-review-campaigns-api-openapi.yml
  format: yaml
  label: Synup Review Campaigns API
  slug: synup-review-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-review-campaigns-api-openapi.yml
- filename: synup-reviews-api-openapi.yml
  format: yaml
  label: Synup Reviews API
  slug: synup-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-reviews-api-openapi.yml
- filename: synup-reviews-review-sources-api-openapi.yml
  format: yaml
  label: Synup Reviews/Review Sources API
  slug: synup-reviews-review-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-reviews-review-sources-api-openapi.yml
- filename: synup-social-api-openapi.yml
  format: yaml
  label: Synup Social API
  slug: synup-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-social-api-openapi.yml
- filename: synup-social-post-ideas-api-openapi.yml
  format: yaml
  label: Synup Social Post Ideas API
  slug: synup-social-post-ideas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-social-post-ideas-api-openapi.yml
- filename: synup-user-management-api-openapi.yml
  format: yaml
  label: Synup User Management API
  slug: synup-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-user-management-api-openapi.yml
- filename: synup-webhooks-api-openapi.yml
  format: yaml
  label: Synup Webhooks API
  slug: synup-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-webhooks-api-openapi.yml
- filename: synup-webhooks-webhooks-api-openapi.yml
  format: yaml
  label: Synup Webhooks/Webhooks API
  slug: synup-webhooks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/openapi/synup-webhooks-webhooks-api-openapi.yml
auth_types: []
description: Synup v4 is API-key authenticated with a custom Authorization scheme. The published OpenAPI documents declare no components.securitySchemes; instead every operation declares Authorization as a required HEADER PARAMETER. The MCP server adds a full OAuth 2.1 path on top of the same credential.
kind: authentication
layout: security
method: searched
name: Synup Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synup declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Synup
provider_slug: synup
scheme_count: 5
schemes:
- declared_in_spec: per-operation header parameter on 209 of 210 operations
  description: The primary REST credential. Note the literal "API " prefix — this is not Bearer.
  evidence:
    body: '{"data":{"allLocations":null},"errors":[{"message":"SY90005:Invalid token"}]}'
    http_status: 401
    probed: '2026-08-13'
    url: https://api.synup.com/api/v4/locations
  example: 'Authorization: API T9V35W3xxxxxxxxxxx'
  format: API <your_api_key>
  id: api_key_header
  in: header
  issued_at: Synup workspace -> Settings -> Integrations -> name the key -> Generate
  name: Authorization
  scope: account-wide; no scoping or per-resource permissions are published for REST keys
  type: apiKey
- authorization_endpoint: https://mcp-agent.synup.com/oauth/mcp/authorize
  description: OAuth 2.1 with PKCE and dynamic client registration, used by MCP clients that sign in through the browser.
  discovery: https://mcp-agent.synup.com/.well-known/oauth-authorization-server
  evidence:
    http_status: 200
    probed: '2026-08-13'
    url: https://mcp-agent.synup.com/.well-known/oauth-authorization-server
  flow: authorization_code
  id: mcp_oauth
  issuer: https://mcp-agent.synup.com
  jwks_uri: https://mcp-agent.synup.com/.well-known/jwks.json
  pkce: S256
  registration_endpoint: https://mcp-agent.synup.com/oauth/mcp/register
  require_state_parameter: true
  revocation_endpoint: https://mcp-agent.synup.com/oauth/mcp/revoke
  scopes:
  - mcp:read
  - mcp:write
  token_endpoint: https://mcp-agent.synup.com/oauth/mcp/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
- companion_headers:
  - X-user-email
  - X-access-mode
  description: The same Synup API key passed to the MCP server, optionally with X-user-email. Used by editor-based clients.
  env_vars:
  - SYNUP_API_KEY
  - SYNUP_USER_EMAIL
  id: mcp_api_key
  in: header
  name: X-api-key
  type: apiKey
- description: 'Authorization: Bearer accepting an API key, an encoded credential, or a Synup token, on the MCP surface only.'
  id: mcp_bearer
  scheme: bearer
  type: http
- description: 'Downstream, per-directory OAuth: the Connected Accounts endpoints broker Google Business Profile, Facebook and Apple connections on behalf of a customer. This is Synup calling out, not Synup authenticating you.'
  docs: https://developer.synup.com/connected-accounts-custom-endpoint-300825
  flow: authorization_code
  id: connected_accounts_oauth
  third_party: true
  type: oauth2
slug: synup-authentication
source_filename: synup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Synup API authentication\ngenerated: '2026-08-13'\nmethod: searched\nsource: https://developer.synup.com/synup-local-seo-api-getting-started-doc-824500\ndocs:\n- https://developer.synup.com/synup-local-seo-api-getting-started-doc-824500\n- https://developer.synup.com/synup-mcp-getting-connected-doc-2070739\ndescription: Synup v4 is API-key authenticated with a custom Authorization scheme. The published OpenAPI\n  documents declare no components.securitySchemes; instead every operation declares Authorization as a\n  required HEADER PARAMETER. The MCP server adds a full OAuth 2.1 path on top of the same credential.\nsummary:\n  rest: api-key (custom Authorization scheme)\n  mcp: oauth2.1 + api-key\n  oauth_for_rest: false\nschemes:\n- id: api_key_header\n  type: apiKey\n  in: header\n  name: Authorization\n  format: API <your_api_key>\n  example: 'Authorization: API T9V35W3xxxxxxxxxxx'\n  description: The primary REST credential. Note the literal \"API \" prefix — this\
  \ is not Bearer.\n  issued_at: Synup workspace -> Settings -> Integrations -> name the key -> Generate\n  scope: account-wide; no scoping or per-resource permissions are published for REST keys\n  declared_in_spec: per-operation header parameter on 209 of 210 operations\n  evidence:\n    url: https://api.synup.com/api/v4/locations\n    http_status: 401\n    body: '{\"data\":{\"allLocations\":null},\"errors\":[{\"message\":\"SY90005:Invalid token\"}]}'\n    probed: '2026-08-13'\n- id: mcp_oauth\n  type: oauth2\n  flow: authorization_code\n  description: OAuth 2.1 with PKCE and dynamic client registration, used by MCP clients that sign in through\n    the browser.\n  issuer: https://mcp-agent.synup.com\n  authorization_endpoint: https://mcp-agent.synup.com/oauth/mcp/authorize\n  token_endpoint: https://mcp-agent.synup.com/oauth/mcp/token\n  registration_endpoint: https://mcp-agent.synup.com/oauth/mcp/register\n  revocation_endpoint: https://mcp-agent.synup.com/oauth/mcp/revoke\n  jwks_uri:\
  \ https://mcp-agent.synup.com/.well-known/jwks.json\n  scopes:\n  - mcp:read\n  - mcp:write\n  pkce: S256\n  require_state_parameter: true\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  discovery: https://mcp-agent.synup.com/.well-known/oauth-authorization-server\n  evidence:\n    url: https://mcp-agent.synup.com/.well-known/oauth-authorization-server\n    http_status: 200\n    probed: '2026-08-13'\n- id: mcp_api_key\n  type: apiKey\n  in: header\n  name: X-api-key\n  description: The same Synup API key passed to the MCP server, optionally with X-user-email. Used by\n    editor-based clients.\n  companion_headers:\n  - X-user-email\n  - X-access-mode\n  env_vars:\n  - SYNUP_API_KEY\n  - SYNUP_USER_EMAIL\n- id: mcp_bearer\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer accepting an API key, an encoded credential, or a Synup token, on\n    the MCP surface only.'\n- id: connected_accounts_oauth\n  type: oauth2\n  flow: authorization_code\n  third_party:\
  \ true\n  description: 'Downstream, per-directory OAuth: the Connected Accounts endpoints broker Google Business\n    Profile, Facebook and Apple connections on behalf of a customer. This is Synup calling out, not Synup\n    authenticating you.'\n  docs: https://developer.synup.com/connected-accounts-custom-endpoint-300825\nauthorization_model:\n  rest: No scopes. A key carries whatever the issuing account and user role can see; user roles are managed\n    through the User Management endpoints.\n  mcp: Two coarse scopes (mcp:read, mcp:write) plus an X-access-mode header (read|write) for key-authenticated\n    sessions.\ngaps:\n- components.securitySchemes is empty in every published OpenAPI document — the credential is documented\n  only as a per-operation header parameter, so generated SDKs and agents cannot discover it from the spec\n  alone.\n- No key rotation, expiry or scoping policy is published for REST API keys.\n- The custom \"API <key>\" Authorization scheme is not a registered\
  \ HTTP auth scheme; generic OpenAPI tooling\n  will not model it correctly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/authentication/synup-authentication.yml
summary_line: 5 schemes
tags:
- Local Marketing
- Listings Management
- Reputation Management
- Local SEO
- Reviews
- Social-Media
- Analytics
- Business Listings
- Review Management
- Agency Software
---
