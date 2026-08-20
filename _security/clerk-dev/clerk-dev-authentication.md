---
api_key_in: []
api_specs:
- filename: clerk-dev-allowlist-blocklist-api-openapi.yml
  format: yaml
  label: Clerk Allowlist & Blocklist API
  slug: clerk-dev-allowlist-blocklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-allowlist-blocklist-api-openapi.yml
- filename: clerk-dev-clients-api-openapi.yml
  format: yaml
  label: Clerk Clients API
  slug: clerk-dev-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-clients-api-openapi.yml
- filename: clerk-dev-email-sms-api-openapi.yml
  format: yaml
  label: Clerk Email & SMS API
  slug: clerk-dev-email-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-email-sms-api-openapi.yml
- filename: clerk-dev-invitations-api-openapi.yml
  format: yaml
  label: Clerk Invitations API
  slug: clerk-dev-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-invitations-api-openapi.yml
- filename: clerk-dev-jwks-api-openapi.yml
  format: yaml
  label: Clerk JWKS API
  slug: clerk-dev-jwks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-jwks-api-openapi.yml
- filename: clerk-dev-jwt-templates-api-openapi.yml
  format: yaml
  label: Clerk JWT Templates API
  slug: clerk-dev-jwt-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-jwt-templates-api-openapi.yml
- filename: clerk-dev-oauth-applications-api-openapi.yml
  format: yaml
  label: Clerk OAuth Applications API
  slug: clerk-dev-oauth-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-oauth-applications-api-openapi.yml
- filename: clerk-dev-organization-invitations-api-openapi.yml
  format: yaml
  label: Clerk Organization Invitations API
  slug: clerk-dev-organization-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-organization-invitations-api-openapi.yml
- filename: clerk-dev-organization-memberships-api-openapi.yml
  format: yaml
  label: Clerk Organization Memberships API
  slug: clerk-dev-organization-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-organization-memberships-api-openapi.yml
- filename: clerk-dev-organizations-api-openapi.yml
  format: yaml
  label: Clerk Organizations API
  slug: clerk-dev-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-organizations-api-openapi.yml
- filename: clerk-dev-saml-enterprise-connections-api-openapi.yml
  format: yaml
  label: Clerk SAML & Enterprise Connections API
  slug: clerk-dev-saml-enterprise-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-saml-enterprise-connections-api-openapi.yml
- filename: clerk-dev-sessions-api-openapi.yml
  format: yaml
  label: Clerk Sessions API
  slug: clerk-dev-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-sessions-api-openapi.yml
- filename: clerk-dev-sign-ups-tokens-api-openapi.yml
  format: yaml
  label: Clerk Sign-ups & Tokens API
  slug: clerk-dev-sign-ups-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-sign-ups-tokens-api-openapi.yml
- filename: clerk-dev-users-api-openapi.yml
  format: yaml
  label: Clerk Users API
  slug: clerk-dev-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-users-api-openapi.yml
- filename: clerk-dev-webhooks-api-openapi.yml
  format: yaml
  label: Clerk Webhooks API
  slug: clerk-dev-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/openapi/clerk-dev-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clerk Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clerk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clerk
provider_slug: clerk-dev
scheme_count: 1
schemes:
- description: 'Your Clerk instance Secret Key (starts with sk_test_ or sk_live_) passed as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clerk-dev-openapi.yml
  type: http
slug: clerk-dev-authentication
source_filename: clerk-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clerk-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Your Clerk instance Secret Key (starts with sk_test_ or sk_live_) passed as\n    `Authorization: Bearer [example key]`.'\n  sources:\n  - openapi/clerk-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk-dev/refs/heads/main/authentication/clerk-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- User Management
- Identity
- Sessions
- Organization
- SSO
- JWT
- MFA
---
