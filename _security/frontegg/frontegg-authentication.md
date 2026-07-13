---
api_key_in: []
api_specs:
- filename: frontegg-identity-openapi.yml
  format: yaml
  label: Frontegg Authentication and Identity Management API
  slug: frontegg-identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-identity-openapi.yml
- filename: frontegg-tenants-openapi.yml
  format: yaml
  label: Frontegg Account Management API
  slug: frontegg-tenants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-tenants-openapi.yml
- filename: frontegg-sso-openapi.yml
  format: yaml
  label: Frontegg Single Sign-On API
  slug: frontegg-sso
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-sso-openapi.yml
- filename: frontegg-scim-openapi.yml
  format: yaml
  label: Frontegg SCIM Provisioning API
  slug: frontegg-scim
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-scim-openapi.yml
- filename: frontegg-entitlements-openapi.yml
  format: yaml
  label: Frontegg Entitlements API
  slug: frontegg-entitlements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-entitlements-openapi.yml
- filename: frontegg-entitlements-agent-openapi.yml
  format: yaml
  label: Frontegg Entitlements Agent (PDP)
  slug: frontegg-entitlements-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-entitlements-agent-openapi.yml
- filename: frontegg-applications-openapi.yml
  format: yaml
  label: Frontegg Multi-Apps API
  slug: frontegg-applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-applications-openapi.yml
- filename: frontegg-audits-openapi.yml
  format: yaml
  label: Frontegg Audits API
  slug: frontegg-audits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-audits-openapi.yml
- filename: frontegg-env-auth-openapi.yml
  format: yaml
  label: Frontegg Environment Authentication API
  slug: frontegg-env-auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-env-auth-openapi.yml
- filename: frontegg-combined-openapi.yml
  format: yaml
  label: Frontegg Combined API
  slug: frontegg-combined
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-combined-openapi.yml
- filename: frontegg-webhooks-asyncapi.yml
  format: yaml
  label: Frontegg Webhooks
  slug: frontegg-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/asyncapi/frontegg-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Frontegg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frontegg secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Frontegg
provider_slug: frontegg
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/frontegg-applications-openapi.yml
  - openapi/frontegg-audits-openapi.yml
  - openapi/frontegg-combined-openapi.yml
  - openapi/frontegg-entitlements-openapi.yml
  - openapi/frontegg-identity-openapi.yml
  - openapi/frontegg-scim-openapi.yml
  - openapi/frontegg-sso-openapi.yml
  - openapi/frontegg-tenants-openapi.yml
  type: http
slug: frontegg-authentication
source_filename: frontegg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/frontegg-applications-openapi.yml, openapi/frontegg-audits-openapi.yml, openapi/frontegg-combined-openapi.yml,\n  openapi/frontegg-entitlements-openapi.yml, openapi/frontegg-identity-openapi.yml, openapi/frontegg-scim-openapi.yml,\n  openapi/frontegg-sso-openapi.yml, openapi/frontegg-tenants-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/frontegg-applications-openapi.yml\n  - openapi/frontegg-audits-openapi.yml\n  - openapi/frontegg-combined-openapi.yml\n  - openapi/frontegg-entitlements-openapi.yml\n  - openapi/frontegg-identity-openapi.yml\n  - openapi/frontegg-scim-openapi.yml\n  - openapi/frontegg-sso-openapi.yml\n  - openapi/frontegg-tenants-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/authentication/frontegg-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Authorization
- Identity Management
- CIAM
- B2B SaaS
- Multi-Tenancy
- RBAC
- SSO
- SCIM
- Entitlements
- OAuth
- OpenID Connect
---
