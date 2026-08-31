---
api_key_in:
- header
- query
api_specs:
- filename: crunchbase-data-autocomplete-api-openapi.yml
  format: yaml
  label: Crunchbase Autocomplete API
  slug: crunchbase-data-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-autocomplete-api-openapi.yml
- filename: crunchbase-data-deleted-entities-api-openapi.yml
  format: yaml
  label: Crunchbase Deleted Entities API
  slug: crunchbase-data-deleted-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-deleted-entities-api-openapi.yml
- filename: crunchbase-data-entity-api-openapi.yml
  format: yaml
  label: Crunchbase Entity API
  slug: crunchbase-data-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-entity-api-openapi.yml
- filename: crunchbase-data-metadata-api-openapi.yml
  format: yaml
  label: Crunchbase Metadata API
  slug: crunchbase-data-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-metadata-api-openapi.yml
- filename: crunchbase-data-search-api-openapi.yml
  format: yaml
  label: Crunchbase Search API
  slug: crunchbase-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-search-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: 'Crunchbase runs two independent authentication models. The REST Data API is a single account-level API key with no scopes and no user identity - the key IS the licence, and which of the six packages it is provisioned against determines which of the 109 operations it can call. The MCP server is separate: OAuth 2.1 with PKCE against www.crunchbase.com, executing as the signed-in Crunchbase user, gated by an MCP seat. A key does not work on MCP and an OAuth token does not work on the REST API.'
kind: authentication
layout: security
method: searched
name: Crunchbase Data Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Crunchbase secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Crunchbase
provider_slug: crunchbase-data
scheme_count: 3
schemes:
- description: API key passed as the X-cb-user-key request header. The only scheme declared by the six published OpenAPI documents, and the form Crunchbase's own cURL examples use. Preferred - it keeps a long-lived credential out of URLs and proxy logs.
  in: header
  name: ApiKeyAuthHeader
  parameter: X-cb-user-key
  sources:
  - openapi/crunchbase-data-advanced-financials-openapi.yml
  - openapi/crunchbase-data-core-financials-openapi.yml
  - openapi/crunchbase-data-firmographic-openapi.yml
  - openapi/crunchbase-data-insights-openapi.yml
  - openapi/crunchbase-data-predictions-insights-openapi.yml
  - openapi/crunchbase-data-predictions-openapi.yml
  - https://data.crunchbase.com/docs/using-the-api
  surface: REST Data API
  type: apiKey
- declared_in_spec: false
  description: The same key passed as the user_key query parameter, e.g. ?user_key=YOUR_API_KEY. Documented and supported but NOT declared in any of the six OpenAPI documents - a real gap between the contract and the docs.
  in: query
  name: userKeyQuery
  parameter: user_key
  sources:
  - https://data.crunchbase.com/docs/using-the-api
  surface: REST Data API
  type: apiKey
