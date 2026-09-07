---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Worksome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Worksome declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Worksome
provider_slug: worksome
scheme_count: 2
schemes:
- access_token_lifetime: 15 days
  authorization_url: https://use.worksome.com/oauth/authorize
  authorize_parameters:
  - name: client_id
    required: true
    type: string
  - name: response_type
    required: true
    type: string
    value: code
  - name: redirect_uri
    required: true
    type: string
  - description: Unguessable random string; CSRF protection. Docs instruct aborting if the returned state does not match.
    name: state
    required: false
    type: string
  - description: consent always shows the approval screen; login always forces re-authentication; omitted means prompt only if not previously authorized.
    enum:
    - consent
    - login
    name: prompt
    required: false
    type: string
  client_registration: Self-service via the Worksome API clients page. A client carries a name and a redirect (callback) URL; only the registered redirect URL is accepted at authorization time.
  code_lifetime: 10 minutes
  flow: authorizationCode
  id: oauth2_authorization_code
  pkce: not documented
  preferred: true
  refresh_grant_type: refresh_token
  refresh_supported: true
  refresh_window: 90 days
  revocation: A client can be revoked from the API clients page, which both blocks new token issuance and invalidates tokens already issued by that client.
  scopes_note: No scope parameter is documented on the authorize call and no scope reference page is published, so no scopes/ artifact is emitted. The docs do acknowledge scopes exist at the failure end — a listed cause of authorization failure is "The token does not have the required scopes" — which means an integrator can be denied by a scope they were never shown. This is a real documentation gap, not an absence of the mechanism.
  scopes_published: false
  token_parameters:
  - client_id
  - client_secret
  - code
  - grant_type
  - redirect_uri
  token_response_fields:
  - token_type
  - expires_in
  - access_token
  - refresh_token
  token_url: https://use.worksome.com/oauth/token
  type: oauth2
- bearer_format: opaque
  header: 'Authorization: Bearer {token}'
  id: personal_access_token
  intended_use: Testing and single-account integrations; also the CLI's only supported credential.
  issuance: Self-service from the Worksome API tokens page.
  lifetime: 6 months from creation, automatically revoked on expiry
  preferred: false
  revocation: Manual, from the API tokens page.
  scheme: bearer
  type: http
