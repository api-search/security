---
api_key_in: []
api_specs:
- filename: scalekit-admin-portal-api-openapi.yml
  format: yaml
  label: Scalekit Admin Portal API
  slug: scalekit-admin-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-admin-portal-api-openapi.yml
- filename: scalekit-authentication-api-openapi.yml
  format: yaml
  label: Scalekit Authentication API
  slug: scalekit-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-authentication-api-openapi.yml
- filename: scalekit-connected-accounts-api-openapi.yml
  format: yaml
  label: Scalekit Connected Accounts API
  slug: scalekit-connected-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-connected-accounts-api-openapi.yml
- filename: scalekit-connections-api-openapi.yml
  format: yaml
  label: Scalekit Connections API
  slug: scalekit-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-connections-api-openapi.yml
- filename: scalekit-directories-api-openapi.yml
  format: yaml
  label: Scalekit Directories API
  slug: scalekit-directories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-directories-api-openapi.yml
- filename: scalekit-organization-settings-api-openapi.yml
  format: yaml
  label: Scalekit Organization Settings API
  slug: scalekit-organization-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-organization-settings-api-openapi.yml
- filename: scalekit-organizations-api-openapi.yml
  format: yaml
  label: Scalekit Organizations API
  slug: scalekit-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-organizations-api-openapi.yml
- filename: scalekit-roles-api-openapi.yml
  format: yaml
  label: Scalekit Roles API
  slug: scalekit-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-roles-api-openapi.yml
- filename: scalekit-users-memberships-api-openapi.yml
  format: yaml
  label: Scalekit Users & Memberships API
  slug: scalekit-users-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/openapi/scalekit-users-memberships-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Scalekit Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Scalekit secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Scalekit
provider_slug: scalekit
scheme_count: 2
schemes:
- description: OAuth 2.0 client-credentials access token passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/scalekit-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{environment}.scalekit.com/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/scalekit-openapi.yml
  type: oauth2
slug: scalekit-authentication
source_filename: scalekit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalekit-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 client-credentials access token passed as a Bearer token.\n  sources:\n  - openapi/scalekit-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}.scalekit.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/scalekit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalekit/refs/heads/main/authentication/scalekit-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Authentication
- SSO
- SCIM
- Identity
- B2B SaaS
- Agent Auth
---
