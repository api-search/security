---
api_key_in:
- header
api_specs:
- filename: goodlord-agent-api-openapi.yml
  format: yaml
  label: Goodlord Agent API
  slug: goodlord-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-agent-api-openapi.yml
- filename: goodlord-application-api-openapi.yml
  format: yaml
  label: Goodlord Application API
  slug: goodlord-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-application-api-openapi.yml
- filename: goodlord-authentication-api-openapi.yml
  format: yaml
  label: Goodlord Authentication API
  slug: goodlord-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-authentication-api-openapi.yml
- filename: goodlord-company-api-openapi.yml
  format: yaml
  label: Goodlord Company API
  slug: goodlord-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-company-api-openapi.yml
- filename: goodlord-file-api-openapi.yml
  format: yaml
  label: Goodlord File API
  slug: goodlord-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-file-api-openapi.yml
- filename: goodlord-insuranceclaim-api-openapi.yml
  format: yaml
  label: Goodlord Insurance Claim API
  slug: goodlord-insuranceclaim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-insuranceclaim-api-openapi.yml
- filename: goodlord-media-api-openapi.yml
  format: yaml
  label: Goodlord Media API
  slug: goodlord-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-media-api-openapi.yml
- filename: goodlord-payment-api-openapi.yml
  format: yaml
  label: Goodlord Payment API
  slug: goodlord-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-payment-api-openapi.yml
- filename: goodlord-rentschedule-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule API
  slug: goodlord-rentschedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedule-api-openapi.yml
- filename: goodlord-rentschedulerow-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row API
  slug: goodlord-rentschedulerow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerow-api-openapi.yml
- filename: goodlord-rentschedulerowpostdto-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row Post Dto API
  slug: goodlord-rentschedulerowpostdto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerowpostdto-api-openapi.yml
- filename: goodlord-rentschedulerowupdate-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row Update API
  slug: goodlord-rentschedulerowupdate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerowupdate-api-openapi.yml
- filename: goodlord-role-api-openapi.yml
  format: yaml
  label: Goodlord Role API
  slug: goodlord-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-role-api-openapi.yml
- filename: goodlord-rolegroup-api-openapi.yml
  format: yaml
  label: Goodlord Role Group API
  slug: goodlord-rolegroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rolegroup-api-openapi.yml
- filename: goodlord-subject-api-openapi.yml
  format: yaml
  label: Goodlord Subject API
  slug: goodlord-subject-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-subject-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Goodlord Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Goodlord secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Goodlord
provider_slug: goodlord
scheme_count: 2
schemes:
- api: Goodlord Referencing API
  description: 'This API uses OAuth2 to authenticate requests. You must use your client credentials to obtain a token.

    Read [Obtain a JWT Token](./operations/getAuthToken) for more information.'
  flows:
  - flow: clientCredentials
    scopes: 0
    scopes_observed:
    - free_plan
    - referencing_product
    tokenUrl: https://api.goodoverlord.com/auth/token
    tokenUrl_sandbox: https://api-sandbox.goodlord.co/auth/token
  name: OAuth2
  request_body: client_id, client_secret and grant_type "client_credentials", posted as JSON
  sources:
  - openapi/goodlord-referencing-api-openapi.json
  - openapi/goodlord-referencing-api-sandbox-openapi.json
  - https://portal.goodlord.co/portal/catalogue-products/referencing-product-1
  token_format: JWT
  token_lifetime_seconds: 3600
  token_type: Bearer
  type: oauth2
- api: Goodlord Insurance App API
  description: Value for the Authorization header parameter.
  in: header
  modelling_note: Semantically an HTTP bearer JWT, but declared as type apiKey. Generated clients lose the bearer semantics. No token endpoint, authorization server or discovery document is published for this API — how a caller obtains the JWT is not documented anywhere.
  name: JWT
  parameter: Authorization
  sources:
  - openapi/goodlord-insurance-app-api-openapi.json
  type: apiKey
