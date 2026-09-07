---
anonymous_access: false
api_key_in: []
api_specs:
- filename: autopay-accounting-api-openapi.yml
  format: yaml
  label: Autopay Accounting API
  slug: autopay-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-accounting-api-openapi.yml
- filename: autopay-booking-api-openapi.yml
  format: yaml
  label: Autopay Booking API
  slug: autopay-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-booking-api-openapi.yml
- filename: autopay-customer-club-api-openapi.yml
  format: yaml
  label: Autopay Customer Club API
  slug: autopay-customer-club-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-customer-club-api-openapi.yml
- filename: autopay-fleet-api-openapi.yml
  format: yaml
  label: Autopay Fleet API
  slug: autopay-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-fleet-api-openapi.yml
- filename: autopay-parking-api-openapi.yml
  format: yaml
  label: Autopay Parking API
  slug: autopay-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-parking-api-openapi.yml
- filename: autopay-payment-api-openapi.yml
  format: yaml
  label: Autopay Payment API
  slug: autopay-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-payment-api-openapi.yml
- filename: autopay-permit-api-openapi.yml
  format: yaml
  label: Autopay Permit API
  slug: autopay-permit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-permit-api-openapi.yml
- filename: autopay-statistics-api-openapi.yml
  format: yaml
  label: Autopay Statistics API
  slug: autopay-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-statistics-api-openapi.yml
- filename: autopay-status-api-openapi.yml
  format: yaml
  label: Autopay Status API
  slug: autopay-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-status-api-openapi.yml
- filename: autopay-vehicle-api-openapi.yml
  format: yaml
  label: Autopay Vehicle API
  slug: autopay-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/openapi/autopay-vehicle-api-openapi.yml
auth_types:
- oauth2
description: 'Every Autopay API is secured with a single mechanism: OAuth 2.0 client credentials against an Auth0-hosted authorization server, presented as a Bearer token. Credentials are issued by a human at Autopay and are bound to ONE operator — a partner integrating across several operators holds one client_id/client_secret pair per operator and must send the right pair per call.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Autopay Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Autopay secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Autopay
provider_slug: autopay
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials against api-auth.autopay.io with audience https://api.autopay.io. Some endpoints additionally require a named scope on the token — permit_booking (Booking API), customer_club (Customer Club API), zone_status (Status API).
  errors:
  - body: '{"error": "access_denied", "error_description": "Unauthorized"}'
    cause: Invalid client_id or client_secret.
    status: 401
  - body: '{"error_id":"authentication_error","message":"No access token present in header!"}'
    cause: Request to api.autopay.io with no Authorization header. Observed live 2026-09-06.
    status: 401
  flows:
  - audience: https://api.autopay.io
    flow: clientCredentials
    scopes: 3
    scopes_known:
    - customer_club
    - permit_booking
    - zone_status
    tokenUrl: https://api-auth.autopay.io/oauth/token
  name: OAuth2
  request:
    body_parameters:
    - name: client_id
      required: true
      type: string
    - name: client_secret
      required: true
      type: string
    - fixed_value: https://api.autopay.io
      name: audience
      required: true
      type: string
    - fixed_value: client_credentials
      name: grant_type
      required: true
      type: string
    content_type: application/json
    method: POST
    note: The token request body is JSON, not the application/x-www-form-urlencoded form RFC 6749 specifies. A generic OAuth client library configured for form encoding will fail against this endpoint.
  response:
    fields:
    - name: access_token
      type: string
    - description: The Autopay APIs reachable with this token.
      name: scope
      type: string
    - description: Seconds until expiry; 86400 in the documented example.
      name: expires_in
      type: integer
    - fixed_value: Bearer
      name: token_type
      type: string
  sources:
  - https://developer.autopay.io/authentication/
  - https://api-auth.autopay.io/.well-known/openid-configuration
  - openapi/autopay-openapi.yml
  token_caching_note: '"Generating excessive access tokens within the expiration time (i.e. requesting a new one for each request) may lead to termination of API access." Autopay enforces this contractually, not with a 429 — the penalty is loss of access. Any agent calling this API MUST cache the token for its full expires_in.'
  token_caching_required: true
  token_lifetime: 'Short-lived: "usually 10-24 hours". Read the real value from expires_in.'
  transport: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: autopay-authentication