- authorizationUrl: https://www.crunchbase.com/oauth/authorize
  client_registration: Client ID Metadata Documents (CIMD) supported; Dynamic Client Registration explicitly NOT supported. Clients without CIMD need a client_id/client_secret pre-registered by a Crunchbase CSM and retrieved under Settings > Integrations > MCP.
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://www.crunchbase.com
  name: MCPOAuth
  pkce: true
  pkce_methods:
  - S256
  - plain
  revocationUrl: https://oauth.crunchbase.com/revoke
  scopes:
  - offline_access
  - lists.read
  sources:
  - https://www.crunchbase.com/.well-known/oauth-authorization-server
  - https://mcp.crunchbase.com/.well-known/oauth-protected-resource
  - https://data.crunchbase.com/docs/connecting-ai-tools
  surface: MCP server (https://mcp.crunchbase.com)
  tokenUrl: https://oauth.crunchbase.com/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
  type: oauth2
slug: crunchbase-data-authentication
source_filename: crunchbase-data-authentication.yml
source_heading: Authentication Profile
source_url: https://data.crunchbase.com/docs/using-the-api
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://data.crunchbase.com/docs/using-the-api\ndocs: https://data.crunchbase.com/docs/using-the-api\nsources:\n- https://data.crunchbase.com/docs/using-the-api\n- https://data.crunchbase.com/docs/calling-api-endpoints\n- https://data.crunchbase.com/docs/connecting-ai-tools\n- https://www.crunchbase.com/.well-known/oauth-authorization-server\n- https://mcp.crunchbase.com/.well-known/oauth-protected-resource\n- openapi/crunchbase-data-predictions-insights-openapi.yml\ndescription: >-\n  Crunchbase runs two independent authentication models. The REST Data API is a single\n  account-level API key with no scopes and no user identity - the key IS the licence,\n  and which of the six packages it is provisioned against determines which of the 109\n  operations it can call. The MCP server is separate: OAuth 2.1 with PKCE against\n  www.crunchbase.com, executing as the signed-in Crunchbase user, gated by an MCP seat.\n  A key does not\
  \ work on MCP and an OAuth token does not work on the REST API.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuthHeader\n  surface: REST Data API\n  type: apiKey\n  in: header\n  parameter: X-cb-user-key\n  description: >-\n    API key passed as the X-cb-user-key request header. The only scheme declared by the\n    six published OpenAPI documents, and the form Crunchbase's own cURL examples use.\n    Preferred - it keeps a long-lived credential out of URLs and proxy logs.\n  sources:\n  - openapi/crunchbase-data-advanced-financials-openapi.yml\n  - openapi/crunchbase-data-core-financials-openapi.yml\n  - openapi/crunchbase-data-firmographic-openapi.yml\n  - openapi/crunchbase-data-insights-openapi.yml\n  - openapi/crunchbase-data-predictions-insights-openapi.yml\n  - openapi/crunchbase-data-predictions-openapi.yml\n  - https://data.crunchbase.com/docs/using-the-api\n- name: userKeyQuery\n\
  \  surface: REST Data API\n  type: apiKey\n  in: query\n  parameter: user_key\n  description: >-\n    The same key passed as the user_key query parameter, e.g.\n    ?user_key=YOUR_API_KEY. Documented and supported but NOT declared in any of the six\n    OpenAPI documents - a real gap between the contract and the docs.\n  declared_in_spec: false\n  sources:\n  - https://data.crunchbase.com/docs/using-the-api\n- name: MCPOAuth\n  surface: MCP server (https://mcp.crunchbase.com)\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  issuer: https://www.crunchbase.com\n  authorizationUrl: https://www.crunchbase.com/oauth/authorize\n  tokenUrl: https://oauth.crunchbase.com/token\n  revocationUrl: https://oauth.crunchbase.com/revoke\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  scopes:\n  - offline_access\n  - lists.read\n  client_registration: >-\n    Client ID Metadata\
  \ Documents (CIMD) supported; Dynamic Client Registration\n    explicitly NOT supported. Clients without CIMD need a client_id/client_secret\n    pre-registered by a Crunchbase CSM and retrieved under Settings > Integrations > MCP.\n  sources:\n  - https://www.crunchbase.com/.well-known/oauth-authorization-server\n  - https://mcp.crunchbase.com/.well-known/oauth-protected-resource\n  - https://data.crunchbase.com/docs/connecting-ai-tools\nkey_issuance:\n  self_serve: false\n  where: Crunchbase UI - Account Settings > Integrations > Crunchbase API Key (\"Show Key\")\n  gate: >-\n    Full API access requires an Enterprise or Applications licence. Holders of the paid\n    Crunchbase Basic plan get a reduced Basic API. There is no free or trial API key.\n  support_contact: api@crunchbase.com\n  note: >-\n    Legacy keys are being retired. Each legacy key has been mapped to the data package\n    that mirrors its previous plan; see lifecycle/crunchbase-data-lifecycle.yml.\ntransport:\n  https_required:\
  \ true\n  http_response: 426\nauthorization_model:\n  rest: >-\n    No scopes and no roles. Authorization is package-shaped: the key is provisioned to\n    one of Fundamentals / Insights / Predictions (published as six OpenAPI documents),\n    and an operation outside that package is simply not callable. There is no way to\n    express least privilege within a key.\n  mcp: >-\n    Two OAuth scopes (offline_access, lists.read) plus a per-user MCP seat that\n    Crunchbase documents as carrying its highest level of data access including\n    predictions and insights. Notably, no lists.write scope is advertised even though\n    cb_list_create and cb_list_add_entities are documented write tools.\nobserved:\n  unauthenticated_response:\n    status: 401\n    body: '[{\"status\":401,\"code\":\"LA401\",\"message\":\"Unauthorized user_key\"}]'\n    note: >-\n      Probed 2026-08-14. Every path on api.crunchbase.com returns this, including\n      /.well-known/* - the origin authenticates ahead of\
  \ routing.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/authentication/crunchbase-data-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company Data
- Web Intelligence
- Funding Data
- Firmographics
- B2B Data
- Investor Data
- Reference Data
- Private Markets
- Predictions
- Market Insights
- MCP
- Fortune 1000
---
