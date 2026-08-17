---
api_key_in: []
api_specs:
- filename: flexpa-access-tokens-api-openapi.yml
  format: yaml
  label: Flexpa Access Tokens API
  slug: flexpa-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-access-tokens-api-openapi.yml
- filename: flexpa-claims-data-api-openapi.yml
  format: yaml
  label: Flexpa Claims Data API
  slug: flexpa-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-claims-data-api-openapi.yml
- filename: flexpa-fhir-api-openapi.yml
  format: yaml
  label: Flexpa FHIR API
  slug: flexpa-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-fhir-api-openapi.yml
- filename: flexpa-link-api-openapi.yml
  format: yaml
  label: Flexpa Link API
  slug: flexpa-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-link-api-openapi.yml
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Flexpa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flexpa secures its APIs with oauth2, http, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Flexpa
provider_slug: flexpa
scheme_count: 3
schemes:
- applies_to:
  - https://api.flexpa.com/fhir
  - https://api.flexpa.com/mcp
  bearerFormat: JWT
  description: 'A Patient Access Token (authorization_code + PKCE, obtained through Flexpa Consent) or an Application Access Token (client_credentials), sent as Authorization: Bearer {access_token}. Application Access Tokens are JWTs signed with ES256 and live 30 minutes.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flexpa-access-tokens-api-openapi.yml
  - openapi/flexpa-claims-data-api-openapi.yml
  - openapi/flexpa-fhir-api-openapi.yml
  - openapi/flexpa-link-api-openapi.yml
  - https://www.flexpa.com/docs/records
  type: http
- description: SMART on FHIR / OAuth 2.0 with PKCE, read from live discovery metadata.
  discovery:
  - https://api.flexpa.com/.well-known/openid-configuration
  - https://api.flexpa.com/.well-known/oauth-authorization-server
  - https://api.flexpa.com/.well-known/smart-configuration
  - https://api.flexpa.com/.well-known/oauth-protected-resource
  flows:
  - authorizationUrl: https://api.flexpa.com/oauth/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    refreshUrl: https://api.flexpa.com/oauth/token
    scopes:
      launch/patient: Standalone patient launch context.
      offline_access: Issue a refresh token.
    tokenUrl: https://api.flexpa.com/oauth/token
  - client_auth: client_secret_basic (publishable key as username, secret key as password)
    flow: clientCredentials
    tokenUrl: https://api.flexpa.com/oauth/token
  jwks_uri: https://api.flexpa.com/.well-known/jwks.json
  name: oauth2
  registration_endpoint: https://api.flexpa.com/oauth/register
  see: scopes/flexpa-scopes.yml
  type: oauth2
- description: Publishable and secret API keys identify the application. The publishable key is the OAuth client_id used on authorization URLs; the secret key is used only server-side, for client_credentials and HTTP Basic authentication.
  in: credentials
  key_prefixes:
  - pk_test_
  - pk_live_
  - sk_test_
  - sk_live_
  modes:
  - test
  - live
  name: apiKeys
  type: apiKey
slug: flexpa-authentication
source_filename: flexpa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://www.flexpa.com/docs/consent + https://www.flexpa.com/docs/records + https://api.flexpa.com/.well-known/openid-configuration\nderived_from: openapi/_original/flexpa-openapi.yml\ndocs: https://www.flexpa.com/docs/consent\nprovider: Flexpa\nproviderId: flexpa\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  primary: OAuth 2.0 authorization code with PKCE (patient) and client_credentials (application)\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    A Patient Access Token (authorization_code + PKCE, obtained through Flexpa\n    Consent) or an Application Access Token (client_credentials), sent as\n    Authorization: Bearer {access_token}. Application Access Tokens are JWTs\n    signed with ES256 and live 30 minutes.\n  applies_to:\n  - https://api.flexpa.com/fhir\n  - https://api.flexpa.com/mcp\n  sources:\n  - openapi/flexpa-access-tokens-api-openapi.yml\n\
  \  - openapi/flexpa-claims-data-api-openapi.yml\n  - openapi/flexpa-fhir-api-openapi.yml\n  - openapi/flexpa-link-api-openapi.yml\n  - https://www.flexpa.com/docs/records\n- name: oauth2\n  type: oauth2\n  description: SMART on FHIR / OAuth 2.0 with PKCE, read from live discovery metadata.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.flexpa.com/oauth/authorize\n    tokenUrl: https://api.flexpa.com/oauth/token\n    refreshUrl: https://api.flexpa.com/oauth/token\n    pkce_methods:\n    - S256\n    scopes:\n      launch/patient: Standalone patient launch context.\n      offline_access: Issue a refresh token.\n  - flow: clientCredentials\n    tokenUrl: https://api.flexpa.com/oauth/token\n    client_auth: client_secret_basic (publishable key as username, secret key as password)\n  discovery:\n  - https://api.flexpa.com/.well-known/openid-configuration\n  - https://api.flexpa.com/.well-known/oauth-authorization-server\n  - https://api.flexpa.com/.well-known/smart-configuration\n\
  \  - https://api.flexpa.com/.well-known/oauth-protected-resource\n  registration_endpoint: https://api.flexpa.com/oauth/register\n  jwks_uri: https://api.flexpa.com/.well-known/jwks.json\n  see: scopes/flexpa-scopes.yml\n- name: apiKeys\n  type: apiKey\n  in: credentials\n  description: >-\n    Publishable and secret API keys identify the application. The publishable key\n    is the OAuth client_id used on authorization URLs; the secret key is used only\n    server-side, for client_credentials and HTTP Basic authentication.\n  key_prefixes:\n  - pk_test_\n  - pk_live_\n  - sk_test_\n  - sk_live_\n  modes:\n  - test\n  - live\nauthorization_url_parameters:\n- client_id (publishable key)\n- redirect_uri (must be pre-registered)\n- response_type=code\n- code_challenge + code_challenge_method=S256\n- scope (must include launch/patient)\n- flexpa_external_id (required)\n- flexpa_search_mode / flexpa_ial2_mode\n- flexpa_resume (recovery flows)\nmobile:\n  ios: ASWebAuthenticationSession (no\
  \ Flexpa SDK required)\n  android: Chrome Custom Tabs; optional AppAuth-Android\n  react_native: expo-auth-session + expo-web-browser, or react-native-app-auth\nmcp_authorization:\n  endpoint: https://api.flexpa.com/mcp\n  challenge: 'WWW-Authenticate: Bearer resource_metadata=\"https://api.flexpa.com/.well-known/oauth-protected-resource/mcp\"'\n  observed_status: 401\n  observed: '2026-08-14'\n  note: The public directory MCP server at /mcp/directory requires no authentication.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/authentication/flexpa-authentication.yml
summary_line: oauth2/http/apiKey · 3 schemes
tags:
- Healthcare
- FHIR
- Patient Access
- Claims Data
- Health Insurance
---
