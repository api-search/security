---
api_key_in: []
api_specs:
- filename: bevz-integrator-service-openapi.yaml
  format: yaml
  label: Bevz Integrator Service
  slug: bevz-integrator-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bevz/refs/heads/main/openapi/bevz-integrator-service-openapi.yaml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Bevz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bevz declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bevz
provider_slug: bevz
scheme_count: 1
schemes:
- bearer_format: JWT
  description: 'Every Integrator Service operation requires the Authorization header. The published docs state plainly: "Ensure you include the header: Authorization: Bearer yourJWTtoken in every request."'
  header: Authorization
  id: bearer-jwt
  location: header
  required: true
  scheme: bearer
  type: http
  value_format: Bearer <token>
slug: bevz-authentication
source_filename: bevz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.bevz.com/#tag/Getting-Started\ndocs: https://docs.bevz.com/\nspec: openapi/bevz-integrator-service-openapi.yaml\napi: Bevz Integrator Service\nsummary: >-\n  Bevz protects the Integrator Service with a bearer JWT that an integrator mints from its own\n  email/password credentials. Credentials are not self-serve: Bevz issues sandbox credentials during\n  the development phase and production credentials only after a collaborative sign-off.\nschemes:\n  - id: bearer-jwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    location: header\n    header: Authorization\n    value_format: 'Bearer <token>'\n    description: >-\n      Every Integrator Service operation requires the Authorization header. The published docs state\n      plainly: \"Ensure you include the header: Authorization: Bearer yourJWTtoken in every request.\"\n    required: true\ntoken:\n  issuance:\n    endpoint: POST {baseUrl}/integrators/login\n\
  \    request_fields: [email, password]\n    response_path: data.token\n    documented_at: https://docs.bevz.com/#tag/Getting-Started\n    note: >-\n      The login endpoint is documented in prose and in the quickstart cURL sample but is NOT declared\n      in the OpenAPI paths object — a client cannot discover it from the machine-readable contract.\n  lifetime_days: 30\n  renewal: Log in again to mint a new token. No refresh-token flow is published.\n  claims:\n    source: openapi/_original/yaml/schemas/jwt.yaml\n    fields:\n      - {name: id, description: Integrator user identifier.}\n      - {name: email, description: Integrator user email.}\n      - {name: client, description: 'Caller class. Published enumeration: Integrator | Portal | Retailer.'}\n      - {name: scope, description: Scope claim carried in the JWT. Bevz publishes no scope vocabulary and the documented sample carries \"*\".}\n      - {name: aud, description: 'Audience. Observed value in the published sample: Bevz.'}\n\
  \      - {name: exp, description: Expiry, consistent with the documented 30-day lifetime.}\n    algorithm_note: The published sample token header declares HS256, but Bevz does not document the signing algorithm as a contract, and no JWKS endpoint is published.\noauth2:\n  applies_to_bevz_api: false\n  note: >-\n    Bevz itself does not expose OAuth. OAuth 2.0 appears only as a THIRD-PARTY flow the API brokers:\n    generateOAuth / exchangeCode / provisionStore drive the Uber Eats merchant authorization\n    handshake on the store's behalf, and their 400 responses surface Uber Eats OAuth errors\n    (invalid_client, invalid_grant, invalid_request, invalid_scope, access_denied).\nonboarding:\n  self_serve: false\n  process: >-\n    Email support@bevz.com to request an Integrator account; an Integrator Account Manager runs\n    onboarding. Bevz then provides sandbox credentials plus a required-API checklist, and issues\n    production credentials only after collaborative testing and sign-off.\n\
  \  source: https://docs.bevz.com/#tag/faq\nauthorization:\n  model: tenant-scoped\n  description: >-\n    Authorization is enforced by integrator tenancy, not by scopes. Every path is nested under\n    /integrators/{integrator_id}, and the published errors confirm the boundary is checked:\n    \"Integrator unauthorized to perform this action!\" (401) and \"Unable to access store, can only\n    update store within the Integrator's umbrella\" (400).\n  scopes_published: false\n  roles_published: false\n  edge: >-\n    The API is fronted by AWS API Gateway. Unauthenticated requests to the host return\n    {\"message\":\"Forbidden\"} or {\"message\":\"Missing Authentication Token\"} with HTTP 403, and the\n    spec's shared 403 body is \"User is not authorized to access this resource with an explicit deny\"\n    — the API Gateway authorizer's own wording.\nerrors:\n  - {status: 401, meaning: JWT missing, expired or invalid., remediation: Re-authenticate at POST /integrators/login. Tokens older\
  \ than 30 days are rejected.}\n  - {status: 403, meaning: Gateway authorizer explicit deny., remediation: Confirm the integrator identity is entitled to the resource; contact tech@bevz.com.}\ngaps:\n  - >-\n    The OpenAPI declares NO components.securitySchemes and no security requirement on any of its 30\n    operations. Authentication is modeled as a required `Authorization` header PARAMETER on each\n    operation instead, so generated clients and scanners will read this contract as unauthenticated\n    even though every call needs a bearer token. This is the single highest-value fix available on\n    this contract.\n  - The token-minting endpoint (POST /integrators/login) is absent from paths[].\n  - No JWKS / OIDC discovery document, no /.well-known/openid-configuration, and no published signing algorithm contract.\n  - No scope vocabulary, despite the JWT carrying a scope claim.\n  - No token revocation endpoint and no refresh flow are published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bevz/refs/heads/main/authentication/bevz-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Delivery Management
- Liquor Retail
- Convenience Store
- Point-of-Sale
- Food Delivery
- Retail Technology
- Marketing
- Menu Management
- Order Management
- Webhook
- Integrator API
---
