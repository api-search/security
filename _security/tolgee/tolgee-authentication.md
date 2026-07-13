---
api_key_in:
- header
api_specs:
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Projects API
  slug: projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Keys API
  slug: keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Translations API
  slug: translations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Languages API
  slug: languages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Import/Export API
  slug: import-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Screenshots API
  slug: screenshots
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tolgee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tolgee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tolgee
provider_slug: tolgee
scheme_count: 1
schemes:
- description: Project API key prefixed with `tgpak_`. Scoped to a single project.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/tolgee-openapi.yml
  type: apiKey
slug: tolgee-authentication
source_filename: tolgee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tolgee-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Project API key prefixed with `tgpak_`. Scoped to a single project.\n  sources:\n  - openapi/tolgee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/authentication/tolgee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Localization
- i18n
- Translation
- Open Source
- Developer Tools
---
