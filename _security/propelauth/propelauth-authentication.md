---
api_key_in: []
api_specs:
- filename: propelauth-api-keys-api-openapi.yml
  format: yaml
  label: PropelAuth End-User API Keys API
  slug: propelauth-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-api-keys-api-openapi.yml
- filename: propelauth-oauth2-api-openapi.yml
  format: yaml
  label: PropelAuth OAuth2 API
  slug: propelauth-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-oauth2-api-openapi.yml
- filename: propelauth-access-tokens-api-openapi.yml
  format: yaml
  label: PropelAuth Access Tokens API
  slug: propelauth-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-access-tokens-api-openapi.yml
- filename: propelauth-discovery-api-openapi.yml
  format: yaml
  label: PropelAuth Discovery API
  slug: propelauth-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-discovery-api-openapi.yml
- filename: propelauth-dynamic-client-registration-api-openapi.yml
  format: yaml
  label: PropelAuth Dynamic Client Registration API
  slug: propelauth-dynamic-client-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-dynamic-client-registration-api-openapi.yml
- filename: propelauth-employees-api-openapi.yml
  format: yaml
  label: PropelAuth Employees API
  slug: propelauth-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-employees-api-openapi.yml
- filename: propelauth-invites-api-openapi.yml
  format: yaml
  label: PropelAuth Invites API
  slug: propelauth-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-invites-api-openapi.yml
- filename: propelauth-magic-links-api-openapi.yml
  format: yaml
  label: PropelAuth Magic Links API
  slug: propelauth-magic-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-magic-links-api-openapi.yml
- filename: propelauth-mcp-oauth-2-1-api-openapi.yml
  format: yaml
  label: PropelAuth MCP OAuth 2.1 API
  slug: propelauth-mcp-oauth-2-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-mcp-oauth-2-1-api-openapi.yml
- filename: propelauth-members-api-openapi.yml
  format: yaml
  label: PropelAuth Members API
  slug: propelauth-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-members-api-openapi.yml
- filename: propelauth-metadata-api-openapi.yml
  format: yaml
  label: PropelAuth Metadata API
  slug: propelauth-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-metadata-api-openapi.yml
- filename: propelauth-migration-api-openapi.yml
  format: yaml
  label: PropelAuth Migration API
  slug: propelauth-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-migration-api-openapi.yml
- filename: propelauth-organizations-api-openapi.yml
  format: yaml
  label: PropelAuth Organizations API
  slug: propelauth-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-organizations-api-openapi.yml
- filename: propelauth-role-mappings-api-openapi.yml
  format: yaml
  label: PropelAuth Role Mappings API
  slug: propelauth-role-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-role-mappings-api-openapi.yml
- filename: propelauth-sessions-api-openapi.yml
  format: yaml
  label: PropelAuth Sessions API
  slug: propelauth-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-sessions-api-openapi.yml
- filename: propelauth-usage-api-openapi.yml
  format: yaml
  label: PropelAuth Usage API
  slug: propelauth-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-usage-api-openapi.yml
- filename: propelauth-users-api-openapi.yml
  format: yaml
  label: PropelAuth Users API
  slug: propelauth-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-users-api-openapi.yml
- filename: propelauth-validation-api-openapi.yml
  format: yaml
  label: PropelAuth Validation API
  slug: propelauth-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-validation-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Propelauth Authentication
name_suffix: Authentication
oauth_flows: []
overview: PropelAuth secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PropelAuth
provider_slug: propelauth
scheme_count: 1
schemes:
- name: BackendApiKey
  scheme: bearer
  sources:
  - openapi/propelauth-api-keys-api-openapi.yml
  - openapi/propelauth-oauth2-api-openapi.yml
  - openapi/propelauth-org-api-openapi.yml
  - openapi/propelauth-user-api-openapi.yml
  type: http
slug: propelauth-authentication
source_filename: propelauth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/propelauth-api-keys-api-openapi.yml, openapi/propelauth-oauth2-api-openapi.yml,\n  openapi/propelauth-org-api-openapi.yml, openapi/propelauth-user-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BackendApiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/propelauth-api-keys-api-openapi.yml\n  - openapi/propelauth-oauth2-api-openapi.yml\n  - openapi/propelauth-org-api-openapi.yml\n  - openapi/propelauth-user-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/authentication/propelauth-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Identity
- B2B
- Multi-Tenancy
- Authorization
- RBAC
- SSO
- SCIM
- MCP
- APIKeys
---
