---
api_key_in: []
api_specs:
- filename: lily-ai-lilyapp-api-openapi.yml
  format: yaml
  label: LilyApp Middleware API
  slug: lilyapp-middleware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lily-ai/refs/heads/main/openapi/lily-ai-lilyapp-api-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Lily Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lily AI secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lily AI
provider_slug: lily-ai
scheme_count: 2
schemes:
- applied_to_operations: 0
  bearerFormat: JWT
  declared_in: openapi/lily-ai-lilyapp-api-openapi.yml
  name: JWT
  note: 'Declared in components.securitySchemes but never referenced by any operation and with no root-level `security` block. The contract therefore reads as fully anonymous while the deployment is not. Probed 2026-08-12: GET /config/brands and GET /subsidiary/list both return HTTP 401 with body {"message":"null Token","status":401,"correlationId":"<uuid>"}.'
  scheme: bearer
  type: http
- api_scope_uri: https://lilyexternalaad.onmicrosoft.com/authprod
  authorization_endpoint: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/b2c_1a_signin_emailmfa/oauth2/v2.0/authorize
  declared_in: null
  discovered_from: app.lily.ai production bundle + live OIDC discovery fetch (HTTP 200, 2026-08-12). Not declared anywhere in Lily AI's OpenAPI.
  end_session_endpoint: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/b2c_1a_signin_emailmfa/oauth2/v2.0/logout
  file: ../well-known/lily-ai-b2c-openid-configuration.json
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://lilyexternalaad.b2clogin.com/036aae23-93d0-4faa-8a62-0699626e2799/v2.0/
  jwks_uri: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/b2c_1a_signin_emailmfa/discovery/v2.0/keys
  mfa: Enforced — the only sign-in user flow the application uses is B2C_1A_SIGNIN_EMAILMFA (email + multi-factor).
  name: AzureADB2C
  openid_configuration: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/B2C_1A_SIGNIN_EMAILMFA/v2.0/.well-known/openid-configuration
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - code id_token
  - code token
  - code id_token token
  - id_token
  - id_token token
  - token
  - token id_token
  scopes_supported:
  - openid
  subject_types_supported:
  - pairwise
  tenant: lilyexternalaad.onmicrosoft.com
  token_endpoint: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/b2c_1a_signin_emailmfa/oauth2/v2.0/token
  type: openIdConnect
  user_flows:
  - B2C_1A_SIGNIN_EMAILMFA
  - B2C_1A_PASSWORDRESETEMAIL
