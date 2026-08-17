---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: probed
name: Doubleverify Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: DoubleVerify secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: DoubleVerify
provider_slug: doubleverify
scheme_count: 3
schemes:
- applies_to: DV Neura MCP Server (https://mcp.doubleverify.com/mcp)
  authorization_server: https://dv-ciam.doubleverify.com/realms/pinnacle
  bearer_methods_supported:
  - header
  name: dv-neura-mcp-oauth
  protected_resource_metadata: https://mcp.doubleverify.com/.well-known/oauth-protected-resource/mcp
  rfc:
  - RFC 9728 (OAuth 2.0 Protected Resource Metadata)
  - RFC 6750 (Bearer token usage)
  scopes_required:
  - openid
  - email
  - profile
  source: probed
  type: oauth2
- applies_to: DV Pinnacle / DV Neura CIAM realm
  authorizationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth
  code_challenge_methods_supported:
  - plain
  - S256
  deviceAuthorizationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth/device
  endSessionUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/logout
  file: well-known/doubleverify-openid-configuration.json
  grant_types_supported:
  - authorization_code
  - client_credentials
  - implicit
  - password
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:uma-ticket
  - urn:openid:params:grant-type:ciba
  id_token_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - EdDSA
  - HS256
  - HS384
  - HS512
  introspectionUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token/introspect
  issuer: https://dv-ciam.doubleverify.com/realms/pinnacle
  jwksUri: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/certs
  name: dv-ciam-openid-connect
  openIdConnectUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/.well-known/openid-configuration
  registrationEndpoint: https://dv-ciam.doubleverify.com/realms/pinnacle/clients-registrations/openid-connect
  revocationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/revoke
  source: probed
  tokenUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
  userinfoUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/userinfo
- applies_to: DV Report Data API (https://data-reporting.doubleverify.com)
  evidence:
  - https://improvado.io/docs/doubleverify
  - https://help.alliplatform.com/data/Working-version/doubleverify
  - probe https://data-reporting.doubleverify.com/requests -> 401
  in: header
  name: dv-report-data-api-bearer
  parameter: Authorization
  scheme: bearer
  source: searched
  token_contact: dataapi@doubleverify.com
  token_issuance: 'Self-service inside DV Pinnacle: Analytics -> Data API -> Create Token, or select an existing token. The token value is used as a bearer token; integrator documentation notes the value is supplied WITHOUT the literal word "Bearer" in some connector UIs.'
  type: http
slug: doubleverify-authentication
source_filename: doubleverify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  Live probes of https://mcp.doubleverify.com/mcp (401 + WWW-Authenticate),\n  https://mcp.doubleverify.com/.well-known/oauth-protected-resource/mcp (200),\n  https://dv-ciam.doubleverify.com/realms/pinnacle/.well-known/openid-configuration (200),\n  and https://data-reporting.doubleverify.com/* (401)\ndocs: https://developer.doubleverify.com/docs/client-integrations/extensions/report-data-api\nnote: >-\n  DERIVED FROM NO OPENAPI. DoubleVerify publishes no OpenAPI, so this profile is not a\n  securitySchemes rollup — it is built from the OAuth/OIDC discovery documents the\n  provider actually serves plus the live 401 challenges on its two API hosts.\n\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  identity_provider: Keycloak (DV CIAM)\n  realm: https://dv-ciam.doubleverify.com/realms/pinnacle\n\
  \  account_gate: Every DoubleVerify API surface requires a DV Pinnacle account. There is\n    no self-service signup and no anonymous tier.\n\nschemes:\n- name: dv-neura-mcp-oauth\n  type: oauth2\n  applies_to: DV Neura MCP Server (https://mcp.doubleverify.com/mcp)\n  bearer_methods_supported:\n  - header\n  scopes_required:\n  - openid\n  - email\n  - profile\n  protected_resource_metadata: https://mcp.doubleverify.com/.well-known/oauth-protected-resource/mcp\n  authorization_server: https://dv-ciam.doubleverify.com/realms/pinnacle\n  source: probed\n  rfc:\n  - RFC 9728 (OAuth 2.0 Protected Resource Metadata)\n  - RFC 6750 (Bearer token usage)\n\n- name: dv-ciam-openid-connect\n  type: openIdConnect\n  applies_to: DV Pinnacle / DV Neura CIAM realm\n  openIdConnectUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/.well-known/openid-configuration\n  issuer: https://dv-ciam.doubleverify.com/realms/pinnacle\n  authorizationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth\n\
  \  tokenUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token\n  userinfoUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/userinfo\n  jwksUri: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/certs\n  introspectionUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/token/introspect\n  revocationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/revoke\n  deviceAuthorizationUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/auth/device\n  endSessionUrl: https://dv-ciam.doubleverify.com/realms/pinnacle/protocol/openid-connect/logout\n  registrationEndpoint: https://dv-ciam.doubleverify.com/realms/pinnacle/clients-registrations/openid-connect\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n\
  \  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\n  token_endpoint_auth_methods_supported:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  - RS384\n  - RS512\n  - PS256\n  - PS384\n  - PS512\n  - ES256\n  - ES384\n  - ES512\n  - EdDSA\n  - HS256\n  - HS384\n  - HS512\n  source: probed\n  file: well-known/doubleverify-openid-configuration.json\n\n- name: dv-report-data-api-bearer\n  type: http\n  scheme: bearer\n  applies_to: DV Report Data API (https://data-reporting.doubleverify.com)\n  in: header\n  parameter: Authorization\n  token_issuance: >-\n    Self-service inside DV Pinnacle: Analytics -> Data API -> Create Token, or select an\n    existing token. The token value is used as a bearer token; integrator documentation\n\
  \    notes the value is supplied WITHOUT the literal word \"Bearer\" in some connector UIs.\n  token_contact: dataapi@doubleverify.com\n  source: searched\n  evidence:\n  - https://improvado.io/docs/doubleverify\n  - https://help.alliplatform.com/data/Working-version/doubleverify\n  - probe https://data-reporting.doubleverify.com/requests -> 401\n\nobserved_challenges:\n- url: https://mcp.doubleverify.com/mcp\n  status: 401\n  www_authenticate: Bearer error=\"invalid_token\", error_description=\"The access token\n    is missing or invalid\", resource_metadata=\"https://mcp.doubleverify.com/.well-known/oauth-protected-resource/mcp\",\n    scope=\"openid email profile\"\n- url: https://data-reporting.doubleverify.com/requests\n  status: 401\n  www_authenticate: null\n  note: Bare 401 with no WWW-Authenticate header and a zero-length body — the Report Data\n    API does not advertise its auth scheme to an unauthenticated caller.\n- url: https://developer.doubleverify.com/docs\n  status: 200\n\
  \  note: Redirects to /docs/login?return_to=%2Fdocs — the developer documentation portal\n    itself is behind a login.\n\ngaps:\n- No securitySchemes can be verified against a machine-readable contract; DoubleVerify\n  publishes no OpenAPI.\n- The Report Data API returns no WWW-Authenticate header, so an agent cannot discover how\n  to authenticate from the wire.\n- Token lifetime, rotation and revocation policy for Report Data API tokens are documented\n  only inside the gated developer portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doubleverify/refs/heads/main/authentication/doubleverify-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Ad Verification
- Ad Measurement
- Media Quality
- Brand Suitability
- Viewability
- Attention Measurement
- Invalid Traffic
- Fraud Detection
- Contextual Targeting
- Programmatic Advertising
- Connected TV
- Social Media Measurement
- Commerce Media
- Publisher Analytics
- MRC Accredited
- AdTech
---
