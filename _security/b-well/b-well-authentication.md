---
api_key_in:
- header
api_specs:
- filename: b-well-users-api-openapi.yml
  format: yaml
  label: b.well Users API
  slug: b-well-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/openapi/b-well-users-api-openapi.yml
- filename: b-well-webhook-api-openapi.yml
  format: yaml
  label: b.well Webhook API
  slug: b-well-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/openapi/b-well-webhook-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: B Well Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- tokenExchange
overview: b.well secures its APIs with oauth2 and apiKey across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and tokenExchange flow(s).
provider_name: b.well
provider_slug: b-well
scheme_count: 7
schemes:
- description: HMAC-SHA512 signature over the canonical signed-header set; the signature is carried in the Authorization header.
  in: header
  name: HMACAuth
  parameter: Authorization
  sources:
  - openapi/b-well-user-data-operations-openapi.json
  type: apiKey
- description: The Base64 encoded SHA512 hash of request content.
  in: header
  name: HMACContentSHA512
  parameter: x-bwell-content-sha512
  sources:
  - openapi/b-well-user-data-operations-openapi.json
  type: apiKey
- description: The DNS Host associated with the request.
  in: header
  name: HMACHost
  parameter: Host
  sources:
  - openapi/b-well-user-data-operations-openapi.json
  type: apiKey
- description: UTC Timestamp in RFC1123 format.
  in: header
  name: HMACDate
  parameter: x-bwell-date
  sources:
  - openapi/b-well-user-data-operations-openapi.json
  type: apiKey
- description: Client specific user authentication token.
  in: header
  name: HMACClientUserToken
  parameter: x-bwell-client-user-token
  sources:
  - openapi/b-well-user-data-operations-openapi.json
  type: apiKey
- description: Client key. Provided to the client by b.well.
  in: header
  name: HMACClientKey
  parameter: x-bwell-client-key
  sources:
  - openapi/b-well-user-data-operations-openapi.json
  type: apiKey
- description: b.well access token used on the Application APIs, the FHIR Server and the MCP server.
  name: BearerToken
  scheme: bearer
  sources:
  - https://developer.bwell.com/docs/system-auth
  - https://developer.bwell.com/docs/mcp-anthropic
  type: http
slug: b-well-authentication
source_filename: b-well-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: openapi/b-well-user-data-operations-openapi.json\ndocs: https://developer.bwell.com/docs/auth-overview\nnotes: >-\n  b.well uses OAuth 2.0 for authentication and scope-based authorization across all\n  APIs and services, in two patterns: token exchange with OIDC for end-user context,\n  and client credentials for system context. The published User Data Operations REST\n  API additionally requires HMAC-SHA512 request signing over a canonical set of\n  b.well headers, which is what the derived scheme list below captures. The FHIR\n  hosts publish an anonymous SMART-on-FHIR configuration document naming the real\n  authorization, token, revocation, userinfo and JWKS endpoints (AWS Cognito).\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - tokenExchange\npatterns:\n- name: End-User Authentication\n  model: OAuth 2.0 Token Exchange with OpenID Connect\n  docs: https://developer.bwell.com/docs/end-user-auth\n\
  \  description: >-\n    Users authenticate through the integrating application's own Identity Provider.\n    b.well exchanges that OIDC ID token for a b.well access token, preserving user\n    identity across systems and enabling SSO. Used by the Web/Kotlin/Swift SDKs, the\n    Application APIs (GraphQL + REST), and every MCP tool call.\n  example: https://developer.bwell.com/docs/oauth-token-exchange\n  refresh: https://developer.bwell.com/docs/example-token-refresh\n- name: System Authentication\n  model: OAuth 2.0 Client Credentials (RFC 6749 §4.4)\n  docs: https://developer.bwell.com/docs/system-auth\n  description: >-\n    Server-to-server access without user context, for bulk FHIR operations, analytics\n    and data synchronization. Client ID and secret are exchanged at POST\n    {base_url}/oauth2/token for a system-scoped bearer token; typical lifetime 3600s.\n  token_endpoint_pattern: '{fhir_base_url}/oauth2/token'\n  bearer_header: 'Authorization: Bearer {access_token}'\n- name:\
  \ HMAC request signing\n  model: HMAC-SHA512 over canonical b.well headers\n  applies_to: openapi/b-well-user-data-operations-openapi.json\n  signed_headers:\n  - x-bwell-date\n  - host\n  - x-bwell-client-user-token\n  - x-bwell-client-key\n  - x-bwell-content-sha512\n  authorization_header_form: 'HMAC-SHA512 SignedHeaders=x-bwell-date;host;x-bwell-client-user-token;x-bwell-client-key;x-bwell-content-sha512&Signature=<hmac-sha512-signature>'\nsmart_configuration:\n  production:\n    file: well-known/b-well-smart-configuration.json\n    source: https://fhir.icanbwell.com/.well-known/smart-configuration\n    issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_Y8fODO5Z7\n    authorization_endpoint: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/authorize\n    token_endpoint: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/token\n    revocation_endpoint: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/revoke\n    userinfo_endpoint: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/userInfo\n\
  \    jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_Y8fODO5Z7/.well-known/jwks.json\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    id_token_signing_alg_values_supported: [RS256]\n    response_types_supported: [code, token]\n  sandbox:\n    file: well-known/b-well-smart-configuration-sandbox.json\n    source: https://fhir.client-sandbox.icanbwell.com/.well-known/smart-configuration\n    issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_yiNhNGXZ7\nschemes:\n- name: HMACAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC-SHA512 signature over the canonical signed-header set; the signature\n    is carried in the Authorization header.\n  sources:\n  - openapi/b-well-user-data-operations-openapi.json\n- name: HMACContentSHA512\n  type: apiKey\n  in: header\n  parameter: x-bwell-content-sha512\n  description: The Base64 encoded SHA512 hash of request content.\n  sources:\n  - openapi/b-well-user-data-operations-openapi.json\n\
  - name: HMACHost\n  type: apiKey\n  in: header\n  parameter: Host\n  description: The DNS Host associated with the request.\n  sources:\n  - openapi/b-well-user-data-operations-openapi.json\n- name: HMACDate\n  type: apiKey\n  in: header\n  parameter: x-bwell-date\n  description: UTC Timestamp in RFC1123 format.\n  sources:\n  - openapi/b-well-user-data-operations-openapi.json\n- name: HMACClientUserToken\n  type: apiKey\n  in: header\n  parameter: x-bwell-client-user-token\n  description: Client specific user authentication token.\n  sources:\n  - openapi/b-well-user-data-operations-openapi.json\n- name: HMACClientKey\n  type: apiKey\n  in: header\n  parameter: x-bwell-client-key\n  description: Client key. Provided to the client by b.well.\n  sources:\n  - openapi/b-well-user-data-operations-openapi.json\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: b.well access token used on the Application APIs, the FHIR Server and\n    the MCP server.\n  sources:\n  - https://developer.bwell.com/docs/system-auth\n\
  \  - https://developer.bwell.com/docs/mcp-anthropic\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/authentication/b-well-authentication.yml
summary_line: oauth2/apiKey · 7 schemes
tags:
- Company
- Health
- Healthcare
- Digital Health
- FHIR
- Health Data
- Interoperability
- Patient Access
- Health Records
- Model Context Protocol
---
