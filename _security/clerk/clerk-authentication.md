---
api_key_in: []
api_specs:
- filename: clerk-webhooks-asyncapi.yml
  format: yaml
  label: Clerk Webhooks (Svix)
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/asyncapi/clerk-webhooks-asyncapi.yml
- filename: clerk-invitations-api-openapi.yml
  format: yaml
  label: Clerk Invitations API
  slug: clerk-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/openapi/clerk-invitations-api-openapi.yml
- filename: clerk-jwttemplates-api-openapi.yml
  format: yaml
  label: Clerk JwtTemplates API
  slug: clerk-jwttemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/openapi/clerk-jwttemplates-api-openapi.yml
- filename: clerk-organizations-api-openapi.yml
  format: yaml
  label: Clerk Organizations API
  slug: clerk-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/openapi/clerk-organizations-api-openapi.yml
- filename: clerk-sessions-api-openapi.yml
  format: yaml
  label: Clerk Sessions API
  slug: clerk-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/openapi/clerk-sessions-api-openapi.yml
- filename: clerk-signintokens-api-openapi.yml
  format: yaml
  label: Clerk SignInTokens API
  slug: clerk-signintokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/openapi/clerk-signintokens-api-openapi.yml
- filename: clerk-users-api-openapi.yml
  format: yaml
  label: Clerk Users API
  slug: clerk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/openapi/clerk-users-api-openapi.yml
- filename: clerk-webhooks-api-openapi.yml
  format: yaml
  label: Clerk Webhooks API
  slug: clerk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk/refs/heads/main/openapi/clerk-webhooks-api-openapi.yml
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
