---
api_key_in: []
api_specs:
- filename: ory-corp-billing-api-openapi.yml
  format: yaml
  label: Ory Billing API
  slug: ory-corp-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-billing-api-openapi.yml
- filename: ory-corp-courier-api-openapi.yml
  format: yaml
  label: Ory Courier API
  slug: ory-corp-courier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-courier-api-openapi.yml
- filename: ory-corp-event-streams-api-openapi.yml
  format: yaml
  label: Ory Event Streams API
  slug: ory-corp-event-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-event-streams-api-openapi.yml
- filename: ory-corp-identity-admin-api-openapi.yml
  format: yaml
  label: Ory Identity (Admin) API
  slug: ory-corp-identity-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-identity-admin-api-openapi.yml
- filename: ory-corp-identity-self-service-api-openapi.yml
  format: yaml
  label: Ory Identity (Self-Service) API
  slug: ory-corp-identity-self-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-identity-self-service-api-openapi.yml
- filename: ory-corp-oauth2-admin-api-openapi.yml
  format: yaml
  label: Ory OAuth2 (Admin) API
  slug: ory-corp-oauth2-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-oauth2-admin-api-openapi.yml
- filename: ory-corp-oauth2-public-api-openapi.yml
  format: yaml
  label: Ory OAuth2 (Public) API
  slug: ory-corp-oauth2-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-oauth2-public-api-openapi.yml
- filename: ory-corp-organizations-api-openapi.yml
  format: yaml
  label: Ory Organizations API
  slug: ory-corp-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-organizations-api-openapi.yml
- filename: ory-corp-permissions-api-openapi.yml
  format: yaml
  label: Ory Permissions API
  slug: ory-corp-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-permissions-api-openapi.yml
- filename: ory-corp-project-tokens-api-openapi.yml
  format: yaml
  label: Ory Project Tokens API
  slug: ory-corp-project-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-project-tokens-api-openapi.yml
- filename: ory-corp-projects-api-openapi.yml
  format: yaml
  label: Ory Projects API
  slug: ory-corp-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-projects-api-openapi.yml
- filename: ory-corp-relationships-api-openapi.yml
  format: yaml
  label: Ory Relationships API
  slug: ory-corp-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/openapi/ory-corp-relationships-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ory Corp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ory secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ory
provider_slug: ory-corp
scheme_count: 1
schemes:
- description: 'Ory API key. Project admin endpoints use an Ory project API key (ory_pat_...); Console endpoints use a workspace API key (ory_wak_...). Passed as `Authorization: Bearer <token>`.'
  name: oryApiKey
  scheme: bearer
  sources:
  - openapi/ory-corp-openapi.yml
  type: http
slug: ory-corp-authentication
source_filename: ory-corp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ory-corp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: oryApiKey\n  type: http\n  scheme: bearer\n  description: 'Ory API key. Project admin endpoints use an Ory project API key (ory_pat_...);\n    Console endpoints use a workspace API key (ory_wak_...). Passed as `Authorization: Bearer\n    <token>`.'\n  sources:\n  - openapi/ory-corp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/authentication/ory-corp-authentication.yml
summary_line: http · 1 scheme
tags:
- Identity
- Authentication
- OAuth2
- OpenID Connect
- Authorization
- Permissions
- IAM
- Open Source
---
