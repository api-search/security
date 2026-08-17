---
api_key_in:
- header
api_specs:
- filename: profound-external-api-openapi.json
  format: json
  label: Profound External API
  slug: profound-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-external-api-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Profound Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- refreshToken
overview: Profound secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and refreshToken flow(s).
provider_name: Profound
provider_slug: profound
scheme_count: 3
schemes:
- applied_to_operations: 125
  docs: https://docs.tryprofound.com/rest-api/authentication
  in: header
  name: APIKeyHeader
  parameter: X-API-Key
  recommended: true
  sources:
  - openapi/profound-external-api-openapi.json
  type: apiKey
- applied_to_operations: 125
  name: BearerAuth
  note: The same API key presented as Authorization Bearer. Also the fallback authentication method for the hosted MCP server, for service accounts that cannot complete a per-user OAuth flow.
  scheme: bearer
  sources:
  - openapi/profound-external-api-openapi.json
  type: http
- applies_to: https://mcp.tryprofound.com/mcp
  dynamic_client_registration: https://auth.tryprofound.com/oauth2/register
  flows:
  - authorizationUrl: https://auth.tryprofound.com/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://auth.tryprofound.com/oauth2/token
  - deviceAuthorizationUrl: https://auth.tryprofound.com/oauth2/device_authorization
    flow: deviceCode
  - flow: refreshToken
    tokenUrl: https://auth.tryprofound.com/oauth2/token
  issuer: https://auth.tryprofound.com
  name: MCP OAuth 2.1
  scopes:
  - openid
  - profile
  - email
  - offline_access
  see: scopes/profound-scopes.yml
  sources:
  - https://mcp.tryprofound.com/.well-known/oauth-authorization-server
  - https://docs.tryprofound.com/mcp/authentication
  type: oauth2
slug: profound-authentication
source_filename: profound-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/profound-external-api-openapi.json\ndocs: https://docs.tryprofound.com/rest-api/authentication\nnote: >-\n  Derived mechanically from the OpenAPI securitySchemes, then upgraded from the\n  docs. Profound runs two distinct authentication models: the REST API is\n  API-key only, while the hosted MCP server is OAuth 2.1 with an API-key bearer\n  fallback. The spec alone shows only the first of the two.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - deviceCode\n  - refreshToken\n  oauth2_applies_to: mcp\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  applied_to_operations: 125\n  recommended: true\n  sources:\n  - openapi/profound-external-api-openapi.json\n  docs: https://docs.tryprofound.com/rest-api/authentication\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applied_to_operations: 125\n  sources:\n\
  \  - openapi/profound-external-api-openapi.json\n  note: >-\n    The same API key presented as Authorization Bearer. Also the fallback\n    authentication method for the hosted MCP server, for service accounts that\n    cannot complete a per-user OAuth flow.\n- name: MCP OAuth 2.1\n  type: oauth2\n  applies_to: https://mcp.tryprofound.com/mcp\n  issuer: https://auth.tryprofound.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tryprofound.com/oauth2/authorize\n    tokenUrl: https://auth.tryprofound.com/oauth2/token\n    pkce: [S256]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.tryprofound.com/oauth2/device_authorization\n  - flow: refreshToken\n    tokenUrl: https://auth.tryprofound.com/oauth2/token\n  scopes: [openid, profile, email, offline_access]\n  dynamic_client_registration: https://auth.tryprofound.com/oauth2/register\n  sources:\n  - https://mcp.tryprofound.com/.well-known/oauth-authorization-server\n  - https://docs.tryprofound.com/mcp/authentication\n\
  \  see: scopes/profound-scopes.yml\nkey_management:\n  location: Platform → Settings → API Keys\n  creation_requires: name (min 3 characters) and an expiration date\n  expiration_required: true\n  shown_once: true\n  revocable: true\n  env_var: PROFOUND_API_KEY\n  note: >-\n    Mandatory expiry on every key is a genuinely good default — most catalog\n    providers issue non-expiring keys. Keys cannot be retrieved after creation.\naccess_gate:\n  plan: Enterprise\n  request_required: true\n  contact: mailto:support@tryprofound.com\n  note: >-\n    API access is not self-serve on any plan. Enterprise customers must request\n    it from support before the API Keys tab appears in the platform.\nscoping:\n  granularity: organization\n  note: >-\n    A key grants access to all data belonging to its organization — categories,\n    regions and category reports. There are no per-resource scopes or read/write\n    separation on the REST API.\nsso:\n  supported: true\n  protocols: [SAML, OIDC]\n\
  \  docs: https://docs.tryprofound.com/platform-config/authentication/sso-overview\n  note: Platform sign-in for customer users; unrelated to API authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/authentication/profound-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- AI
- Answer Engine Optimization
- AEO
- AI Search
- Generative Engine Optimization
- Marketing
- Analytics
- Agent Analytics
- Brand Visibility
- Citations
- MCP
---
