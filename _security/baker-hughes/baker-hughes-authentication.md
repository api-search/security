---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Baker Hughes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Baker Hughes declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Baker Hughes
provider_slug: baker-hughes
scheme_count: 1
schemes:
- authorization_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/auth
  backchannel_authentication_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/ext/ciba/auth
  code_challenge_methods_supported:
  - plain
  - S256
  device_authorization_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/auth/device
  end_session_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/logout
  grant_types_supported:
  - authorization_code
  - client_credentials
  - implicit
  - password
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:uma-ticket
  - urn:openid:params:grant-type:ciba
  id_token_signing_alg_values_supported:
  - PS384
  - RS384
  - EdDSA
  - ES384
  - HS256
  - HS512
  - ES256
  - RS256
  - HS384
  - ES512
  - PS256
  - PS512
  - RS512
  introspection_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/token/introspect
  issuer: https://auth-developer.bakerhughes.com/auth/realms/dedicated
  jwks_uri: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/certs
  name: oidc
  observed_client:
    client_id: app-cdp
    code_challenge_method: S256
    evidence: Location header of GET https://developer.bakerhughes.com/api/auth/keycloak/start?env=development (302)
    redirect_uri: https://developer.bakerhughes.com/api/auth/keycloak/handler/frame
    scope: openid profile email
  openIdConnectUrl: https://auth-developer.bakerhughes.com/auth/realms/dedicated/.well-known/openid-configuration
  pushed_authorization_request_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/ext/par/request
  registration_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/clients-registrations/openid-connect
  require_pushed_authorization_requests: false
  response_types_supported:
  - code
  - none
  - id_token
  - token
  - id_token token
  - code id_token
  - code token
  - code id_token token
  revocation_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/revoke
  scopes_supported:
  - openid
  - tenant-scope
  - abac_scope
  - email
  - profile
  tls_client_certificate_bound_access_tokens: true
  token_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/token
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
  userinfo_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/userinfo
slug: baker-hughes-authentication
source_filename: baker-hughes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: https://auth-developer.bakerhughes.com/auth/realms/dedicated/.well-known/openid-configuration\nprovider: Baker Hughes\nproviderId: baker-hughes\nscope: Identity for the Baker Hughes Developer Portal (developer.bakerhughes.com, a Backstage instance) and the\n  Cordant platform tenants it fronts. No public API reference documents how a Cordant/BHC3 API call itself is authenticated;\n  everything below is read from the provider's own OIDC discovery document, not inferred.\nsummary: 'OpenID Connect / OAuth 2.0 via a Keycloak realm (''dedicated''). The developer portal''s sign-in (GET\n  /api/auth/keycloak/start?env=development on developer.bakerhughes.com) 302s to this realm''s authorization endpoint\n  with client_id=app-cdp, PKCE S256 and scope ''openid profile email''. Anonymous calls to the portal''s catalog\n  API (/api/catalog/entities) return 401 {\"AuthenticationError\": \"Missing credentials\"}; there is no self-serve\n\
  \  sign-up — the portal''s support contact is cordant_success@bakerhughes.com.'\nschemes:\n- name: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth-developer.bakerhughes.com/auth/realms/dedicated/.well-known/openid-configuration\n  issuer: https://auth-developer.bakerhughes.com/auth/realms/dedicated\n  authorization_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/auth\n  token_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/token\n  userinfo_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/userinfo\n  jwks_uri: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/certs\n  introspection_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/token/introspect\n  revocation_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/revoke\n\
  \  end_session_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/logout\n  device_authorization_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/auth/device\n  pushed_authorization_request_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/ext/par/request\n  backchannel_authentication_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/protocol/openid-connect/ext/ciba/auth\n  registration_endpoint: https://auth-developer.bakerhughes.com/auth/realms/dedicated/clients-registrations/openid-connect\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - implicit\n  - password\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:uma-ticket\n  - urn:openid:params:grant-type:ciba\n  response_types_supported:\n  -\
  \ code\n  - none\n  - id_token\n  - token\n  - id_token token\n  - code id_token\n  - code token\n  - code id_token token\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  token_endpoint_auth_methods_supported:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  tls_client_certificate_bound_access_tokens: true\n  require_pushed_authorization_requests: false\n  scopes_supported:\n  - openid\n  - tenant-scope\n  - abac_scope\n  - email\n  - profile\n  id_token_signing_alg_values_supported:\n  - PS384\n  - RS384\n  - EdDSA\n  - ES384\n  - HS256\n  - HS512\n  - ES256\n  - RS256\n  - HS384\n  - ES512\n  - PS256\n  - PS512\n  - RS512\n  observed_client:\n    client_id: app-cdp\n    redirect_uri: https://developer.bakerhughes.com/api/auth/keycloak/handler/frame\n    scope: openid profile email\n    code_challenge_method: S256\n    evidence: Location header of GET https://developer.bakerhughes.com/api/auth/keycloak/start?env=development\
  \ (302)\nportal_gate:\n  url: https://developer.bakerhughes.com/api/catalog/entities\n  status: 401\n  body: '{\"error\":{\"name\":\"AuthenticationError\",\"message\":\"Missing credentials\"}}'\n  probed: '2026-09-17'\ncredential_issuance: Not self-serve. No public sign-up or key-issuance page was found; the portal's only published\n  contact is cordant_success@bakerhughes.com and the Cordant site routes to CordantTechSupport@BakerHughes.com.\nnotes:\n- The realm advertises a registration_endpoint (Keycloak clients-registrations/openid-connect); anonymous GET returns\n  404 and no initial-access-token policy is published, so open dynamic client registration is NOT asserted.\n- The realm-level public_key and JWKS (RS256 sig + RSA-OAEP enc keys) are served anonymously at the jwks_uri.\n- Cordant marketing copy says the platform 'offers APIs for integration' (OT/IT connectivity) but publishes no auth\n  scheme for them; treat API-call authentication as undocumented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baker-hughes/refs/heads/main/authentication/baker-hughes-authentication.yml
summary_line: 1 scheme
tags:
- Energy Technology
- Industrial IoT
- Oil and Gas
- Asset Performance Management
- Digital Energy
- Fortune 500
---
