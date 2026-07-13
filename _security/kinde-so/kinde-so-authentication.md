---
api_key_in: []
api_specs:
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Users API
  slug: kinde-so-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Organizations API
  slug: kinde-so-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Roles API
  slug: kinde-so-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Permissions API
  slug: kinde-so-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Feature Flags API
  slug: kinde-so-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Applications API
  slug: kinde-so-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Connections API
  slug: kinde-so-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde APIs and Scopes API
  slug: kinde-so-apis-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Subscribers API
  slug: kinde-so-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Business API
  slug: kinde-so-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Properties API
  slug: kinde-so-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Webhooks API
  slug: kinde-so-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Billing API
  slug: kinde-so-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kinde So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kinde secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kinde
provider_slug: kinde-so
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Requires an access token obtained using the OAuth2 client_credentials flow from an authorized M2M application.
  name: kindeBearerAuth
  scheme: bearer
  sources:
  - openapi/kinde-so-openapi.yml
  type: http
slug: kinde-so-authentication
source_filename: kinde-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kinde-so-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: kindeBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Requires an access token obtained using the OAuth2 client_credentials flow from\n    an authorized M2M application.\n  sources:\n  - openapi/kinde-so-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/authentication/kinde-so-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- User Management
- Identity
- Authorization
- SaaS
- CIAM
---
