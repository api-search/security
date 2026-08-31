---
api_key_in: []
auth_types: []
description: The Specright API v1.1.0 accepts three authentication schemes and layers a mandatory caller-identity header on top of all of them. Every business operation additionally requires x-user-id, which is not a security scheme in the OpenAPI sense but is marked required on all 45 non-token operations — an agent that supplies only a credential will be rejected.
kind: authentication
layout: security
method: searched
name: Specright Authentication
name_suffix: Authentication
oauth_flows: []
overview: Specright declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Specright
provider_slug: specright
scheme_count: 3
schemes:
- applied_to: All 45 operations under /specs, /specfamilies, /suppliers and /objects, including every bulk-job operation.
  description: API key granted by Specright to access the API. Documented as required on every operation outside /token. Keys are issued by Specright to customers and partners — there is no self-service key issuance.
  evidence: 'Reference lists "x-api-key | header | string | true | api key granted by Specright to access the API" on each operation, and closes each with "To perform this operation, you must be authenticated by means of one of the following methods: ApiKeyAuth, BearerAuth".'
  id: ApiKeyAuth
  in: header
  name: x-api-key
  type: apiKey
- bearer_format: JWT
  description: 'Access token obtained from POST /v1/token. Accepted as an alternative to the API key on all business operations. Confirmed live: an anonymous GET https://api.specright.com/v1 returns 401 with the response header "WWW-Authenticate: Bearer".'
  evidence: 'Probed 2026-08-28: https://api.specright.com/v1 -> 401, www-authenticate: Bearer'
  id: BearerAuth
  scheme: bearer
  type: http
- applied_to:
  - POST /token
  description: Used exclusively to call the token endpoint. POST /v1/token is the only operation whose documented method is BasicAuth.
  id: BasicAuth
  scheme: basic
  type: http
