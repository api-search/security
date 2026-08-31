---
api_key_in: []
api_specs:
- filename: service-cloud-bot-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Bot API
  slug: service-cloud-bot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-bot-api-openapi.yml
- filename: service-cloud-health-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Health API
  slug: service-cloud-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-health-api-openapi.yml
- filename: service-cloud-versions-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Versions API
  slug: service-cloud-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-versions-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Service Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Salesforce Service Cloud APIs secures its APIs with oauth2, openIdConnect, and http-bearer across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Salesforce Service Cloud APIs
provider_slug: service-cloud
scheme_count: 4
schemes:
- description: chatbotAuth supports authorization code and implicit OAuth flows.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes:
    - chatbot_api
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: implicit
    scopes:
    - chatbot_api
  name: chatbotAuth
  sources:
  - openapi/service-cloud-einstein-bots-openapi.yml
  surface: Einstein Bots Runtime API
  type: oauth2
- description: Salesforce OAuth access token obtained using the JWT Bearer flow. Use the chatbot_api scope with this flow to enable access to the Einstein Bots services.
  name: jwtBearer
  scheme: bearer
  sources:
  - openapi/service-cloud-einstein-bots-openapi.yml
  surface: Einstein Bots Runtime API
  type: http
- description: Every REST call carries the OAuth access token. The token also determines the INSTANCE — the token response returns instance_url, and the API base is that instance_url plus /services/data/v67.0. Never hard-code a host.
  header: 'Authorization: Bearer <access_token>'
  name: platform-bearer
  scheme: bearer
  surface: Salesforce Platform REST API (sObjects, Query, Search, Composite)
  type: http
- description: MCP clients authenticate with OAuth 2.0 Authorization Code with PKCE against an External Client App consumer key created by a Salesforce admin, requesting the mcp_api scope.
  name: mcp-jwt
  probed: POST tools/list without a token → 401 {"errors":[{"message":"JWT Token is required"}]}
  scheme: bearer
  surface: Salesforce Hosted MCP Servers
  type: http
