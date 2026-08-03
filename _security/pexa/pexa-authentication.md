---
api_key_in: []
api_specs:
- filename: pexa-exchange-api-swagger.json
  format: json
  label: PEXA Exchange API
  slug: pexa-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-exchange-api-swagger.json
- filename: pexa-standalone-discharge-experience-api-openapi.yaml
  format: yaml
  label: PEXA Standalone Discharge Experience API
  slug: pexa-standalone-discharge-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-standalone-discharge-experience-api-openapi.yaml
- filename: pexa-plus-marketplace-b2b-api-openapi.yaml
  format: yaml
  label: PEXA Plus Marketplace B2B API
  slug: pexa-plus-marketplace-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-plus-marketplace-b2b-api-openapi.yaml
- filename: pexa-notification-service-openapi.yaml
  format: yaml
  label: PEXA Notification Service [$]
  slug: pexa-notification-service-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-notification-service-openapi.yaml
- filename: pexa-projects-api-v4-openapi.yaml
  format: yaml
  label: PEXA Projects API
  slug: pexa-projects-api-v4-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-projects-api-v4-openapi.yaml
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Pexa Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: PEXA secures its APIs with oauth2 and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: PEXA
provider_slug: pexa
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://auth.pexa.com.au/oauth/token
  name: oauth2
  sources:
  - openapi/pexa-notification-service-openapi.yaml
  type: oauth2
- flows:
  - authorizationUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token
  name: oauth2
  sources:
  - openapi/pexa-projects-api-v4-openapi.yaml
  spec_defect: The Projects v4 document ships an internal Keycloak URL (host.kubernetes.internal) as its authorization and token endpoint. The real endpoints are https://auth.pexa.com.au/oauth/token (production) and https://auth-tst.pexalabs.com.au/oauth/token (test).
  type: oauth2
- flows:
  - authorizationUrl: https://'{{auth2_env}}'/authorize
    flow: authorizationCode
    tokenUrl: https://'{{auth2_env}}'/oauth/token
  - flow: clientCredentials
    tokenUrl: https://'{{auth2_env}}'/oauth/token
  name: oauth2
  sources:
  - openapi/pexa-standalone-discharge-experience-api-openapi.yaml
  spec_defect: The Standalone Discharge document ships unresolved templates ({{auth2_env}}, {{api_scope}}) rather than real endpoint URLs and scope names.
  type: oauth2
