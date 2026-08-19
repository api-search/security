---
api_key_in:
- header
api_specs:
- filename: coorpacademy-content-openapi.json
  format: json
  label: Coorpacademy Content API
  slug: coorpacademy-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-content-openapi.json
- filename: coorpacademy-platform-openapi.json
  format: json
  label: Coorpacademy Platform API
  slug: coorpacademy-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-platform-openapi.json
- filename: coorpacademy-progression-openapi.json
  format: json
  label: Coorpacademy Progression API
  slug: coorpacademy-progression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-progression-openapi.json
- filename: coorpacademy-progression-aggregations-openapi.json
  format: json
  label: Coorpacademy Progression Aggregations API
  slug: coorpacademy-progression-aggregations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-progression-aggregations-openapi.json
- filename: coorpacademy-scim-openapi.json
  format: json
  label: Coorpacademy SCIM API
  slug: coorpacademy-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-scim-openapi.json
- filename: coorpacademy-content-scorm-openapi.json
  format: json
  label: Coorpacademy SCORM Content API
  slug: coorpacademy-scorm-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-content-scorm-openapi.json
- filename: coorpacademy-scorm-openapi.json
  format: json
  label: Coorpacademy SCORM API
  slug: coorpacademy-scorm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-scorm-openapi.json
- filename: coorpacademy-mail-openapi.json
  format: json
  label: Coorpacademy Email API
  slug: coorpacademy-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-mail-openapi.json
- filename: coorpacademy-mobile-openapi.json
  format: json
  label: Coorpacademy Mobile API
  slug: coorpacademy-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-mobile-openapi.json
- filename: coorpacademy-review-openapi.json
  format: json
  label: Coorpacademy Review API
  slug: coorpacademy-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-review-openapi.json
- filename: coorpacademy-h5p-openapi.json
  format: json
  label: Coorpacademy H5P API
  slug: coorpacademy-h5p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-h5p-openapi.json
- filename: coorpacademy-external-openapi.json
  format: json
  label: Coorpacademy External Resources API
  slug: coorpacademy-external-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-external-openapi.json
- filename: coorpacademy-media-openapi.json
  format: json
  label: Coorpacademy Media API
  slug: coorpacademy-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-media-openapi.json
- filename: coorpacademy-pdf-openapi.json
  format: json
  label: Coorpacademy PDF API
  slug: coorpacademy-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-pdf-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coorpacademy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coorpacademy secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coorpacademy
provider_slug: coorpacademy
scheme_count: 5
schemes:
- in: header
  name: token
  parameter: authorization
  sources:
  - openapi/coorpacademy-content-openapi.json
  - openapi/coorpacademy-review-openapi.json
  type: apiKey
- in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/coorpacademy-content-scorm-openapi.json
  - openapi/coorpacademy-mail-openapi.json
  - openapi/coorpacademy-scorm-openapi.json
  type: apiKey
- in: header
  name: token
  parameter: token
  sources:
  - openapi/coorpacademy-h5p-openapi.json
  - openapi/coorpacademy-scim-openapi.json
  type: apiKey
- in: header
  name: Authorization
  parameter: Api-Secret
  sources:
  - openapi/coorpacademy-mobile-openapi.json
  type: apiKey
- in: header
  name: authentication
  parameter: authentication
  sources:
  - openapi/coorpacademy-platform-openapi.json
  - openapi/coorpacademy-progression-aggregations-openapi.json
  - openapi/coorpacademy-progression-openapi.json
  type: apiKey