slug: service-cloud-authentication
source_filename: service-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://login.salesforce.com/.well-known/openid-configuration (probed 200, 2026-08-27),\n  https://api.salesforce.com/.well-known/oauth-authorization-server (probed 200),\n  https://api.salesforce.com/.well-known/oauth-protected-resource + the per-MCP-resource form (probed 200),\n  openapi/service-cloud-einstein-bots-openapi.yml, and\n  https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_understanding_authentication.htm\ndocs: https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_understanding_authentication.htm\nsummary:\n  primary: OAuth 2.0 bearer token\n  api_keys: false\n  api_key_note: >-\n    Salesforce issues NO API keys. Every API call carries an OAuth access token minted against a\n    specific org for a specific user. There is no static credential to leak and no test/live key prefix.\n  types: [oauth2, openIdConnect, http-bearer]\n  mutual_tls: >-\n    Supported\
  \ as an org-level setting (Enforce mutual authentication for the API), not declared in\n    any captured contract.\nauthorization_servers:\n  - issuer: https://login.salesforce.com\n    discovery: https://login.salesforce.com/.well-known/openid-configuration\n    http_status: 200\n    file: well-known/service-cloud-login-openid-configuration.json\n    endpoints:\n      authorization: https://login.salesforce.com/services/oauth2/authorize\n      token: https://login.salesforce.com/services/oauth2/token\n      userinfo: https://login.salesforce.com/services/oauth2/userinfo\n      jwks: https://login.salesforce.com/id/keys\n      revocation: https://login.salesforce.com/services/oauth2/revoke\n      introspection: https://login.salesforce.com/services/oauth2/introspect\n      registration: https://login.salesforce.com/services/oauth2/register\n    response_types_supported: [code, token, 'token id_token']\n    token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic,\
  \ private_key_jwt]\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    scopes: 36\n  - issuer: https://login.salesforce.com\n    discovery: https://api.salesforce.com/.well-known/oauth-authorization-server\n    http_status: 200\n    file: well-known/service-cloud-api-oauth-authorization-server.json\n    note: >-\n      A REDUCED view served from the API host: authorize/token/jwks only, no registration,\n      introspection or revocation, grant_types [authorization_code, refresh_token],\n      token_endpoint_auth_methods [client_secret_post], scopes [api, sfap_api, refresh_token,\n      einstein_gpt_api], code_challenge_methods [S256].\n  - name: Sandbox\n    login_host: https://test.salesforce.com\n    note: Sandboxes authenticate against test.salesforce.com, not login.salesforce.com.\nprotected_resources:\n  - resource: https://api.salesforce.com\n    metadata: https://api.salesforce.com/.well-known/oauth-protected-resource\n    http_status:\
  \ 200\n    scopes_supported: [api, sfap_api, refresh_token, einstein_gpt_api]\n  - resource: https://api.salesforce.com/platform/mcp/v1/platform/sobject-all\n    metadata: https://api.salesforce.com/.well-known/oauth-protected-resource/platform/mcp/v1/platform/sobject-all\n    http_status: 200\n    scopes_supported: [mcp_api, refresh_token]\n    caveat: The per-resource path is a wildcard generator — a bogus resource name also returns 200.\nschemes:\n  - name: chatbotAuth\n    type: oauth2\n    surface: Einstein Bots Runtime API\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n        tokenUrl: https://login.salesforce.com/services/oauth2/token\n        scopes: [chatbot_api]\n      - flow: implicit\n        authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n        scopes: [chatbot_api]\n    description: chatbotAuth supports authorization code and implicit OAuth flows.\n    sources: [openapi/service-cloud-einstein-bots-openapi.yml]\n\
  \  - name: jwtBearer\n    type: http\n    scheme: bearer\n    surface: Einstein Bots Runtime API\n    description: >-\n      Salesforce OAuth access token obtained using the JWT Bearer flow. Use the chatbot_api scope\n      with this flow to enable access to the Einstein Bots services.\n    sources: [openapi/service-cloud-einstein-bots-openapi.yml]\n  - name: platform-bearer\n    type: http\n    scheme: bearer\n    surface: 'Salesforce Platform REST API (sObjects, Query, Search, Composite)'\n    header: 'Authorization: Bearer <access_token>'\n    description: >-\n      Every REST call carries the OAuth access token. The token also determines the INSTANCE — the\n      token response returns instance_url, and the API base is that instance_url plus\n      /services/data/v67.0. Never hard-code a host.\n  - name: mcp-jwt\n    type: http\n    scheme: bearer\n    surface: Salesforce Hosted MCP Servers\n    probed: 'POST tools/list without a token → 401 {\"errors\":[{\"message\":\"JWT Token is\
  \ required\"}]}'\n    description: >-\n      MCP clients authenticate with OAuth 2.0 Authorization Code with PKCE against an External\n      Client App consumer key created by a Salesforce admin, requesting the mcp_api scope.\nflows:\n  - name: Authorization Code with PKCE\n    supported: true\n    pkce: S256\n    use: Interactive user consent; the flow MCP clients use.\n  - name: Refresh Token\n    supported: true\n  - name: JWT Bearer (private_key_jwt)\n    supported: true\n    use: >-\n      Server-to-server with no user interaction — the standard integration-user pattern for a\n      Service Cloud backend. Also the documented flow for Einstein Bots.\n  - name: Implicit\n    supported: true\n    note: Declared by the Einstein Bots spec. Deprecated by current OAuth guidance; prefer PKCE.\n  - name: Client Credentials\n    supported: true\n    note: Requires an execution user to be assigned on the connected app.\n  - name: Device Flow\n    supported: true\n    note: Used by `sf org login\
  \ device` in the CLI.\ntoken_shape:\n  access_token: opaque\n  id_token: 'JWT, RS256, verified against https://login.salesforce.com/id/keys'\n  instance_binding: >-\n    The token response includes instance_url and id. instance_url is the API base host for that\n    org — Service Cloud has no single global API host.\n  claims_supported:\n    [active, address, email, email_verified, family_name, given_name, is_app_installed, language,\n     locale, name, nickname, organization_id, phone_number, phone_number_verified, photos, picture,\n     preferred_username, profile, sub, updated_at, urls, user_id, user_type, zoneinfo]\nrelated:\n  scopes: scopes/service-cloud-scopes.yml\n  conventions: conventions/service-cloud-conventions.yml\n  conformance: conformance/service-cloud-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/authentication/service-cloud-authentication.yml
summary_line: oauth2/openIdConnect/http-bearer · 4 schemes
tags:
- Cloud
- CRM
- Customer-Service
- Enterprise
- Salesforce
- Support
---