slug: lily-ai-authentication
source_filename: lily-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  openapi/lily-ai-lilyapp-api-openapi.yml (components.securitySchemes), live 401\n  responses from https://lilyapp-api-prd.pub.lilyai.net (2026-08-12), the\n  app.lily.ai production JavaScript bundle, and the OIDC discovery document at\n  https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/B2C_1A_SIGNIN_EMAILMFA/v2.0/.well-known/openid-configuration\ndocs: null\nsummary:\n  types:\n  - http\n  - openIdConnect\n  model: >-\n    Bearer JWT issued by Lily AI's Azure AD B2C (Entra External ID) tenant. There is\n    no API key, no client-credentials path, and no self-service way to obtain a\n    credential — access is provisioned through Lily AI onboarding.\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  declared_in: openapi/lily-ai-lilyapp-api-openapi.yml\n  applied_to_operations: 0\n  note: >-\n    Declared in components.securitySchemes but never referenced by any operation and\n\
  \    with no root-level `security` block. The contract therefore reads as fully\n    anonymous while the deployment is not. Probed 2026-08-12: GET /config/brands and\n    GET /subsidiary/list both return HTTP 401 with body\n    {\"message\":\"null Token\",\"status\":401,\"correlationId\":\"<uuid>\"}.\n- name: AzureADB2C\n  type: openIdConnect\n  declared_in: null\n  discovered_from: >-\n    app.lily.ai production bundle + live OIDC discovery fetch (HTTP 200,\n    2026-08-12). Not declared anywhere in Lily AI's OpenAPI.\n  openid_configuration: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/B2C_1A_SIGNIN_EMAILMFA/v2.0/.well-known/openid-configuration\n  file: ../well-known/lily-ai-b2c-openid-configuration.json\n  issuer: https://lilyexternalaad.b2clogin.com/036aae23-93d0-4faa-8a62-0699626e2799/v2.0/\n  tenant: lilyexternalaad.onmicrosoft.com\n  authorization_endpoint: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/b2c_1a_signin_emailmfa/oauth2/v2.0/authorize\n\
  \  token_endpoint: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/b2c_1a_signin_emailmfa/oauth2/v2.0/token\n  jwks_uri: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/b2c_1a_signin_emailmfa/discovery/v2.0/keys\n  end_session_endpoint: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/b2c_1a_signin_emailmfa/oauth2/v2.0/logout\n  user_flows:\n  - B2C_1A_SIGNIN_EMAILMFA\n  - B2C_1A_PASSWORDRESETEMAIL\n  scopes_supported:\n  - openid\n  api_scope_uri: https://lilyexternalaad.onmicrosoft.com/authprod\n  response_types_supported: [code, code id_token, code token, code id_token token, id_token, id_token token, token, token id_token]\n  response_modes_supported: [query, fragment, form_post]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [pairwise]\n  mfa: >-\n    Enforced — the only sign-in user flow the application uses is\n    B2C_1A_SIGNIN_EMAILMFA (email + multi-factor).\nlogin_operations:\n- operationId:\
  \ AuthV2Controller_loginUserExt\n  path: /v2/auth/b2c/login\n  method: GET\n  note: Current-generation Azure AD B2C login for external (customer) users.\n- operationId: AuthV2Controller_loginUser\n  path: /v2/auth/microsoft/login\n  method: GET\n  note: Microsoft (internal Entra) login.\n- operationId: AuthV2Controller_loginQaSupport\n  path: /v2/auth/qa-automated/login\n  method: POST\n  note: >-\n    QA automation login (QaSupportLoginDto). This is the only operation in the whole\n    contract that declares 401 and 403 responses.\n- operationId: AuthController_loginUserExt\n  path: /auth/b2c/login\n  method: GET\n  note: Superseded v1 equivalent, still live and undeprecated.\n- operationId: AuthController_loginUser\n  path: /auth/microsoft/login\n  method: GET\n  note: Superseded v1 equivalent, still live and undeprecated.\nauthorization:\n  model: subsidiary (retailer tenant) scoping, carried on the request\n  note: >-\n    There is no OAuth scope surface for the API itself — the B2C\
  \ tenant advertises\n    only `openid`, and the API declares no oauth2 flows and no scopes. Entitlement\n    is expressed by the subsidiary identifier a caller passes, in four different\n    spellings (subsidiaryCode, subsidiaryID, subsidiary-id header, x-subsidiary-id\n    header). No scopes/ artifact is emitted, per the pipeline's OAuth-only rule.\ncredential_acquisition:\n  self_service: false\n  sign_up: null\n  note: >-\n    No developer sign-up, no key-issuance page, no documented onboarding. Lily AI\n    provisions application access through sales-led enterprise onboarding\n    (https://www.lily.ai/free-trial requests a pilot; it is not a credential path).\nx-evidence:\n- url: https://lilyapp-api-prd.pub.lilyai.net/config/brands\n  status: 401\n  fetched: '2026-08-12'\n- url: https://lilyexternalaad.b2clogin.com/lilyexternalaad.onmicrosoft.com/B2C_1A_SIGNIN_EMAILMFA/v2.0/.well-known/openid-configuration\n  status: 200\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lily-ai/refs/heads/main/authentication/lily-ai-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Company
- Retail
- E-Commerce
- Artificial Intelligence
- Product Data
- Advertising
- Agentic Commerce
- Search
- Marketing
---
