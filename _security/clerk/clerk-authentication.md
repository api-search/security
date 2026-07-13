---
api_key_in: []
api_specs:
- filename: openapi-specs
  format: yaml
  label: Clerk Backend API
  slug: backend-api
  spec_type: OpenAPI
  url: https://github.com/clerk/openapi-specs
- filename: clerk-webhooks-asyncapi.yml
  format: yaml
  label: Clerk Webhooks (Svix)
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/asyncapi/clerk-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clerk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clerk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clerk
provider_slug: clerk
scheme_count: 1
schemes:
- description: Clerk secret key (sk_test_... or sk_live_...)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/clerk-openapi.yml
  type: http
slug: clerk-authentication
source_filename: clerk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clerk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Clerk secret key (sk_test_... or sk_live_...)\n  sources:\n  - openapi/clerk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/authentication/clerk-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- User Management
- Identity
- Passkeys
- MFA
- B2B
- Organizations
- Billing
---