source_filename: autopay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://developer.autopay.io/authentication/\ndocs: https://developer.autopay.io/authentication/\ndiscovery: https://api-auth.autopay.io/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  self_serve: false\n  mfa_on_api: n/a\ndescription: >-\n  Every Autopay API is secured with a single mechanism: OAuth 2.0 client credentials against an\n  Auth0-hosted authorization server, presented as a Bearer token. Credentials are issued by a\n  human at Autopay and are bound to ONE operator — a partner integrating across several\n  operators holds one client_id/client_secret pair per operator and must send the right pair\n  per call.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-auth.autopay.io/oauth/token\n    audience: https://api.autopay.io\n    scopes: 3\n    scopes_known:\n    - customer_club\n    - permit_booking\n\
  \    - zone_status\n  transport: 'Authorization: Bearer <access_token>'\n  request:\n    method: POST\n    content_type: application/json\n    body_parameters:\n    - {name: client_id, type: string, required: true}\n    - {name: client_secret, type: string, required: true}\n    - {name: audience, type: string, required: true, fixed_value: https://api.autopay.io}\n    - {name: grant_type, type: string, required: true, fixed_value: client_credentials}\n    note: >-\n      The token request body is JSON, not the application/x-www-form-urlencoded form RFC 6749\n      specifies. A generic OAuth client library configured for form encoding will fail against\n      this endpoint.\n  response:\n    fields:\n    - {name: access_token, type: string}\n    - {name: scope, type: string, description: The Autopay APIs reachable with this token.}\n    - {name: expires_in, type: integer, description: Seconds until expiry; 86400 in the documented example.}\n    - {name: token_type, type: string, fixed_value:\
  \ Bearer}\n  token_lifetime: 'Short-lived: \"usually 10-24 hours\". Read the real value from expires_in.'\n  token_caching_required: true\n  token_caching_note: >-\n    \"Generating excessive access tokens within the expiration time (i.e. requesting a new one\n    for each request) may lead to termination of API access.\" Autopay enforces this\n    contractually, not with a 429 — the penalty is loss of access. Any agent calling this API\n    MUST cache the token for its full expires_in.\n  errors:\n  - {status: 401, body: '{\"error\": \"access_denied\", \"error_description\": \"Unauthorized\"}', cause: Invalid client_id or client_secret.}\n  - {status: 401, body: '{\"error_id\":\"authentication_error\",\"message\":\"No access token present in header!\"}', cause: Request to api.autopay.io with no Authorization header. Observed live 2026-09-06.}\n  description: >-\n    OAuth 2.0 Client Credentials against api-auth.autopay.io with audience\n    https://api.autopay.io. Some endpoints additionally\
  \ require a named scope on the token —\n    permit_booking (Booking API), customer_club (Customer Club API), zone_status (Status API).\n  sources:\n  - https://developer.autopay.io/authentication/\n  - https://api-auth.autopay.io/.well-known/openid-configuration\n  - openapi/autopay-openapi.yml\nauthorization_server:\n  issuer: https://api-auth.autopay.io/\n  token_endpoint: https://api-auth.autopay.io/oauth/token\n  jwks_uri: https://api-auth.autopay.io/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  discovery_document: well-known/autopay-openid-configuration.json\n  probed: '2026-09-06'\n  http_status: 200\n  vendor: Auth0 (inferred from the audience-parameter token request and the discovery document shape; not stated by Autopay)\ncredential_issuance:\n  self_serve: false\n  process: >-\n    \"Contact your Autopay representative to acquire the Client Credentials (Client ID and\n    Secret) for your application.\" There is no developer signup, no console and\
  \ no key-rotation\n    endpoint. The integrator must also register a Technical Contact Person with\n    partner-support@autopay.io, naming the client_id(s) it applies to.\n  rotation: not documented\n  scoping: One credential pair per operator; a credential used against another operator's facilities returns an error.\ntoken_claims_used_by_the_api:\n  note: >-\n    Several documented error ids reveal that Autopay reads tenancy claims out of the token\n    rather than from the request — missing_tenant_id_token_error, missing_landlord_id_token_error,\n    missing_operator_token_error and invalid_operator_id. The tenant, landlord and operator an\n    agent acts as are fixed by the credential, not chosen per call.\noutbound_authentication:\n  note: >-\n    Autopay also authenticates ITSELF to integrator-hosted callback endpoints. Supported methods\n    are Basic, Bearer, API key (X-API-Key) and OAuth2 client credentials — see\n    asyncapi/autopay-webhooks.yml.\ngaps:\n- No OAuth 2.0 Protected\
  \ Resource Metadata (RFC 9728) is served on api.autopay.io.\n- No dynamic client registration.\n- No mTLS, no request signing, no key rotation endpoint.\n- No documented scope reference page; the three scope names above are the only ones the reference mentions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/authentication/autopay-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Parking
- Parking Payments
- Fleet Management
- Permits
- Parking Operators
- Norway
---
