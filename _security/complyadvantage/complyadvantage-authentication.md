---
api_key_in:
- header
api_specs:
- filename: complyadvantage-mesh-api-openapi.json
  format: json
  label: ComplyAdvantage Mesh Platform API
  slug: complyadvantage-mesh-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-mesh-api-openapi.json
- filename: complyadvantage-case-management-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Case Management API
  slug: complyadvantage-case-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-case-management-api-openapi.yml
- filename: complyadvantage-monitored-searches-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Monitored Searches API
  slug: complyadvantage-monitored-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-monitored-searches-api-openapi.yml
- filename: complyadvantage-searches-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Searches API
  slug: complyadvantage-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-searches-api-openapi.yml
- filename: complyadvantage-users-api-openapi.yml
  format: yaml
  label: ComplyAdvantage Users API
  slug: complyadvantage-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-users-api-openapi.yml
auth_types:
- oauth2-client-credentials
- http-bearer
- apiKey
description: 'Two APIs, two unrelated authentication models. The Mesh platform uses an OAuth2 client-credentials exchange - an access key and secret minted in the UI are traded at POST /v3/token for a bearer token that lives 24 hours and cannot be refreshed. The legacy REST API uses a static account API key sent as `Authorization: Token <key>`. Neither model is fully expressed in a machine-readable contract: the Mesh OpenAPI declares only an opaque `http bearer` scheme with no OAuth flow object and no scopes, and there is no published spec for the legacy API at all.'
kind: authentication
layout: security
method: searched
name: Complyadvantage Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComplyAdvantage secures its APIs with oauth2-client-credentials, http-bearer, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ComplyAdvantage
provider_slug: complyadvantage
scheme_count: 3
schemes:
- api: ComplyAdvantage Mesh Platform API
  credential_shape: access key + secret, with configurable lifespan, permissions and optional expiry date
  credential_source: 'Mesh UI: Settings > Access Management > API Credentials'
  description: 'The token issued by the client-credentials exchange. Declared globally - security is [{BearerAuth: []}] and no operation overrides it, so every one of the 163 Mesh operations requires it.'
  format: 'Authorization: Bearer {access_token}'
  in: header
  name: BearerAuth
  parameter: Authorization
  revocation: When client credentials expire or are revoked by the user they can no longer generate access tokens. Already-issued tokens are not documented as being revoked.
  scheme: bearer
  sources:
  - openapi/complyadvantage-mesh-api-openapi.json
  - https://docs.mesh.complyadvantage.com/reference/createtokenv3
  token_endpoint: POST /v3/token
  token_operation_id: createTokenV3
  token_refresh: none - there is no refresh grant; mint a new token the same way
  token_ttl_seconds: 86400
  type: http
- api: ComplyAdvantage Mesh Platform API
  deprecated: true
  description: POST /v2/token (createToken) exchanges username + password + realm for the same 24-hour bearer token. Deprecated - "If you are setting up a new API integration, use API credentials and the /v3/token endpoint instead of this one." `realm` is the organization name supplied by ComplyAdvantage at onboarding and is case-sensitive. The provider recommends a dedicated API-user email address, one per account.
  name: LegacyTokenExchange
  replacement: POST /v3/token
  sources:
  - https://docs.mesh.complyadvantage.com/reference/createtoken
  - https://docs.mesh.complyadvantage.com/docs/getting-started
  sunset: not published
  type: oauth2-password
- api: ComplyAdvantage legacy REST API
  description: Static per-account API key generated inside the ComplyAdvantage web platform; an account is required, so there is no anonymous or self-serve key issuance. No rotation policy, expiry, or scoping is published. Applies to all three regional bases - api.complyadvantage.com (EU), api.us.complyadvantage.com (US), api.ap.complyadvantage.com (APAC).
  format: 'Authorization: Token YOUR_API_KEY'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/complyadvantage-case-management-api-openapi.yml
  - openapi/complyadvantage-monitored-searches-api-openapi.yml
  - openapi/complyadvantage-searches-api-openapi.yml
  - openapi/complyadvantage-users-api-openapi.yml
  - https://docs.complyadvantage.com/api-docs
  type: apiKey
