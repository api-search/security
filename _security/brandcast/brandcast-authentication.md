---
api_key_in:
- header
api_specs:
- filename: brandcast-websites-openapi.yml
  format: yaml
  label: Brandcast API
  slug: brandcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-websites-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Brandcast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brandcast secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Brandcast
provider_slug: brandcast
scheme_count: 2
schemes:
- description: Brandcast API requests are authenticated with an API key sent in the x-api-key HTTP header over HTTPS. Keys are issued by Brandcast and are tied to the developer's Brandcast account. This is the only authentication a third-party developer can use.
  in: header
  name: apiKeyHeader
  parameter_name: x-api-key
  required_on: all 26 published operations
  sources:
  - https://developer.brandcast.io/
  - openapi/_original/websites.json
  transport: https-only
  type: apiKey
- bearer_format: JWT
  companion_header:
    description: '"The account context for this action. Required when using Authorization header." Supplies which Brandcast account the JWT is acting for.'
    name: x-account-id
  description: '"A valid JWT. Only required when called by Design Studio." An internal first-party credential accepted on the three website export operations alongside the API key. Brandcast publishes no authorization server, token endpoint, scope set, JWT issuer, audience or key-rotation guidance for it, so it is not usable by third-party developers — recorded because it appears verbatim in the provider''s own contract.'
  in: header
  name: designStudioJWT
  parameter_name: Authorization
  required: false
  required_on:
  - createExportJob
  - getExportJob
  - getExportList
  scheme: bearer
  sources:
  - openapi/_original/websites.json
  type: http
slug: brandcast-authentication
source_filename: brandcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.brandcast.io/\ndocs: https://developer.brandcast.io/\nspec_source: >-\n  openapi/_original/{account,templates,websites,salesforce}.json — the Brandcast\n  Swagger 1.2 declarations published at\n  https://s3.amazonaws.com/apidoc.brandcast-prod.io/ and loaded by the Swagger\n  UI on developer.brandcast.io\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  transport: https-only\n  required_on: all 26 published operations\n  description: >-\n    Brandcast API requests are authenticated with an API key sent in the\n    x-api-key HTTP header over HTTPS. Keys are issued by Brandcast and are tied\n    to the developer's Brandcast account. This is the only authentication a\n    third-party developer can use.\n  sources:\n  - https://developer.brandcast.io/\n\
  \  - openapi/_original/websites.json\n- name: designStudioJWT\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  parameter_name: Authorization\n  required: false\n  required_on:\n  - createExportJob\n  - getExportJob\n  - getExportList\n  companion_header:\n    name: x-account-id\n    description: >-\n      \"The account context for this action. Required when using Authorization\n      header.\" Supplies which Brandcast account the JWT is acting for.\n  description: >-\n    \"A valid JWT. Only required when called by Design Studio.\" An internal\n    first-party credential accepted on the three website export operations\n    alongside the API key. Brandcast publishes no authorization server, token\n    endpoint, scope set, JWT issuer, audience or key-rotation guidance for it,\n    so it is not usable by third-party developers — recorded because it appears\n    verbatim in the provider's own contract.\n  sources:\n  - openapi/_original/websites.json\nkey_management:\n\
  \  issuance: vendor-issued\n  self_service: false\n  rotation_policy_published: false\n  expiry_published: false\n  key_prefix_published: false\n  note: >-\n    Keys are provisioned by Brandcast and bound to a Brandcast account. No\n    self-service key creation, rotation, scoping or revocation flow is\n    documented, and no key prefix convention is published.\nscopes:\n  supported: false\n  note: >-\n    The API has no scope or permission model — a key is all-or-nothing across\n    all 26 operations, including destructive ones (deleteWebsite,\n    unpublishWebsite). No scopes/ artifact is emitted, per the pipeline's\n    OAuth-only rule for that artifact.\nmfa: null\nnotes: >-\n  Round 2 upgrade. The prior round recorded the x-api-key scheme correctly from\n  the developer portal prose but stated that no specification is published;\n  that is now superseded — Brandcast does publish a machine-readable contract\n  (Swagger 1.2) at s3.amazonaws.com/apidoc.brandcast-prod.io, and the auth\n\
  \  model above is confirmed against it parameter by parameter. The second scheme\n  (Design Studio JWT + x-account-id) was found only in that contract and does\n  not appear in the portal prose at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/authentication/brandcast-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Enterprise Software
- No-Code
- Website Builder
- Content Management
- Digital Experience
- Web Design
- Brand Management
---