slug: worksome-authentication
source_filename: worksome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://docs.worksome.com/authentication/\ndocs: https://docs.worksome.com/authentication/\nnote: >-\n  Derived from the published Authentication page rather than from an OpenAPI securitySchemes\n  block — Worksome publishes no OpenAPI. The API is GraphQL-only and every authenticated\n  call carries a standard Authorization: Bearer header against the single endpoint\n  https://api.worksome.com/graphql. Two token sources exist: OAuth 2.0 authorization code\n  (the preferred path, for acting on behalf of other users) and Personal Access Tokens (for\n  testing and single-account integrations). Note that schema INTROSPECTION is open and\n  unauthenticated — an anonymous POST of the introspection query to the endpoint returns the\n  full 496-type schema — while every data-bearing query and mutation requires a token.\n\ntransport:\n  tls_required: true\n  endpoint: https://api.worksome.com/graphql\n  method: POST\n  content_type_required:\
  \ application/json\n  csrf_note: >-\n    The Apollo federation gateway enforces CSRF preflight. A POST without Content-Type:\n    application/json, or any GET without an apollo-require-preflight (or\n    x-apollo-operation-name) header, is rejected with extensions.code BAD_REQUEST before the\n    request reaches GraphQL.\n\nschemes:\n- id: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  preferred: true\n  authorization_url: https://use.worksome.com/oauth/authorize\n  token_url: https://use.worksome.com/oauth/token\n  refresh_supported: true\n  refresh_grant_type: refresh_token\n  pkce: not documented\n  client_registration: >-\n    Self-service via the Worksome API clients page. A client carries a name and a redirect\n    (callback) URL; only the registered redirect URL is accepted at authorization time.\n  authorize_parameters:\n  - name: client_id\n    required: true\n    type: string\n  - name: response_type\n    required: true\n    type: string\n    value: code\n\
  \  - name: redirect_uri\n    required: true\n    type: string\n  - name: state\n    required: false\n    type: string\n    description: Unguessable random string; CSRF protection. Docs instruct aborting if the returned state does not match.\n  - name: prompt\n    required: false\n    type: string\n    enum: [consent, login]\n    description: consent always shows the approval screen; login always forces re-authentication; omitted means prompt only if not previously authorized.\n  token_parameters: [client_id, client_secret, code, grant_type, redirect_uri]\n  token_response_fields: [token_type, expires_in, access_token, refresh_token]\n  code_lifetime: 10 minutes\n  access_token_lifetime: 15 days\n  refresh_window: 90 days\n  scopes_published: false\n  scopes_note: >-\n    No scope parameter is documented on the authorize call and no scope reference page is\n    published, so no scopes/ artifact is emitted. The docs do acknowledge scopes exist at the\n    failure end — a listed cause of\
  \ authorization failure is \"The token does not have the\n    required scopes\" — which means an integrator can be denied by a scope they were never\n    shown. This is a real documentation gap, not an absence of the mechanism.\n  revocation: >-\n    A client can be revoked from the API clients page, which both blocks new token issuance\n    and invalidates tokens already issued by that client.\n\n- id: personal_access_token\n  type: http\n  scheme: bearer\n  bearer_format: opaque\n  preferred: false\n  intended_use: Testing and single-account integrations; also the CLI's only supported credential.\n  issuance: Self-service from the Worksome API tokens page.\n  lifetime: 6 months from creation, automatically revoked on expiry\n  revocation: Manual, from the API tokens page.\n  header: 'Authorization: Bearer {token}'\n\nauthorization_model:\n  tenancy: >-\n    A token belongs to a user, and a user may have access to multiple accounts. The viewer\n    query returns the authenticated user;\
  \ the top-level accounts query returns the accounts\n    the token can act on. accounts returns an Account interface implemented by Company,\n    Organisation, Partner, StaffingAgency and Worker — most company-context operations\n    require a Company id. Cross-company access is denied, and the docs list \"wrong company\n    scope\" as a distinct authorization failure cause.\n  field_level: >-\n    Authorization is enforced per field, not only per operation. A field the token may not\n    read returns null inside data with a matching entry in the errors array, so a partial\n    success is the normal shape of an under-privileged query.\n  roles: >-\n    Role names are not published. The docs reference \"the required role (e.g., manager,\n    admin)\" as an example only.\n\nmulti_factor:\n  available: true\n  note: >-\n    The GraphQL schema exposes end-user MFA management — createSmsMultiFactor,\n    verifySmsMultiFactor, createTotpMultiFactor, verifyTotpMultiFactor, removeMultiFactor,\n\
  \    and multiFactor/multiFactors queries. This is MFA for platform users managed through the\n    API, not a second factor on API token authentication itself.\n  methods: [sms, totp]\n  source: graphql/worksome.graphql\n\nsso:\n  available: true\n  protocol: SAML\n  note: SSO/SAML is named as an included platform capability on the pricing page. No SAML metadata endpoint or configuration reference is published in the developer docs.\n  source: https://www.worksome.com/pricing\n\nwebhook_authentication:\n  direction: inbound-to-consumer\n  mechanism: HMAC-SHA256\n  header: Signature\n  secret: Shared secret agreed with Worksome out of band\n  verification: hash_hmac('sha256', raw_body, secret) compared in constant time against the Signature header\n  note: >-\n    The signature covers the RAW request body — the docs are explicit that the body must be\n    read and verified before it is parsed. The header carries a bare hex digest with no\n    timestamp and no version prefix, so there is\
  \ no replay window bound to the signature\n    itself; the docs instead put the burden on the consumer, requiring handlers to be\n    idempotent and to detect duplicates by entity id.\n  source: https://docs.worksome.com/webhooks/guides/handle-webhooks/\n\nfailure_modes:\n- condition: Missing or invalid bearer token\n  code: DOWNSTREAM_SERVICE_ERROR\n  http: 200\n  discriminator: 'extensions.guards == [\"api\"] AND message == \"Unauthenticated.\"'\n- condition: Valid token, operation not permitted\n  code: DOWNSTREAM_SERVICE_ERROR\n  http: 200\n  discriminator: No validation map, no guards; message \"You are not authorized to perform this action.\" with the operation in path.\n- condition: Expired or revoked token\n  code: DOWNSTREAM_SERVICE_ERROR\n  http: 200\n  remediation: Issue a new PAT (6-month lifetime) or refresh the OAuth token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worksome/refs/heads/main/authentication/worksome-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Freelancer Management System
- Contingent Workforce
- Human Resources
- Staffing
- Workforce Compliance
- Payments
- GraphQL
- Webhooks
- Denmark
---