slug: goodlord-authentication
source_filename: goodlord-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/goodlord-insurance-app-api-openapi.json, openapi/goodlord-referencing-api-openapi.json,\n  openapi/goodlord-referencing-api-sandbox-openapi.json\ndocs: https://portal.goodlord.co/portal/catalogue-products/referencing-product-1\nnote: >-\n  Derived from the security schemes declared across Goodlord's three published OpenAPI 3.1.0\n  documents, then upgraded from the Authentication walkthrough in the Goodlord Developer\n  Portal — which documents a mandatory request header (Company-ID) and a runtime scope string\n  that appear nowhere in the machine-readable contracts.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  self_serve_credentials: false\n  credential_issuance: >-\n    Issued by a Goodlord sales manager or account manager as part of a commercial engagement.\n    The developer portal's own registration page returns \"Registration is not allowed\"\
  \ and\n    requires an invite code. Sandbox first, production enabled afterwards.\nschemes:\n- name: OAuth2\n  type: oauth2\n  api: Goodlord Referencing API\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.goodoverlord.com/auth/token\n    tokenUrl_sandbox: https://api-sandbox.goodlord.co/auth/token\n    scopes: 0\n    scopes_observed: [free_plan, referencing_product]\n  request_body: client_id, client_secret and grant_type \"client_credentials\", posted as JSON\n  token_format: JWT\n  token_type: Bearer\n  token_lifetime_seconds: 3600\n  description: |-\n    This API uses OAuth2 to authenticate requests. You must use your client credentials to obtain a token.\n    Read [Obtain a JWT Token](./operations/getAuthToken) for more information.\n  sources:\n  - openapi/goodlord-referencing-api-openapi.json\n  - openapi/goodlord-referencing-api-sandbox-openapi.json\n  - https://portal.goodlord.co/portal/catalogue-products/referencing-product-1\n- name: JWT\n  type: apiKey\n  in:\
  \ header\n  parameter: Authorization\n  api: Goodlord Insurance App API\n  description: Value for the Authorization header parameter.\n  modelling_note: >-\n    Semantically an HTTP bearer JWT, but declared as type apiKey. Generated clients lose the\n    bearer semantics. No token endpoint, authorization server or discovery document is\n    published for this API — how a caller obtains the JWT is not documented anywhere.\n  sources:\n  - openapi/goodlord-insurance-app-api-openapi.json\nrequired_headers:\n- api: Goodlord Referencing API\n  headers:\n  - {name: Authorization, value: 'Bearer <access_token>', required: true, declared_in_spec: true}\n  - name: Company-ID\n    value: '<issued Company ID>'\n    required: true\n    declared_in_spec: false\n    note: >-\n      Mandatory tenant selector on EVERY request. Documented only in the portal Authentication\n      walkthrough; it appears in no OpenAPI parameter, header or securityScheme. This is the\n      single biggest gap between Goodlord's\
  \ contract and its runtime — a client generated\n      straight from the spec will fail.\n  - {name: Content-Type, value: application/json, required: true, declared_in_spec: true}\n- api: Goodlord Insurance App API\n  headers:\n  - {name: Authorization, value: '<JWT>', required: true, declared_in_spec: true}\n  - name: Accept\n    value: application/ld+json | application/vnd.api+json | application/json | text/csv\n    required: false\n    note: content negotiation is strict — the specification document itself only accepts application/vnd.openapi+json\nauthorization_model:\n- api: Goodlord Referencing API\n  model: product scope + tenant header\n  detail: >-\n    The granted scope selects the product (referencing_product) and plan (free_plan); the\n    Company-ID header selects the letting agency whose data is visible. No per-operation or\n    per-resource permissions are published.\n- api: Goodlord Insurance App API\n  model: role-based\n  detail: >-\n    An Agent carries roles[] and roleGroups[]\
  \ and is scoped to one or more companies[].\n    RoleGroups are flagged admin and/or agent. GET /api/v1/me returns the caller's own\n    identity, companies, roles and role groups. Every collection returns 403 when the resource\n    falls outside the caller's companies.\ndelegated_tokens:\n  api: Goodlord Referencing API\n  operations: [getBotToken, createBotToken]\n  paths:\n  - 'GET /referencing/subject/{subjectId}/auth/token'\n  - 'POST /referencing/subject/{subjectId}/auth/token'\n  note: >-\n    The Referencing API can mint a per-subject \"bot\" JWT scoped to a single subject —\n    a delegated token for driving a subject's own referencing journey. Goodlord publishes no\n    prose documentation for these two operations; their lifetime, audience and permitted\n    operations are undocumented.\nend_user_platform_identity:\n  scheme: OpenID Connect / OAuth 2.0 via Microsoft Entra External ID (Azure AD B2C) custom policy\n  audience: letting agents, landlords, tenants and guarantors —\
  \ NOT developers\n  tenant_id: 7ddbafdc-ee33-46fb-968a-3011e2a0a825\n  policy: B2C_1A_2_SIGNUPORSIGNIN\n  issuer: https://login.goodlord.co/7ddbafdc-ee33-46fb-968a-3011e2a0a825/v2.0/\n  discovery: well-known/goodlord-openid-configuration.json\n  scopes_supported: [openid]\n  id_token_signing_algs: [RS256]\n  subject_types: [pairwise]\n  custom_claims: [companies, userRoles, userTypes]\n  resource_scope_prefix: https://vouchauth.onmicrosoft.com/gl-api\n  note: >-\n    The \"vouchauth\" tenant name reflects Goodlord's Vouch referencing lineage — corroborated by\n    the Referencing API's own contact address, devs@vouch.co.uk, and by the \"vouch\" source name\n    in the webhook payload envelope.\ndiscovery:\n  oauth_authorization_server_metadata: false\n  openid_configuration_on_api_hosts: false\n  note: >-\n    Neither Referencing gateway serves RFC 8414 authorization-server metadata or an OIDC\n    discovery document. The only discovery document in the estate belongs to the end-user\n\
  \    platform login.\nrelated:\n  scopes: scopes/goodlord-scopes.yml\n  conventions: conventions/goodlord-conventions.yml\n  sandbox: sandbox/goodlord-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/authentication/goodlord-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Management
- Rentals
- Lettings
- Tenant Referencing
- Tenancy Management
- Insurance
- Payments
---