slug: complyadvantage-authentication
source_filename: complyadvantage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://docs.mesh.complyadvantage.com/reference/createtokenv3,\n  https://docs.mesh.complyadvantage.com/reference/createtoken,\n  https://docs.mesh.complyadvantage.com/docs/getting-started,\n  https://docs.complyadvantage.com/api-docs; derived from\n  openapi/complyadvantage-mesh-api-openapi.json and the four refined legacy specs in openapi/\ndocs: https://docs.mesh.complyadvantage.com/reference/createtokenv3\nprovider: ComplyAdvantage\nproviderId: complyadvantage\ndescription: >-\n  Two APIs, two unrelated authentication models. The Mesh platform uses an OAuth2\n  client-credentials exchange - an access key and secret minted in the UI are traded at\n  POST /v3/token for a bearer token that lives 24 hours and cannot be refreshed. The legacy\n  REST API uses a static account API key sent as `Authorization: Token <key>`. Neither model\n  is fully expressed in a machine-readable contract: the Mesh OpenAPI declares only an\n\
  \  opaque `http bearer` scheme with no OAuth flow object and no scopes, and there is no\n  published spec for the legacy API at all.\nsummary:\n  types:\n  - oauth2-client-credentials\n  - http-bearer\n  - apiKey\n  api_key_in:\n  - header\n  mtls: false\n  oidc: false\n  discovery_document: none published\nschemes:\n- name: BearerAuth\n  api: ComplyAdvantage Mesh Platform API\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer {access_token}'\n  description: >-\n    The token issued by the client-credentials exchange. Declared globally -\n    security is [{BearerAuth: []}] and no operation overrides it, so every one of the 163\n    Mesh operations requires it.\n  token_endpoint: POST /v3/token\n  token_operation_id: createTokenV3\n  credential_source: 'Mesh UI: Settings > Access Management > API Credentials'\n  credential_shape: access key + secret, with configurable lifespan, permissions and optional expiry date\n  token_ttl_seconds:\
  \ 86400\n  token_refresh: none - there is no refresh grant; mint a new token the same way\n  revocation: >-\n    When client credentials expire or are revoked by the user they can no longer generate\n    access tokens. Already-issued tokens are not documented as being revoked.\n  sources:\n  - openapi/complyadvantage-mesh-api-openapi.json\n  - https://docs.mesh.complyadvantage.com/reference/createtokenv3\n- name: LegacyTokenExchange\n  api: ComplyAdvantage Mesh Platform API\n  type: oauth2-password\n  deprecated: true\n  description: >-\n    POST /v2/token (createToken) exchanges username + password + realm for the same 24-hour\n    bearer token. Deprecated - \"If you are setting up a new API integration, use API\n    credentials and the /v3/token endpoint instead of this one.\" `realm` is the organization\n    name supplied by ComplyAdvantage at onboarding and is case-sensitive. The provider\n    recommends a dedicated API-user email address, one per account.\n  replacement: POST /v3/token\n\
  \  sunset: not published\n  sources:\n  - https://docs.mesh.complyadvantage.com/reference/createtoken\n  - https://docs.mesh.complyadvantage.com/docs/getting-started\n- name: apiKeyAuth\n  api: ComplyAdvantage legacy REST API\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Token YOUR_API_KEY'\n  description: >-\n    Static per-account API key generated inside the ComplyAdvantage web platform; an account\n    is required, so there is no anonymous or self-serve key issuance. No rotation policy,\n    expiry, or scoping is published. Applies to all three regional bases -\n    api.complyadvantage.com (EU), api.us.complyadvantage.com (US),\n    api.ap.complyadvantage.com (APAC).\n  sources:\n  - openapi/complyadvantage-case-management-api-openapi.yml\n  - openapi/complyadvantage-monitored-searches-api-openapi.yml\n  - openapi/complyadvantage-searches-api-openapi.yml\n  - openapi/complyadvantage-users-api-openapi.yml\n  - https://docs.complyadvantage.com/api-docs\n\
  authorization:\n  model: named account permissions plus account-level entitlements\n  note: >-\n    Not OAuth scopes. A 401 means the token is bad; a 403 means the credential's role lacks\n    the permission the endpoint names, or the account lacks the product entitlement.\n  artifact: scopes/complyadvantage-scopes.yml\nend_user_auth:\n  provider: AWS Cognito\n  evidence: >-\n    app.complyadvantage.com redirects to\n    auth.complyadvantage.com/login?client_id=...&response_type=code&scope=aws.cognito.signin.user.admin\n    openid email profile - an authorization-code flow on a Cognito hosted UI.\n  note: >-\n    This is the human web-app login, not an API surface. No OIDC discovery document is\n    published on auth.complyadvantage.com (/.well-known/openid-configuration returns 404),\n    so third parties cannot federate against it.\ntransport:\n  https_required: true\n  note: >-\n    \"All API requests must be made over HTTPS; calls made over plain HTTP will fail.\" Both\n    API hosts\
  \ answer 401 for every unauthenticated path, including /.well-known/*, so the\n    gateway authenticates before it routes.\ngaps:\n- The Mesh OpenAPI declares no oauth2 securityScheme, so the client-credentials flow and the token endpoint are invisible to code generators.\n- No scopes are published; least privilege has to be assembled by reading the prose permission line on each of 163 endpoints.\n- No OIDC discovery, no JWKS endpoint, no mTLS, no DPoP.\n- No documented key/credential rotation policy for the legacy API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/authentication/complyadvantage-authentication.yml
summary_line: oauth2-client-credentials/http-bearer/apiKey · 3 schemes
tags:
- Anti-Money Laundering
- AML
- Fraud Detection
- Sanctions Screening
- Compliance
- PEP Screening
- Adverse Media
- KYC
- Watchlist
- Transaction Monitoring
- Financial Crime
- RegTech
---
