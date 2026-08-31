---
api_key_in: []
api_specs:
- filename: respondology-comment-results-api-openapi.yml
  format: yaml
  label: Respondology Comment Results API
  slug: respondology-comment-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-comment-results-api-openapi.yml
- filename: respondology-comments-api-openapi.yml
  format: yaml
  label: Respondology Comments API
  slug: respondology-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-comments-api-openapi.yml
- filename: respondology-moderation-reasons-api-openapi.yml
  format: yaml
  label: Respondology Moderation Reasons API
  slug: respondology-moderation-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-moderation-reasons-api-openapi.yml
- filename: respondology-post-results-api-openapi.yml
  format: yaml
  label: Respondology Post Results API
  slug: respondology-post-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-post-results-api-openapi.yml
- filename: respondology-posts-api-openapi.yml
  format: yaml
  label: Respondology Posts API
  slug: respondology-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-posts-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Respondology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Respondology declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Respondology
provider_slug: respondology
scheme_count: 1
schemes:
- applies_to: all 8 external_api operations (comments and posts); GET /moderation_reasons declares no key
  description: API key issued during onboarding. The OpenAPI declares it as a required header PARAMETER on each operation rather than as a components.securitySchemes entry.
  id: api_key_header
  in: header
  name: X-Api-Key
  required: true
  type: apiKey
  unauthorized_response:
    body:
      error: API key not found
    status: 401
slug: respondology-authentication
source_filename: respondology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: https://api.respondology.io/swagger.json — X-Api-Key header parameter on every operation + info.description\n  onboarding text\napi: respondology-api\nsummary: API-key authentication via a required X-Api-Key request header. Keys are issued by a Respondology\n  account manager during onboarding; there is no self-service key provisioning.\nschemes:\n- id: api_key_header\n  type: apiKey\n  in: header\n  name: X-Api-Key\n  required: true\n  applies_to: all 8 external_api operations (comments and posts); GET /moderation_reasons declares no\n    key\n  description: API key issued during onboarding. The OpenAPI declares it as a required header PARAMETER\n    on each operation rather than as a components.securitySchemes entry.\n  unauthorized_response:\n    status: 401\n    body:\n      error: API key not found\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes: false\nprovisioning:\n  self_service: false\n  method: contact\
  \ Respondology to set up an account and receive an API key and secret\n  source: OpenAPI info.description Getting Started section\n  contact: support@respondology.com\nfindings:\n- The spec declares NO components.securitySchemes and no top-level or per-operation security[] block.\n  Auth is modeled only as a required X-Api-Key header parameter, so generated clients will not treat it\n  as a security requirement.\n- info.description states onboarding issues \"your API key and secret\", but only the key (X-Api-Key) appears\n  anywhere in the contract. The secret has no documented use, header, or signing scheme in the published\n  spec.\nrecommendations:\n- Declare an apiKey securityScheme in components.securitySchemes and reference it from security[] so tooling\n  enforces it.\n- Document what the issued secret is for (webhook signature verification is the likely intent) or remove\n  it from the onboarding text.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/authentication/respondology-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Content Moderation
- Social Media
- Comment Moderation
- Trust and Safety
- Artificial Intelligence
- Brand Protection
- Social Listening
- Webhooks
- Marketing
---
