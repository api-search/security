---
api_key_in: []
api_specs:
- filename: beyond-identity-applications-api-openapi.yml
  format: yaml
  label: Beyond Identity Applications API
  slug: beyond-identity-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-applications-api-openapi.yml
- filename: beyond-identity-authenticator-configurations-api-openapi.yml
  format: yaml
  label: Beyond Identity Authenticator Configurations API
  slug: beyond-identity-authenticator-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-authenticator-configurations-api-openapi.yml
- filename: beyond-identity-credential-binding-jobs-api-openapi.yml
  format: yaml
  label: Beyond Identity Credential Binding Jobs API
  slug: beyond-identity-credential-binding-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-credential-binding-jobs-api-openapi.yml
- filename: beyond-identity-credentials-api-openapi.yml
  format: yaml
  label: Beyond Identity Credentials API
  slug: beyond-identity-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-credentials-api-openapi.yml
- filename: beyond-identity-groups-api-openapi.yml
  format: yaml
  label: Beyond Identity Groups API
  slug: beyond-identity-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-groups-api-openapi.yml
- filename: beyond-identity-identities-api-openapi.yml
  format: yaml
  label: Beyond Identity Identities API
  slug: beyond-identity-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-identities-api-openapi.yml
- filename: beyond-identity-identity-provider-api-openapi.yml
  format: yaml
  label: Beyond Identity Identity Provider API
  slug: beyond-identity-identity-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-identity-provider-api-openapi.yml
- filename: beyond-identity-launch-mechanisms-api-openapi.yml
  format: yaml
  label: Beyond Identity Launch Mechanisms API
  slug: beyond-identity-launch-mechanisms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-launch-mechanisms-api-openapi.yml
- filename: beyond-identity-realms-api-openapi.yml
  format: yaml
  label: Beyond Identity Realms API
  slug: beyond-identity-realms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-realms-api-openapi.yml
- filename: beyond-identity-resource-servers-api-openapi.yml
  format: yaml
  label: Beyond Identity Resource Servers API
  slug: beyond-identity-resource-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-resource-servers-api-openapi.yml
- filename: beyond-identity-roles-api-openapi.yml
  format: yaml
  label: Beyond Identity Roles API
  slug: beyond-identity-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-roles-api-openapi.yml
- filename: beyond-identity-scim-api-openapi.yml
  format: yaml
  label: Beyond Identity SCIM API
  slug: beyond-identity-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-scim-api-openapi.yml
- filename: beyond-identity-sso-configs-api-openapi.yml
  format: yaml
  label: Beyond Identity SSO Configs API
  slug: beyond-identity-sso-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-sso-configs-api-openapi.yml
- filename: beyond-identity-tenants-api-openapi.yml
  format: yaml
  label: Beyond Identity Tenants API
  slug: beyond-identity-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-tenants-api-openapi.yml
- filename: beyond-identity-themes-api-openapi.yml
  format: yaml
  label: Beyond Identity Themes API
  slug: beyond-identity-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-themes-api-openapi.yml
- filename: beyond-identity-tokens-api-openapi.yml
  format: yaml
  label: Beyond Identity Tokens API
  slug: beyond-identity-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/openapi/beyond-identity-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Beyond Identity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beyond Identity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Beyond Identity
provider_slug: beyond-identity
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: See the [Authentication](#section/Authentication) section for details.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/beyond-identity-secure-access-api-openapi.yml
  - openapi/beyond-identity-secure-workforce-api-openapi.yml
  type: http
slug: beyond-identity-authentication
source_filename: beyond-identity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/beyond-identity-secure-access-api-openapi.yml, openapi/beyond-identity-secure-workforce-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: See the [Authentication](#section/Authentication) section for details.\n  sources:\n  - openapi/beyond-identity-secure-access-api-openapi.yml\n  - openapi/beyond-identity-secure-workforce-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-identity/refs/heads/main/authentication/beyond-identity-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Passwordless
- Zero Trust
- Identity
- Passkeys
- MFA
- Device Security
- OAuth 2.0
- OIDC
- SCIM
---
