---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Theorg Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: The Org secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: The Org
provider_slug: theorg
scheme_count: 2
schemes:
- applies_to:
  - REST API
  - MCP endpoint
  description: 'All requests authenticate with an account-scoped API key passed in the X-Api-Key header. Keys are created from the developer subscription page after creating a free The Org account (each key is given an informative name). All requests must be made over HTTPS; plain HTTP calls fail. The same key authenticates the REST API and the MCP endpoint — the MCP docs state "Authentication uses your existing API key. No separate MCP sign-up is required."

    '
  in: header
  name: ApiKeyAuth
  parameter_name: X-Api-Key
  sources:
  - https://developers.theorg.com/api/get-started
  - https://developers.theorg.com/api/key-concepts
  - https://developers.theorg.com/mcp
  type: apiKey
- applies_to:
  - MCP endpoint
  description: 'An OAuth 2.1 authorization server (public client, authorization code + PKCE S256, RFC 7591 dynamic client registration) gates the MCP endpoint at https://api.theorg.com/v1.1/mcp. It is discoverable but UNDOCUMENTED: the key-concepts and MCP pages describe only X-Api-Key, while the API host serves live RFC 8414 and RFC 9728 metadata and an unauthenticated POST to the MCP endpoint answers 401 with ''WWW-Authenticate: Bearer realm="mcp", resource_metadata=..., scope=mcp''.

    '
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://api.theorg.com/oauth/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    scopes:
    - mcp
    tokenUrl: https://api.theorg.com/oauth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://api.theorg.com
  name: OAuth2
  registration_endpoint: https://api.theorg.com/oauth/register
  scopes_artifact: scopes/theorg-scopes.yml
  sources:
  - https://api.theorg.com/.well-known/oauth-authorization-server
  - https://api.theorg.com/.well-known/oauth-protected-resource
  type: oauth2
slug: theorg-authentication
source_filename: theorg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://developers.theorg.com/api/get-started\ndocs: https://developers.theorg.com/api/key-concepts\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: X-Api-Key\n  applies_to: [REST API, MCP endpoint]\n  description: >\n    All requests authenticate with an account-scoped API key passed in the\n    X-Api-Key header. Keys are created from the developer subscription page after\n    creating a free The Org account (each key is given an informative name). All\n    requests must be made over HTTPS; plain HTTP calls fail. The same key authenticates\n    the REST API and the MCP endpoint — the MCP docs state \"Authentication uses your\n    existing API key. No separate MCP sign-up is required.\"\n  sources:\n  - https://developers.theorg.com/api/get-started\n  - https://developers.theorg.com/api/key-concepts\n\
  \  - https://developers.theorg.com/mcp\n- name: OAuth2\n  type: oauth2\n  applies_to: [MCP endpoint]\n  issuer: https://api.theorg.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.theorg.com/oauth/authorize\n    tokenUrl: https://api.theorg.com/oauth/token\n    pkce_methods: [S256]\n    token_endpoint_auth_methods: [none]\n    scopes: [mcp]\n  registration_endpoint: https://api.theorg.com/oauth/register\n  dynamic_client_registration: true\n  description: >\n    An OAuth 2.1 authorization server (public client, authorization code + PKCE S256,\n    RFC 7591 dynamic client registration) gates the MCP endpoint at\n    https://api.theorg.com/v1.1/mcp. It is discoverable but UNDOCUMENTED: the\n    key-concepts and MCP pages describe only X-Api-Key, while the API host serves live\n    RFC 8414 and RFC 9728 metadata and an unauthenticated POST to the MCP endpoint\n    answers 401 with\n    'WWW-Authenticate: Bearer realm=\"mcp\", resource_metadata=..., scope=mcp'.\n\
  \  sources:\n  - https://api.theorg.com/.well-known/oauth-authorization-server\n  - https://api.theorg.com/.well-known/oauth-protected-resource\n  scopes_artifact: scopes/theorg-scopes.yml\naccepted_credentials:\n  note: >-\n    The MCP 401 body enumerates the accepted credential forms verbatim:\n    \"Missing credentials. Provide Authorization: Bearer, X-Api-Key, or the api_key\n    query parameter.\" The api_key query-string form is a credential-in-URL pattern\n    that leaks into logs, referrers and browser history; it is not documented on the\n    developer portal but the API accepts it.\n  forms:\n  - kind: bearer-token\n    location: Authorization header\n  - kind: api-key\n    location: X-Api-Key header\n  - kind: api-key\n    location: api_key query parameter\n    caution: credential in URL\ntransport: https-required\nkey_management:\n  create: https://theorg.com/subscription#api\n  rotation_policy: null\n  expiry: null\n  note: >-\n    Keys are created and named from the subscription\
  \ page. The Org publishes no key\n    rotation policy, expiry, or scoping model for API keys — a key is account-scoped\n    and carries full account privileges (\"Your API keys carry many privileges, so be\n    sure to keep them secure!\").\nx-evidence:\n  fetched: '2026-08-14'\n  probes:\n  - url: https://api.theorg.com/v1.1/mcp\n    method: POST\n    http_status: 401\n    note: unauthenticated tools/list returns the Bearer challenge\n  - url: https://api.theorg.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://api.theorg.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theorg/refs/heads/main/authentication/theorg-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Organizational Charts
- People Data
- Sales Intelligence
- Prospecting
- Org Chart
- B2B Data
- MCP
- Contact Data
- Lead Generation
- Jobs
- Agents
---
