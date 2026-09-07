---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aclid-openapi.yml
  format: yaml
  label: Aclid API
  slug: aclid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclid/refs/heads/main/openapi/aclid-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aclid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aclid secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aclid
provider_slug: aclid
scheme_count: 1
schemes:
- documented_in: openapi tag description (not components.securitySchemes)
  in: header
  key_issuance: Self-service from the user profile in the Aclid Dashboard (https://dash.aclid.bio).
  name: AclidApiKey
  parameter_name: Authorization
  prefix_note: The key is sent as the RAW value of the Authorization header with no "Bearer " prefix — both published examples do this. The published example value is a JWT-shaped string (eyJhbGciOiJSUzI1NiIsImtpZCI6...), consistent with the AWS Cognito user pool that backs the Aclid console.
  scheme_prefix: none
  sources:
  - openapi/aclid-openapi.yml
  transport: https-only
  transport_note: All API requests must be made over HTTPS; plain HTTP calls fail.
  type: apiKey
slug: aclid-authentication
source_filename: aclid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://api.aclid.bio/docs\ndocs: https://api.aclid.bio/docs#tag/Authentication\nnote: >-\n  DERIVED FROM THE DOCS, NOT FROM securitySchemes. The Aclid OpenAPI 3.1.0 declares NO\n  components.securitySchemes and no top-level or per-operation security[] requirement, so\n  derive-authentication.py found nothing to aggregate. The auth contract is published as prose in\n  the spec's own \"Authentication\" tag description (rendered at the ReDoc reference above) and is\n  captured here verbatim in structure. This is a real contract gap on Aclid's side: a generated\n  client or an agent reading only the machine-readable half would send unauthenticated requests\n  and get HTTP 403.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  spec_declares_security: false\nschemes:\n- name: AclidApiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  scheme_prefix: none\n  prefix_note: >-\n    The key\
  \ is sent as the RAW value of the Authorization header with no \"Bearer \" prefix — both\n    published examples do this. The published example value is a JWT-shaped string\n    (eyJhbGciOiJSUzI1NiIsImtpZCI6...), consistent with the AWS Cognito user pool that backs the\n    Aclid console.\n  transport: https-only\n  transport_note: All API requests must be made over HTTPS; plain HTTP calls fail.\n  key_issuance: Self-service from the user profile in the Aclid Dashboard (https://dash.aclid.bio).\n  documented_in: openapi tag description (not components.securitySchemes)\n  sources: [openapi/aclid-openapi.yml]\nmodes:\n  live_test_separation: true\n  selector: the API key itself\n  detail: >-\n    \"You can use the Aclid API in test mode, which doesn't affect your live data. The API key you\n    use to authenticate the request determines whether the request is live mode or test mode.\"\n    Aclid publishes no key prefix convention, so a caller cannot tell live from test by inspecting\n  \
  \  the key.\nconsole_identity:\n  note: >-\n    Separate from API-key auth. The Aclid console (dash.aclid.bio) and the customer verification\n    flow (verify.aclid.bio) authenticate END USERS through an AWS Cognito user pool operated by\n    Aclid, whose region and pool id are published in the client configuration of both apps.\n  provider: AWS Cognito\n  region: us-east-1\n  user_pool_id: us-east-1_PJ68v2vt9\n  branded_domain: https://aclid.auth.us-east-1.amazoncognito.com\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_PJ68v2vt9\n  discovery: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_PJ68v2vt9/.well-known/openid-configuration\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_PJ68v2vt9/.well-known/jwks.json\n  oidc_scopes_supported: [openid, email, phone, profile]\n  response_types_supported: [code, token]\n  id_token_signing_alg: RS256\n  federated_identity:\n    orcid: >-\n      The customer verification flow offers \"Link ORCID\" and states\
  \ \"We partnered with ORCID to\n      help verify your information. Your research ID helps expedite the biosecurity review.\"\n      An ORCID client id and https://orcid.org are present in the verify.aclid.bio app config.\n  file: well-known/aclid-openid-configuration.json\n  probed: '2026-09-06'\n  http_status: 200\nobserved:\n- request: GET https://api.aclid.bio/v2/screens (no Authorization header)\n  status: 403\n  body_fields: [auth_detail, detail, path, request_id, request_time, response_type]\n  probed: '2026-09-06'\ngaps:\n- No components.securitySchemes in the published OpenAPI.\n- No security[] requirement on any of the 18 operations.\n- No documented key prefix, so live vs test mode is not inspectable by the caller.\n- No documented key rotation, expiry or revocation procedure.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aclid/refs/heads/main/authentication/aclid-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Biosecurity
- Biosafety
- Compliance
- Synthetic Biology
- Life Sciences
- DNA Sequence Screening
- Sanctions Screening
- Export Control
- Biotechnology
- Risk Assessment
- Know Your Customer
---
