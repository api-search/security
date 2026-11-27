---
anonymous_access: false
api_key_in: []
api_specs:
- filename: callforme-tel-account-api-openapi.yml
  format: yaml
  label: CallForMe Account API
  slug: callforme-tel-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-account-api-openapi.yml
- filename: callforme-tel-batches-api-openapi.yml
  format: yaml
  label: CallForMe Batches API
  slug: callforme-tel-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-batches-api-openapi.yml
- filename: callforme-tel-businesses-api-openapi.yml
  format: yaml
  label: CallForMe Businesses API
  slug: callforme-tel-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-businesses-api-openapi.yml
- filename: callforme-tel-calls-api-openapi.yml
  format: yaml
  label: CallForMe Calls API
  slug: callforme-tel-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-calls-api-openapi.yml
- filename: callforme-tel-pricing-api-openapi.yml
  format: yaml
  label: CallForMe Pricing API
  slug: callforme-tel-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-pricing-api-openapi.yml
- filename: callforme-tel-setups-api-openapi.yml
  format: yaml
  label: CallForMe Setups API
  slug: callforme-tel-setups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-setups-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CallForMe Authentication
name_suffix: Authentication
oauth_flows: []
overview: CallForMe secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CallForMe
provider_slug: callforme-tel
scheme_count: 3
schemes:
- description: 'cfm_... key. Optional: without it, POST /v1/calls returns 402 with a setup link.'
  header: 'Authorization: Bearer cfm_your_key'
  how_to_obtain: From the first call (a keyless POST /calls returns a one-time setup link and the retry returns account_key once), or create one at https://callforme.tel/account.
  key_prefix: cfm_
  name: bearer
  scheme: bearer
  sources:
  - openapi/callforme-tel-openapi.yml
  - https://callforme.tel/docs/rest-api.md
  surface: REST API (https://callforme.tel/v1)
  type: http
- authorization_endpoint: https://callforme.tel/oauth/authorize
  client_id_metadata_document_supported: true
  description: Remote MCP, streamable HTTP, stateless, with standard MCP authorization (OAuth). The client's Connect step creates the account; the client keeps the token.
  discovery:
  - https://callforme.tel/.well-known/oauth-protected-resource
  - https://callforme.tel/.well-known/oauth-authorization-server
  - https://callforme.tel/.well-known/openid-configuration
  dynamic_client_registration: true
  flows:
  - authorization_code
  - refresh_token
  issuer: https://callforme.tel
  name: mcp-oauth
  pkce: S256
  registration_endpoint: https://callforme.tel/oauth/register
  revocation_endpoint: https://callforme.tel/oauth/revoke
  scopes:
  - calls
  sources:
  - https://callforme.tel/docs/mcp.md
  - well-known/callforme-tel-oauth-authorization-server.json
  surface: MCP (https://callforme.tel/mcp)
  token_endpoint: https://callforme.tel/oauth/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
- description: 'Key alternatives for clients without OAuth: https://callforme.tel/mcp/k/<your key> (key in the URL), or https://callforme.tel/mcp with an Authorization: Bearer cfm_... header. https://callforme.tel/mcp/open needs no auth and returns a setup link per session.'
  name: mcp-key
  sources:
  - https://callforme.tel/docs/mcp.md
  surface: MCP
  type: apiKey
slug: callforme-tel-authentication
source_filename: callforme-tel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource:\n- https://callforme.tel/docs/rest-api.md\n- https://callforme.tel/docs/mcp.md\ndocs: https://callforme.tel/docs/rest-api\ndocs_mcp: https://callforme.tel/docs/mcp\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  surface: REST API (https://callforme.tel/v1)\n  description: 'cfm_... key. Optional: without it, POST /v1/calls returns 402 with a setup link.'\n  header: 'Authorization: Bearer cfm_your_key'\n  key_prefix: cfm_\n  how_to_obtain: From the first call (a keyless POST /calls returns a one-time setup link and the retry returns account_key once), or create one\n    at https://callforme.tel/account.\n  sources:\n  - openapi/callforme-tel-openapi.yml\n  - https://callforme.tel/docs/rest-api.md\n- name: mcp-oauth\n  type: oauth2\n  surface: MCP (https://callforme.tel/mcp)\n  description: Remote MCP, streamable HTTP, stateless, with standard MCP authorization (OAuth). The\
  \ client's Connect step creates the account;\n    the client keeps the token.\n  sources:\n  - https://callforme.tel/docs/mcp.md\n  - well-known/callforme-tel-oauth-authorization-server.json\n  flows:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  scopes:\n  - calls\n  issuer: https://callforme.tel\n  authorization_endpoint: https://callforme.tel/oauth/authorize\n  token_endpoint: https://callforme.tel/oauth/token\n  registration_endpoint: https://callforme.tel/oauth/register\n  revocation_endpoint: https://callforme.tel/oauth/revoke\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  discovery:\n  - https://callforme.tel/.well-known/oauth-protected-resource\n  - https://callforme.tel/.well-known/oauth-authorization-server\n  - https://callforme.tel/.well-known/openid-configuration\n- name: mcp-key\n  type: apiKey\n  surface: MCP\n  description: 'Key\
  \ alternatives for clients without OAuth: https://callforme.tel/mcp/k/<your key> (key in the URL), or https://callforme.tel/mcp\n    with an Authorization: Bearer cfm_... header. https://callforme.tel/mcp/open needs no auth and returns a setup link per session.'\n  sources:\n  - https://callforme.tel/docs/mcp.md\nkeyless_operations:\n- planCall\n- findBusiness\n- pricing\n- waitForSetup\nnote: OAuth metadata (scope \"calls\", PKCE S256, dynamic client registration) is read from the published well-known discovery documents; the OpenAPI\n  declares only the bearer scheme.\nscopes: scopes/callforme-tel-scopes.yml\n"
source_yaml_url: https://artifacts.apis.io/callforme-tel/authentication/callforme-tel-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- AI Agents
- Voice
- Phone Calls
- Telephony
- MCP
- REST API
---
