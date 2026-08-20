---
api_key_in:
- header
api_specs:
- filename: hyperlabs-web-openapi-original.json
  format: json
  label: HYPERLABS Web API
  slug: hyperlabs-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperlabs/refs/heads/main/openapi/hyperlabs-web-openapi-original.json
- filename: hyperlabs-radium-asyncapi.yml
  format: yaml
  label: HYPERLABS Radium gRPC API (TDR11100)
  slug: hyperlabs-radium-grpc-api-tdr11100
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperlabs/refs/heads/main/asyncapi/hyperlabs-radium-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hyperlabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: HYPERLABS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HYPERLABS
provider_slug: hyperlabs
scheme_count: 1
schemes:
- description: 'Standard Authorization header using the Bearer scheme. Example: "Bearer {token}"'
  in: header
  name: oauth2
  parameter: Authorization
  sources:
  - openapi/hyperlabs-web-openapi-original.json
  type: apiKey
  x-actual-type: http-bearer
  x-correction: The scheme KEY is "oauth2" but the declaration is type apiKey in the Authorization header. There is no authorizationUrl, no tokenUrl, no scopes and no flows object anywhere in the spec, so this is a bearer token, not an OAuth 2.0 scheme. Generators and scanners that key off the scheme name will mis-model this API. Corrected in overlays/hyperlabs-web-overlay.yaml.
slug: hyperlabs-authentication
source_filename: hyperlabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/hyperlabs-web-openapi-original.json + grpc/hyperlabs-radium.proto + live probes\ndocs: https://www.hyperlabs.com/api/swagger/index.html\nnotes: >-\n  HYPERLABS publishes no written authentication guide. This profile is derived from the published\n  OpenAPI securityScheme, the token-issuing operations and their response schemas, and observed live\n  behaviour. Baseline produced by 0-working/derive-authentication.py, then enriched with the token\n  issuance flow, the federated sign-in providers, the anonymous/protected operation split and the gRPC\n  surface — none of which the mechanical pass can see.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  effective_model: bearer-jwt\nschemes:\n- name: oauth2\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Standard Authorization header using the Bearer scheme. Example: \"Bearer {token}\"'\n  sources:\n  - openapi/hyperlabs-web-openapi-original.json\n\
  \  x-correction: >-\n    The scheme KEY is \"oauth2\" but the declaration is type apiKey in the Authorization header. There is\n    no authorizationUrl, no tokenUrl, no scopes and no flows object anywhere in the spec, so this is a\n    bearer token, not an OAuth 2.0 scheme. Generators and scanners that key off the scheme name will\n    mis-model this API. Corrected in overlays/hyperlabs-web-overlay.yaml.\n  x-actual-type: http-bearer\ntoken_issuance:\n- operation: 'POST /v1/account/login'\n  request: 'CustomerLoginDto {userName, password}'\n  response: 'CustomerLoginResultDto {tokenType, accessToken}'\n  anonymous: true\n- operation: 'POST /v1/account/google/login'\n  precedes_with: 'GET /v1/account/google/params (returns CustomerGoogleParamsDto {clientId})'\n  request: CustomerGoogleLoginDto\n  response: CustomerLoginResultDto\n  anonymous: true\n  errors: 400 with RFC 7807 ProblemDetails\n- operation: 'POST /v1/account/microsoft/login'\n  precedes_with: 'GET /v1/account/microsoft/params\
  \ (returns CustomerMicrosoftParamsDto {clientId})'\n  request: CustomerMicrosoftLoginDto\n  response: CustomerLoginResultDto\n  anonymous: true\n  errors: 400 with RFC 7807 ProblemDetails\n- operation: 'POST /v1/admin/account/login'\n  note: separate staff login issuing LoginResultDto for the /v1/admin surface\nfederated_identity:\n  role: relying-party\n  providers: [Google, Microsoft]\n  discovery_document_published: false\n  notes: >-\n    HYPERLABS consumes Google and Microsoft OIDC sign-in; it is not itself an OIDC provider and serves\n    no /.well-known/openid-configuration.\naccount_lifecycle:\n  register: 'POST /v1/account/register (RegisterCustomerDto) -> 204'\n  confirm: 'POST /v1/account/confirm-registration'\n  forgot_password: 'POST /v1/account/forgot-password -> 204'\n  reset_password: 'POST /v1/account/reset-password -> 204'\n  change_password: 'POST /v1/account/change-password (authenticated) -> 204'\nauthorization:\n  model: role-based\n  roles_endpoint: 'GET /v1/admin/roles'\n\
  \  surfaces:\n  - {prefix: /v1/admin, operations: 115, audience: staff}\n  - {prefix: '/v1/customer + /v1/profile', audience: authenticated customer}\n  - {prefix: 'other /v1', audience: anonymous public}\n  scopes: none — no OAuth scope surface exists, so no scopes/ artifact is emitted\noperation_split:\n  total: 175\n  protected: 121\n  anonymous: 54\n  note: 'protected operations declare security [{oauth2: []}] with 401 and 403 responses'\nbot_protection:\n  mechanism: Google reCAPTCHA\n  applies_to:\n  - 'POST /v1/request-quote'\n  - 'POST /v1/contact-messages'\n  - 'POST /v1/wishlist/quote'\n  - 'POST /v1/wishlist/share'\n  - 'POST /v1/customer/wishlist/quote'\n  field: recaptchaToken\n  site_key_exposure: 'the public site key is served in the clear at https://www.hyperlabs.com/config/config.js (expected — reCAPTCHA site keys are public by design)'\ngrpc:\n  service: radium.v1.Radium\n  source: grpc/hyperlabs-radium.proto\n  authentication: none\n  transport_security: none\n  evidence:\
  \ >-\n    The provider's own published sample client (TDR11100_gRPC_public.py) opens\n    grpc.insecure_channel(f\"{ip}:50052\") — plaintext, no TLS, no credentials, and no per-call metadata\n    other than an optional \"req_id\" correlation key. Anyone with network reach to the instrument can\n    control it, including Reset and UploadLicense. This is a local-lab-network trust model.\n  licensing: >-\n    The service does gate capability by license (GetLicenseStatus, GetLicenseInfo, UploadLicense,\n    GenerateLicenseRequest, ReloadLicense) — that is entitlement, not authentication.\nx-evidence:\n  fetched: '2026-08-01'\n  sources:\n  - {url: 'https://www.hyperlabs.com/api/swagger/v1/swagger.json', http_status: 200}\n  - {url: 'https://www.hyperlabs.com/api/v1/website/contact', http_status: 200, note: anonymous call succeeded with no Authorization header}\n  - {url: 'https://www.hyperlabs.com/config/config.js', http_status: 200}\n  - {url: 'https://github.com/HYPERLABS/TDR11100', http_status:\
  \ 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperlabs/refs/heads/main/authentication/hyperlabs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- signal-integrity
- Test and Measurement
- Electronic Components
- Instrumentation
- time-domain-reflectometry
- high-speed-digital
- Datacom
- Hardware
- gRPC
- Manufacturing
---
