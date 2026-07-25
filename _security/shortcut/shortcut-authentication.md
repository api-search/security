---
api_key_in:
- header
api_specs:
- filename: shortcut-categories-api-openapi.yml
  format: yaml
  label: Shortcut Categories API
  slug: shortcut-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-categories-api-openapi.yml
- filename: shortcut-custom-fields-api-openapi.yml
  format: yaml
  label: Shortcut Custom Fields API
  slug: shortcut-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-custom-fields-api-openapi.yml
- filename: shortcut-documents-api-openapi.yml
  format: yaml
  label: Shortcut Documents API
  slug: shortcut-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-documents-api-openapi.yml
- filename: shortcut-entity-templates-api-openapi.yml
  format: yaml
  label: Shortcut Entity Templates API
  slug: shortcut-entity-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-entity-templates-api-openapi.yml
- filename: shortcut-epics-api-openapi.yml
  format: yaml
  label: Shortcut Epics API
  slug: shortcut-epics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-epics-api-openapi.yml
- filename: shortcut-workflows-api-openapi.yml
  format: yaml
  label: Shortcut Workflows API
  slug: shortcut-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Shortcut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shortcut secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Shortcut
provider_slug: shortcut
scheme_count: 1
schemes:
- description: Personal API token generated at app.shortcut.com settings.
  in: header
  name: ShortcutToken
  parameter: Shortcut-Token
  sources:
  - openapi/shortcut-openapi.yml
  type: apiKey
slug: shortcut-authentication
source_filename: shortcut-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shortcut-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ShortcutToken\n  type: apiKey\n  in: header\n  parameter: Shortcut-Token\n  description: Personal API token generated at app.shortcut.com settings.\n  sources:\n  - openapi/shortcut-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/authentication/shortcut-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Project Management
- Agile
- Software Development
- Issue Tracking
- Kanban
- Sprint Planning
- Collaboration
- Developer Tools
---