slug: specright-authentication
source_filename: specright-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: >-\n  https://developer.specright.com/ (the Specright API v1.1.0 reference, served inside the\n  developer portal's JavaScript bundle) and\n  https://login.specright.com/realms/Specright/.well-known/openid-configuration (200,\n  probed 2026-08-28).\ndocs: https://developer.specright.com/\nname: Specright API authentication\ndescription: >-\n  The Specright API v1.1.0 accepts three authentication schemes and layers a mandatory\n  caller-identity header on top of all of them. Every business operation additionally\n  requires x-user-id, which is not a security scheme in the OpenAPI sense but is marked\n  required on all 45 non-token operations — an agent that supplies only a credential will\n  be rejected.\n\napi_base: https://api.specright.com/v1\nsandbox_base: https://test.specright.com/v1\n\nschemes:\n  - id: ApiKeyAuth\n    type: apiKey\n    in: header\n    name: x-api-key\n    description: >-\n      API key granted by Specright\
  \ to access the API. Documented as required on every\n      operation outside /token. Keys are issued by Specright to customers and partners —\n      there is no self-service key issuance.\n    applied_to: >-\n      All 45 operations under /specs, /specfamilies, /suppliers and /objects, including\n      every bulk-job operation.\n    evidence: >-\n      Reference lists \"x-api-key | header | string | true | api key granted by Specright to\n      access the API\" on each operation, and closes each with \"To perform this operation,\n      you must be authenticated by means of one of the following methods: ApiKeyAuth,\n      BearerAuth\".\n  - id: BearerAuth\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      Access token obtained from POST /v1/token. Accepted as an alternative to the API key\n      on all business operations. Confirmed live: an anonymous GET\n      https://api.specright.com/v1 returns 401 with the response header\n      \"WWW-Authenticate:\
  \ Bearer\".\n    evidence: 'Probed 2026-08-28: https://api.specright.com/v1 -> 401, www-authenticate: Bearer'\n  - id: BasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Used exclusively to call the token endpoint. POST /v1/token is the only operation\n      whose documented method is BasicAuth.\n    applied_to: [POST /token]\n\nrequired_headers:\n  - name: x-user-id\n    in: header\n    required: true\n    description: >-\n      \"userid of the user making the request\" — the Specright user the call acts as. Marked\n      required: true on all 45 business operations. This is a second, orthogonal identity\n      axis: the API key or bearer token authenticates the integration, x-user-id selects\n      the acting principal, and Specright's Salesforce-side record permissions are then\n      evaluated against that user.\n    agent_note: >-\n      An agent must be given BOTH a credential and a Specright user identity. A 403 on a\n      well-formed request most often means\
  \ the x-user-id principal lacks record access,\n      not that the key is wrong.\n  - name: x-api-key\n    in: header\n    required: true\n    description: See ApiKeyAuth above. Documented as required even where BearerAuth is used.\n\ntoken_endpoint:\n  operation: POST /token\n  url: https://api.specright.com/v1/token\n  auth: BasicAuth\n  content_type: application/x-www-form-urlencoded\n  request_fields:\n    - name: grant_type\n      type: string\n      required: false\n    - name: refresh_token\n      type: string\n      required: false\n  response_fields:\n    - name: access_token\n      type: string\n      format: JWT\n    - name: token_type\n      type: string\n      value: bearer\n    - name: expires_in\n      type: integer\n      value: 3600\n      note: One hour. An agent holding a long-running session must refresh.\n    - name: refresh_token\n      type: string\n  responses: {200: token, 400: Bad Request, 401: Unauthorized}\n\nidentity_provider:\n  vendor: Keycloak\n  issuer:\
  \ https://login.specright.com/realms/Specright\n  realm: Specright\n  discovery: https://login.specright.com/realms/Specright/.well-known/openid-configuration\n  discovery_status: 200\n  token_endpoint: https://login.specright.com/realms/Specright/protocol/openid-connect/token\n  authorization_endpoint: https://login.specright.com/realms/Specright/protocol/openid-connect/auth\n  introspection_endpoint: https://login.specright.com/realms/Specright/protocol/openid-connect/token/introspect\n  userinfo_endpoint: https://login.specright.com/realms/Specright/protocol/openid-connect/userinfo\n  revocation_endpoint: https://login.specright.com/realms/Specright/protocol/openid-connect/revoke\n  end_session_endpoint: https://login.specright.com/realms/Specright/protocol/openid-connect/logout\n  jwks_uri: https://login.specright.com/realms/Specright/protocol/openid-connect/certs\n  registration_endpoint: https://login.specright.com/realms/Specright/clients-registrations/openid-connect\n  device_authorization_endpoint:\
  \ https://login.specright.com/realms/Specright/protocol/openid-connect/auth/device\n  grant_types_supported:\n    - authorization_code\n    - client_credentials\n    - implicit\n    - password\n    - refresh_token\n    - 'urn:ietf:params:oauth:grant-type:device_code'\n    - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    - 'urn:ietf:params:oauth:grant-type:token-exchange'\n    - 'urn:ietf:params:oauth:grant-type:uma-ticket'\n    - 'urn:openid:params:grant-type:ciba'\n  token_endpoint_auth_methods_supported:\n    - private_key_jwt\n    - client_secret_basic\n    - client_secret_post\n    - tls_client_auth\n    - client_secret_jwt\n  code_challenge_methods_supported: [plain, S256]\n  id_token_signing_alg_values_supported:\n    [PS384, RS384, EdDSA, ES384, HS256, HS512, ES256, RS256, HS384, ES512, PS256, PS512, RS512]\n  note: >-\n    The developer portal's own JavaScript posts to this Keycloak token endpoint with scope\n    \"specright-api\", so the Keycloak realm — not just the /v1/token\
  \ shim — is the real\n    authorization server behind the bearer flow. mutualTLS (tls_client_auth) and\n    private_key_jwt are both advertised, which is a stronger client-authentication posture\n    than the API-key path the docs lead with.\n\nseparate_oauth_surface:\n  host: www.specright.com\n  issuer: https://www.specright.com\n  purpose: >-\n    A completely distinct OAuth authorization server, published by the WordPress MCP\n    adapter on the marketing site. Scope \"mcp\", PKCE S256, public clients only\n    (token_endpoint_auth_methods_supported: [\"none\"]). It has nothing to do with\n    api.specright.com and must not be confused with the Keycloak realm above.\n  see: ../mcp/specright-mcp.yml\n\nonboarding:\n  self_service: false\n  how_to_get_credentials: >-\n    Specright issues API keys and developer accounts to customers and partners on request.\n    The 2020-02-13 launch post directs prospective developers to a contact form, and the\n    reference's 403 description says\
  \ \"Please reach out to api@specright.com for assistance\".\n  contact: api@specright.com\n  portal: https://developer.specright.com/\n\ngaps:\n  - No published OpenAPI document, so securitySchemes cannot be read machine-side; every\n    field above is transcribed from the rendered reference or from the live OIDC document.\n  - The reference declares both ApiKeyAuth and BearerAuth as acceptable on the same\n    operations but never states precedence when both headers are sent.\n  - x-api-key appears twice in some published code samples (once with a literal example\n    value, once as API_KEY), which is a docs-generation artefact rather than a real\n    two-key requirement.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/specright/refs/heads/main/authentication/specright-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Specification Management
- Supply Chain
- Packaging
- Product Lifecycle Management
- Manufacturing
- Sustainability
- Supplier Collaboration
- Bill of Materials
- Salesforce
- Enterprise Software
---
