---
api_key_in:
- header
api_specs:
- filename: truepill-insurance-api-openapi.yml
  format: yaml
  label: Truepill Insurance API
  slug: truepill-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-insurance-api-openapi.yml
- filename: truepill-patients-api-openapi.yml
  format: yaml
  label: Truepill Patients API
  slug: truepill-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-patients-api-openapi.yml
- filename: truepill-prescriptions-api-openapi.yml
  format: yaml
  label: Truepill Prescriptions API
  slug: truepill-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-prescriptions-api-openapi.yml
- filename: truepill-transfers-api-openapi.yml
  format: yaml
  label: Truepill Transfers API
  slug: truepill-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-transfers-api-openapi.yml
- filename: truepill-webhooks-api-openapi.yml
  format: yaml
  label: Truepill Webhooks API
  slug: truepill-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-webhooks-api-openapi.yml
- filename: truepill-fulfillment-api-openapi.yml
  format: yaml
  label: Truepill Fulfillment API
  slug: truepill-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-fulfillment-api-openapi.yml
- filename: truepill-consults-api-openapi.yml
  format: yaml
  label: Truepill Consults API
  slug: truepill-consults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-consults-api-openapi.yml
- filename: truepill-diagnostics-api-openapi.yml
  format: yaml
  label: Truepill Diagnostics API
  slug: truepill-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-diagnostics-api-openapi.yml
- filename: truepill-media-api-openapi.yml
  format: yaml
  label: Truepill Media API
  slug: truepill-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-media-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Truepill Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truepill secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Truepill
provider_slug: truepill
scheme_count: 1
schemes:
- applied_globally: true
  description: Every FuzeRx endpoint is authenticated with a single provisioned API key sent in the Authorization header, prefixed with the literal token "ApiKey". The published documentation calls this "HTTP Basic Auth" but the wire format is a bearer-style opaque key, not RFC 7617 base64 credentials. The key is provisioned by Fuze Health during commercial onboarding — there is no self-serve key issuance, no OAuth authorization server, and no scope model.
  format: 'Authorization: ApiKey <YOUR API KEY>'
  in: header
  name: apiKey
  parameter: Authorization
  scheme_prefix: ApiKey
  sources:
  - openapi/truepill-patients-api-openapi.yml
  - openapi/truepill-prescriptions-api-openapi.yml
  - openapi/truepill-transfers-api-openapi.yml
  - openapi/truepill-insurance-api-openapi.yml
  - openapi/truepill-webhooks-api-openapi.yml
  - openapi/truepill-fulfillment-api-openapi.yml
  - openapi/truepill-diagnostics-api-openapi.yml
  - openapi/truepill-consults-api-openapi.yml
  - openapi/truepill-media-api-openapi.yml
  - https://rxdocs.fuzehealth.com
  type: apiKey
slug: truepill-authentication
source_filename: truepill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://rxdocs.fuzehealth.com (Overview → Authentication, Making Requests, Environments)\ndocs: https://rxdocs.fuzehealth.com\nspec_source: openapi/_original/truepill-fuzerx-swagger.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  environments: 2\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_prefix: ApiKey\n  format: 'Authorization: ApiKey <YOUR API KEY>'\n  description: >-\n    Every FuzeRx endpoint is authenticated with a single provisioned API key sent\n    in the Authorization header, prefixed with the literal token \"ApiKey\". The\n    published documentation calls this \"HTTP Basic Auth\" but the wire format is a\n    bearer-style opaque key, not RFC 7617 base64 credentials. The key is\n    provisioned by Fuze Health during commercial onboarding — there is no\n    self-serve key issuance, no\
  \ OAuth authorization server, and no scope model.\n  applied_globally: true\n  sources:\n  - openapi/truepill-patients-api-openapi.yml\n  - openapi/truepill-prescriptions-api-openapi.yml\n  - openapi/truepill-transfers-api-openapi.yml\n  - openapi/truepill-insurance-api-openapi.yml\n  - openapi/truepill-webhooks-api-openapi.yml\n  - openapi/truepill-fulfillment-api-openapi.yml\n  - openapi/truepill-diagnostics-api-openapi.yml\n  - openapi/truepill-consults-api-openapi.yml\n  - openapi/truepill-media-api-openapi.yml\n  - https://rxdocs.fuzehealth.com\nkey_issuance:\n  self_serve: false\n  process: >-\n    Two keys are issued per customer during onboarding — one sandbox key and one\n    production key. The environment is selected purely by which key is presented,\n    together with the matching base host.\n  contact: rx.support@fuzehealth.com\nkey_prefixes:\n- environment: production\n  prefix: tp_live_key_\n  source: https://rxdocs.fuzehealth.com (Create a Patient curl example)\n- environment:\
  \ sandbox\n  prefix: tp_test_key_\n  source: https://rxdocs.fuzehealth.com (Sandbox Testing with Simulations curl examples)\nfailure_response:\n  status: 401\n  body_shape: '{\"statusCode\": 401, \"error\": \"Unauthorized\", \"message\": \"Please Send an Api Key\"}'\n  observed: https://rxapi.fuzehealth.com/ (unauthenticated GET, probed 2026-08-14)\n  note: >-\n    The API host returns this challenge for every path except /swagger.json,\n    which is served anonymously.\ntransport:\n  tls: TLS 1.2 or higher\n  source: https://rxdocs.fuzehealth.com (HIPAA & Security)\n  note: Documentation states all API requests are transmitted over TLS 1.2 and all data is encrypted in transit and at rest.\nscopes: none\nnotes: >-\n  There is no OAuth 2.0 or OpenID Connect surface, so no scopes/ artifact is\n  emitted for this provider. Authorization is coarse: one key grants the whole\n  contracted surface. The /v1/insurance_claim family is described in the docs as\n  access-restricted, which implies\
  \ per-account entitlements rather than\n  token-level scoping.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/authentication/truepill-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Pharmacy
- Healthcare
- Prescription Fulfillment
- Telehealth
- Diagnostics
- Insurance
- Copay Adjudication
- Prior Authorization
- Electronic Prescribing
- Pharmacy Transfers
- Webhooks
- HIPAA
---