slug: pexa-authentication
source_filename: pexa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource:\n- https://developer.pexa.com.au/Exchange/docs/documentation/ (Authentication, Authentication Compliance)\n- https://developer.pexa.com.au/Projects/docs/documentation/\n- https://developer.pexa.com.au/Webhooks/docs/definitions/webhooks/\n- https://www.pexa.com.au/pexa-apis/\n- https://auth.pexa.com.au/.well-known/openid-configuration\n- openapi/pexa-notification-service-openapi.yaml\n- openapi/pexa-projects-api-v4-openapi.yaml\n- openapi/pexa-standalone-discharge-experience-api-openapi.yaml\ndocs: https://developer.pexa.com.au/Exchange/docs/documentation/\nsummary:\n  types:\n  - oauth2\n  - mutualTLS\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  api_key_in: []\n  statement: >-\n    \"We authenticate our APIs using industry best practices, either through OAuth2.0 or Mutual TLS.\"\n    - https://www.pexa.com.au/pexa-apis/\n  token_lifetime: 12 hours\n  transport: PEXA only accepts TLS v1.2 protocol (or above)\n\
  \  header: 'Authorization: Bearer <access_token>'\naccess_gate:\n  self_serve: false\n  requirement: signed PEXA API Agreement\n  process:\n  - Register at https://www.pexa.com.au/pexa-apis/ - PEXA validates the details\n  - Once validated and approved, PEXA emails the test access details\n  - Plan and design, build and test, production readiness, go live\n  - Credential requests and re-issues via apisupport@pexa.com.au\n  authorization_code_extra: PEXA also requires your redirect_uri before issuing authorization-code credentials\n  portal_signup: disabled in the developer portal build (hideSignUp true; AWS Cognito identity)\nauthorization_servers:\n- environment: production\n  issuer: https://auth.pexa.com.au/\n  authorization_endpoint: https://auth.pexa.com.au/authorize\n  token_endpoint: https://auth.pexa.com.au/oauth/token\n  revocation_endpoint: https://auth.pexa.com.au/oauth/revoke\n  jwks_uri: https://auth.pexa.com.au/.well-known/jwks.json\n  discovery: https://auth.pexa.com.au/.well-known/openid-configuration\n\
  \  discovery_status: 200\n  shape: Auth0\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  code_challenge_methods_supported: [S256, plain]\n  document: well-known/pexa-openid-configuration.json\n- environment: test\n  issuer: https://auth-tst.pexalabs.com.au/\n  authorization_endpoint: https://auth-tst.pexalabs.com.au/authorize\n  token_endpoint: https://auth-tst.pexalabs.com.au/oauth/token\n  discovery: https://auth-tst.pexalabs.com.au/.well-known/openid-configuration\n  discovery_status: 200\n  document: well-known/pexa-openid-configuration-test.json\nflows:\n- flow: clientCredentials\n  audience: machine-to-machine integrations\n  parameters: [grant_type=client_credentials, client_id, client_secret, scope]\n  note: >-\n    Scope is required on the token request and is declared per endpoint in the developer portal.\n    The documented example scope is au_pub_tst_pexa_conversation_api_v2_read.\n- flow: authorizationCode\n  audience:\
  \ business-to-consumer - an individual user authenticating with their own PEXA credentials\n  parameters: [client_id, response_type=code, redirect_uri, scope, 'then grant_type=authorization_code + code + client_secret']\n  note: >-\n    Prompts the user to log into PEXA with their individual login, password and multi-factor\n    authentication at the start of every session.\n- flow: mutualTLS\n  audience: alternative to OAuth 2.0 for API authentication\n  note: >-\n    Offered as an alternative on the API integration page, with certificate error guidance in the\n    Exchange documentation. Not declared as a securityScheme in any shipped contract.\n- flow: private_key_jwt (outbound)\n  audience: webhook delivery in HMAC_OAUTH mode\n  note: >-\n    In HMAC_OAUTH mode PEXA authenticates ITSELF to the customer's token endpoint, signing the client\n    assertion with an AWS KMS RSA key using PS256. Claims: iss/sub = clientId, aud = authUrl,\n    exp = now + 10 minutes, iat, jti (random UUID).\
  \ client_secret is the alternative. Optional mTLS\n    applies to both the token request and the delivery.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pexa.com.au/oauth/token\n    scopes: 5\n  sources:\n  - openapi/pexa-notification-service-openapi.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/auth\n    tokenUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token\n    scopes: 3\n  - flow: clientCredentials\n    tokenUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token\n    scopes: 3\n  sources:\n  - openapi/pexa-projects-api-v4-openapi.yaml\n  spec_defect: >-\n    The Projects v4 document ships an internal Keycloak URL (host.kubernetes.internal) as its\n    authorization and token endpoint. The real endpoints are https://auth.pexa.com.au/oauth/token\n\
  \    (production) and https://auth-tst.pexalabs.com.au/oauth/token (test).\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: \"https://'{{auth2_env}}'/authorize\"\n    tokenUrl: \"https://'{{auth2_env}}'/oauth/token\"\n  - flow: clientCredentials\n    tokenUrl: \"https://'{{auth2_env}}'/oauth/token\"\n  sources:\n  - openapi/pexa-standalone-discharge-experience-api-openapi.yaml\n  spec_defect: >-\n    The Standalone Discharge document ships unresolved templates ({{auth2_env}}, {{api_scope}})\n    rather than real endpoint URLs and scope names.\ncompliance_requirements:\n- PEXA only accepts TLS v1.2 protocol\n- The OAuth 2.0 flow implementation must be secure\n- Client id and client secret must be securely stored and encrypted, and must not be accessible to\n  software users or other parties\n- The token request process must be executed securely and must not be interceptable\n- The access token must be stored securely and encrypted\nnotes:\n-\
  \ No API-key authentication exists anywhere in the estate.\n- No anonymous or public endpoint exists - even /health requires a token.\n- >-\n  The production OIDC discovery document advertises many Auth0 grant types (password, implicit,\n  device_code, token-exchange, jwt-bearer). Only client_credentials and authorization_code are\n  documented for PEXA API integrators; the rest are tenant defaults, not offered contracts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/authentication/pexa-authentication.yml
summary_line: oauth2/mutualTLS · 3 schemes
tags:
- Real Estate
- Australia
- Conveyancing
- Property Settlement
- Land Registry
- Title
- PropTech
- Mortgage
- Digital Signing
- Webhooks
---
