---
api_key_in: []
api_specs:
- filename: trusona-verification-api-openapi.yml
  format: yaml
  label: Trusona ATO Protect Verification API
  slug: trusona-ato-protect-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trusona/refs/heads/main/openapi/trusona-verification-api-openapi.yml
- filename: trusona-driver-license-verification-api-openapi.yml
  format: yaml
  label: Trusona Driver License Verification API (IDV API)
  slug: trusona-driver-license-verification-api-idv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trusona/refs/heads/main/openapi/trusona-driver-license-verification-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Trusona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trusona secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trusona
provider_slug: trusona
scheme_count: 1
schemes:
- bearerFormat: JWT
  environment_variables:
  - name: ATOP_TOKEN
    purpose: The Bearer JWT.
    required: true
  - default: https://authcloud.trusona.net
    name: ATOP_BASE_URL
    purpose: API origin; overridable for non-prod.
    required: false
  handling_guidance: Trusona's own reference tells integrators to pass the Authorization header to curl via --config rather than on the command line, so the token stays out of the process argument list, and warns that the residual exposure is the environment variable itself — prefer a short-lived token on a shared host.
  header: Authorization
  name: bearerAuth
  provisioning: out-of-band
  provisioning_note: Neither spec defines a token-issuing endpoint. The JWT is issued from the Trusona dashboard (https://dashboard.trusona.com/) or by an account contact, so there is no programmatic credential-rotation path in the published contract.
  scheme: bearer
  smoke_test: GET /api/v1/verifications?since=2024-01-01T00:00:00Z — any numeric array length (including 0) proves the token works; 401 means missing/expired/wrong, 400 usually means a malformed `since`.
  sources:
  - openapi/trusona-driver-license-verification-api-openapi.yml
  - openapi/trusona-verification-api-openapi.yml
  type: http
  value_format: Bearer <JWT>
slug: trusona-authentication
source_filename: trusona-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: openapi/trusona-driver-license-verification-api-openapi.yml,\n  openapi/trusona-verification-api-openapi.yml\ndocs: https://github.com/trusona/atop-agent-skill/blob/HEAD/reference/auth.md\nnote: 'Derived from both OpenAPI documents, then upgraded from Trusona''s own\n  first-party auth reference (reference/auth.md in the Apache-2.0 ATO Protect Agent\n  Skill), which documents the provisioning model, the environment variables and the\n  token-handling guidance the specs do not carry.'\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\n  applied: 'Globally — both documents declare a root-level security: [{bearerAuth: []}],\n    so every operation on both APIs requires the token.'\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/trusona-driver-license-verification-api-openapi.yml\n  - openapi/trusona-verification-api-openapi.yml\n\
  \  header: Authorization\n  value_format: 'Bearer <JWT>'\n  provisioning: out-of-band\n  provisioning_note: 'Neither spec defines a token-issuing endpoint. The JWT is issued\n    from the Trusona dashboard (https://dashboard.trusona.com/) or by an account contact,\n    so there is no programmatic credential-rotation path in the published contract.'\n  environment_variables:\n  - name: ATOP_TOKEN\n    required: true\n    purpose: The Bearer JWT.\n  - name: ATOP_BASE_URL\n    required: false\n    default: https://authcloud.trusona.net\n    purpose: API origin; overridable for non-prod.\n  handling_guidance: 'Trusona''s own reference tells integrators to pass the Authorization\n    header to curl via --config rather than on the command line, so the token stays out\n    of the process argument list, and warns that the residual exposure is the environment\n    variable itself — prefer a short-lived token on a shared host.'\n  smoke_test: 'GET /api/v1/verifications?since=2024-01-01T00:00:00Z\
  \ — any numeric array\n    length (including 0) proves the token works; 401 means missing/expired/wrong, 400\n    usually means a malformed `since`.'\nlegacy_scheme:\n  api: Trusona ID Proofing API (v2)\n  type: apiKey\n  spec_documented: false\n  note: 'The legacy AAMVA ID Proofing surface uses an API key rather than a bearer JWT\n    and answers 403 (\"Either the API key was not provided or it was invalid\") where the\n    authcloud APIs answer 401. The header name is not published in the integration guide,\n    so it is not recorded here. There is no OpenAPI for this surface.'\n  docs: https://www.trusona.com/integrations/trusona-id-proofing-integration-guide\noauth:\n  present: false\n  note: 'No OAuth 2.0 or OpenID Connect anywhere — no oauth2 securityScheme, no\n    authorization/token endpoints, and /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server both 404 on the API hosts. There is\n    consequently NO scope surface, which is why scopes/ is intentionally\
  \ not emitted\n    rather than left empty.'\nresponse_encryption:\n  supported: true\n  note: 'Beyond transport auth, Trusona offers an encrypted projection of the API at\n    /api/v1/encrypted/verifications: the caller supplies a public key in JWK format\n    (RSA, EC, or OKP with crv=X25519) and verification and document payloads are returned\n    encrypted to it. This is unusual and materially reduces PII exposure in transit\n    logging and at the response boundary.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trusona/refs/heads/main/authentication/trusona-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Authentication
- Identity
- Identity Verification
- Fraud Detection
- Account Takeover
- Security
- Deepfake Detection
- Cybersecurity
- Agent Skills
---
