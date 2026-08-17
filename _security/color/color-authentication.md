---
api_key_in:
- header
api_specs:
- filename: color-external-api-v1-openapi.yml
  format: yaml
  label: Color External API V1
  slug: color-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/color/refs/heads/main/openapi/color-external-api-v1-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Color Authentication
name_suffix: Authentication
oauth_flows: []
overview: Color secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Color
provider_slug: color
scheme_count: 1
schemes:
- applied: root-level security requirement, so every one of the 13 operations requires it
  description: Per-environment API token in the Authorization header. Obtain separate staging and production tokens from Color.
  header_name: Authorization
  in: header
  name: Bearer
  note: 'Color declares this as an apiKey-in-header scheme rather than http/bearer even though the value carries the "Bearer " prefix. Tooling that keys off `scheme: bearer` will not recognise it. Verbatim from Color''s spec; not corrected here.'
  sources:
  - openapi/_original/color-external-api-v1-openapi.json
  type: apiKey
  value_format: Bearer <token>
slug: color-authentication
source_filename: color-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://docs.color.com/reference\ndocs: https://docs.color.com/docs/getting-started-with-color-apis\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    API access uses a per-environment static bearer token issued by Color and sent\n    as \"Authorization: Bearer <token>\". Staging and production each have their own\n    token and base host, and tokens are handed out by a Color representative during\n    partner onboarding — there is no self-service key issuance. Portal/user sign-in\n    is separate and handled via SAML 2.0 SSO.\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  header_name: Authorization\n  value_format: Bearer <token>\n  applied: root-level security requirement, so every one of the 13 operations requires\n    it\n  description: >-\n    Per-environment API token in the Authorization header. Obtain separate staging\n    and production tokens from Color.\n\
  \  sources:\n  - openapi/_original/color-external-api-v1-openapi.json\n  note: >-\n    Color declares this as an apiKey-in-header scheme rather than http/bearer even\n    though the value carries the \"Bearer \" prefix. Tooling that keys off\n    `scheme: bearer` will not recognise it. Verbatim from Color's spec; not\n    corrected here.\nissuance:\n  self_service: false\n  process: Requested from a Color representative during partner onboarding.\n  environments:\n    production: https://api.color.com/api/v1/external\n    staging: https://api.staging.color.com/api/v1/external\n    staging_legacy: https://external.staging.color.com/api/v1\n  rotation_policy: not published\n  expiry: not published\nfailure_semantics:\n  status: 403\n  body: Authentication token was not provided or accepted.\n  note: >-\n    Color returns 403, not 401, and sends no WWW-Authenticate challenge. An agent\n    branching on 401 will never see an auth failure from this API.\nscopes:\n  supported: false\n  note:\
  \ >-\n    No OAuth and no scope surface. Authorisation is implicit in the token — a token\n    is bound to an organisation and its populations. scopes/ is deliberately not\n    emitted.\nsso:\n  protocol: SAML 2.0\n  idp_initiated: false\n  acs_url: https://colorhealth.kinde.com/login/saml/callback\n  sp_initiated_bookmark: https://home.color.com/start-sso?domain=<email_domain>\n  identity_platform: Kinde\n  docs: https://docs.color.com/docs/sso-integration\n  note: Portal sign-in only; not usable for API authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/color/refs/heads/main/authentication/color-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Health
- Healthcare
- Genomics
- Oncology
- Cancer Care
- Preventive Health
- Eligibility
- Virtual Care
- Diagnostics
- Laboratory
- Employee Benefits
---