slug: coorpacademy-authentication
source_filename: coorpacademy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: derived\nsource: openapi/coorpacademy-content-openapi.json, openapi/coorpacademy-content-scorm-openapi.json,\n  openapi/coorpacademy-h5p-openapi.json, openapi/coorpacademy-mail-openapi.json, openapi/coorpacademy-mobile-openapi.json,\n  openapi/coorpacademy-platform-openapi.json, openapi/coorpacademy-progression-aggregations-openapi.json,\n  openapi/coorpacademy-progression-openapi.json, openapi/coorpacademy-review-openapi.json, openapi/coorpacademy-scim-openapi.json,\n  openapi/coorpacademy-scorm-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/coorpacademy-content-openapi.json\n  - openapi/coorpacademy-review-openapi.json\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/coorpacademy-content-scorm-openapi.json\n  - openapi/coorpacademy-mail-openapi.json\n \
  \ - openapi/coorpacademy-scorm-openapi.json\n- name: token\n  type: apiKey\n  in: header\n  parameter: token\n  sources:\n  - openapi/coorpacademy-h5p-openapi.json\n  - openapi/coorpacademy-scim-openapi.json\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Api-Secret\n  sources:\n  - openapi/coorpacademy-mobile-openapi.json\n- name: authentication\n  type: apiKey\n  in: header\n  parameter: authentication\n  sources:\n  - openapi/coorpacademy-platform-openapi.json\n  - openapi/coorpacademy-progression-aggregations-openapi.json\n  - openapi/coorpacademy-progression-openapi.json\n\n# --- API Evangelist enrichment 2026-08-17: docs search + live probes -------------------------------\ndocs: https://api.coorpacademy.com/\ndocs_note: >-\n  There is NO authentication documentation. The Swagger UI at https://api.coorpacademy.com/ renders the\n  securityScheme declarations and nothing else — no auth guide, no key-issuance page, no developer\n  portal. Searched coorpacademy.com\
  \ (nav, footer, all five sitemaps), support.coorpacademy.com (a\n  learner-facing FAQ with no API content) and github.com/CoorpAcademy. Nothing explains how to obtain a\n  key. Method stays `derived` because there is no prose to upgrade it with.\nmodel:\n  types: [apiKey]\n  transport: header\n  oauth2: false\n  openid_connect: false\n  bearer: false\n  mutual_tls: false\n  basic: false\n  scopes: false\n  key_rotation_documented: false\n  key_issuance_documented: false\nheader_name_inconsistency:\n  distinct_header_names: 5\n  finding: >-\n    The most important fact about authentication here: there is no single header. Five names are used\n    across fourteen services, two of which differ only by letter case, and one of which is non-standard.\n    An integrator must read the per-service specification.\n  map:\n  - header: authorization\n    services: [content, review]\n  - header: Authorization\n    services: [content-scorm, mail, scorm]\n  - header: token\n    services: [h5p, scim]\n\
  \  - header: authentication\n    services: [platform, progression, progression-aggregations]\n  - header: Api-Secret\n    services: [mobile]\nundeclared_services:\n  services: [external, media, pdf]\n  finding: >-\n    Three of the fourteen specs declare no securityScheme at all. They are NOT open: an unauthenticated\n    call to a sibling path on the same host returns HTTP 403 {\"message\":\"Missing Authentication Token\"}\n    — the AWS API Gateway body — so the edge gates them while the contract stays silent about how. This\n    is a documentation gap, not an unauthenticated API.\nobserved:\n  method: probed\n  checked: '2026-08-17'\n  probes:\n  - url: https://content.coorpacademy.com/api/v2/notifications\n    http_status: 401\n    body: '{\"message\":\"Invalid or missing authorization key\"}'\n    server: Express (x-powered-by)\n  - url: https://progression.coorpacademy.com/api/v1/progressions\n    http_status: 401\n    body: >-\n      {\"code\":\"server_error\",\"status\":401,\"\
  success\":false,\"message\":\"Unauthorized\",\"errors\":[{\"message\":\"Unauthorized\",\"code\":\"server_error\",\"status\":401,\"statusCode\":401,\"expose\":true}]}\n    server: Express (x-powered-by)\n  - url: https://platform.coorpacademy.com/api/v1/brands\n    http_status: 401\n    body: '{\"code\":\"server_error\",\"status\":401,\"success\":false,\"message\":\"Unauthorized\",\"errors\":[{\"statusCode\":401,\"status\":401,\"code\":\"server_error\"}]}'\n    server: Express (x-powered-by)\n  - url: https://api.coorpacademy.com/scim/coorp/Users\n    http_status: 400\n    body: >-\n      {\"schemas\":[\"urn:ietf:params:scim:api:messages:2.0:Error\"],\"detail\":\"JWTError: Expecting type:\n      string at key: authorization but instead got: undefined\",\"status\":400}\n    edge: CloudFront (x2) behind Cloudflare\n  - url: https://api.coorpacademy.com/mail/api/v1/welcome\n    http_status: 403\n    body: '{\"message\":\"Missing Authentication Token\"}'\n    edge: AWS API Gateway behind CloudFront\
  \ (x2) behind Cloudflare\ncontract_vs_behaviour_discrepancy:\n  service: scim\n  declared: apiKey in a `token` header\n  observed: >-\n    The 400 body reports \"JWTError: Expecting type: string at key: authorization but instead got:\n    undefined\", which indicates the implementation reads a JWT from an `authorization` header rather than\n    the `token` header the contract names. Two disagreements in one: the header name, and the credential\n    type (a signed JWT, not an opaque key).\n  action: >-\n    Confirm with Coorpacademy which header and credential type are authoritative for SCIM before\n    configuring an identity provider. Recorded in overlays/coorpacademy-scim-overlay.yaml.\n  severity: blocks-integration\ninformation_disclosure:\n  finding: >-\n    Two unauthenticated responses leak implementation detail. The SCIM 400 names an internal JWT library\n    and its parse failure; the three Express hosts return `x-powered-by: Express`. Neither is severe,\n    both are trivially\
  \ removable, and both are the kind of thing a security review flags.\nkey_issuance:\n  self_serve: false\n  documented: false\n  note: >-\n    No signup, no developer portal, no pricing page, no documented key request. API access is negotiated\n    inside a platform contract; commercial contact now routes to Go1\n    (https://www.go1.com/fr/speak-with-an-expert-old). There is a learner login and self-serve learner\n    signup at https://connect.coorpacademy.com/login (email/password plus Facebook, Google and LinkedIn\n    social sign-on), but that is the platform front door, not API access.\nwell_known:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  note: >-\n    Every /.well-known/ path 404s on every host. www and api 301 into an empty S3 bucket. See\n    well-known/coorpacademy-well-known.yml.\nsso_for_end_users:\n  note: >-\n    Distinct from API auth. Coorpacademy brokers enterprise SSO for LEARNERS through the Platform API —\n \
  \   SAML 2.0 (POST /brands/{id}/metadatas parses an IdP metadata.xml) and OIDC, with a claim-to-user\n    mapping (userMappingPayload) per brand. Coorpacademy is an OIDC relying party there, not a provider.\n    See openapi/coorpacademy-platform-openapi.json and skills/coorpacademy-configure-brand-sso.md.\ncross_links:\n  conventions: conventions/coorpacademy-conventions.yml\n  conformance: conformance/coorpacademy-conformance.yml\n  errors: errors/coorpacademy-problem-types.yml\n  scopes: null\n  scopes_note: >-\n    No scopes/ artifact is written and no OAuthScopes pointer is emitted. derive-oauth-scopes.py found\n    zero oauth2 securitySchemes across all fourteen specs; there is no scope surface to document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/authentication/coorpacademy-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Company
- Saas
- corporate-learning
- lms
- learning-experience-platform
- edtech
- elearning
- scorm
- h5p
- scim
- user-provisioning
- learning-analytics
- skills
- certifications
- gamification
- france
- switzerland
---
