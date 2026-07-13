---
api_key_in: []
api_specs:
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Import / Upload API
  slug: import-upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Export API
  slug: export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Languages API
  slug: languages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
- filename: localazy-openapi.yml
  format: yaml
  label: Localazy Projects (Management) API
  slug: projects-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/openapi/localazy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Localazy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Localazy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Localazy
provider_slug: localazy
scheme_count: 1
schemes:
- description: 'Authenticate with the header `Authorization: Bearer {token}`. Tokens may be a project token (read/write to one project), a translation token (AI translation only), or an organization token (organization scope, by request).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/localazy-openapi.yml
  type: http
slug: localazy-authentication
source_filename: localazy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/localazy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate with the header `Authorization: Bearer {token}`. Tokens may be\n    a project token (read/write to one project), a translation token (AI translation only),\n    or an organization token (organization scope, by request).'\n  sources:\n  - openapi/localazy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localazy/refs/heads/main/authentication/localazy-authentication.yml
summary_line: http · 1 scheme
tags:
- Localization
- Translation
- Internationalization
- i18n
- L10n
- Translation Management
---
