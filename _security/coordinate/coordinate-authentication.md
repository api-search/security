---
api_key_in:
- header
api_specs:
- filename: coordinate-comments-api-openapi.yml
  format: yaml
  label: Coordinate Comments API
  slug: coordinate-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-comments-api-openapi.yml
- filename: coordinate-entity-api-openapi.yml
  format: yaml
  label: Coordinate Entity API
  slug: coordinate-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-entity-api-openapi.yml
- filename: coordinate-goals-api-openapi.yml
  format: yaml
  label: Coordinate Goals API
  slug: coordinate-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-goals-api-openapi.yml
- filename: coordinate-groups-api-openapi.yml
  format: yaml
  label: Coordinate Groups API
  slug: coordinate-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-groups-api-openapi.yml
- filename: coordinate-organizations-api-openapi.yml
  format: yaml
  label: Coordinate Organizations API
  slug: coordinate-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-organizations-api-openapi.yml
- filename: coordinate-progress-reports-api-openapi.yml
  format: yaml
  label: Coordinate Progress Reports API
  slug: coordinate-progress-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-progress-reports-api-openapi.yml
- filename: coordinate-project-pages-api-openapi.yml
  format: yaml
  label: Coordinate Project Pages API
  slug: coordinate-project-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-project-pages-api-openapi.yml
- filename: coordinate-projects-api-openapi.yml
  format: yaml
  label: Coordinate Projects API
  slug: coordinate-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-projects-api-openapi.yml
- filename: coordinate-stakeholders-api-openapi.yml
  format: yaml
  label: Coordinate Stakeholders API
  slug: coordinate-stakeholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-stakeholders-api-openapi.yml
- filename: coordinate-storage-api-openapi.yml
  format: yaml
  label: Coordinate Storage API
  slug: coordinate-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-storage-api-openapi.yml
- filename: coordinate-tasks-api-openapi.yml
  format: yaml
  label: Coordinate Tasks API
  slug: coordinate-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-tasks-api-openapi.yml
- filename: coordinate-users-api-openapi.yml
  format: yaml
  label: Coordinate Users API
  slug: coordinate-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-users-api-openapi.yml
- filename: coordinate-webhooks-api-openapi.yml
  format: yaml
  label: Coordinate Webhooks API
  slug: coordinate-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/openapi/coordinate-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coordinate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coordinate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coordinate
provider_slug: coordinate
scheme_count: 1
schemes:
- description: 'API key sent in a custom `Bearer:` header (note: this is a header named "Bearer", not the standard `Authorization: Bearer` scheme). Create keys in the Coordinate UI under Settings > Integrations > API Keys. The key scopes all requests to its owning vendor.'
  in: header
  name: BearerHeader
  parameter: Bearer
  sources:
  - openapi/coordinate-openapi.yml
  type: apiKey
slug: coordinate-authentication
source_filename: coordinate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/coordinate-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerHeader\n  type: apiKey\n  in: header\n  parameter: Bearer\n  description: 'API key sent in a custom `Bearer:` header (note: this is a header named \"Bearer\",\n    not the standard `Authorization: Bearer` scheme). Create keys in the Coordinate UI under\n    Settings > Integrations > API Keys. The key scopes all requests to its owning vendor.'\n  sources:\n  - openapi/coordinate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coordinate/refs/heads/main/authentication/coordinate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise Saas
- Project Management
- Client Portal
- Client Onboarding
- Professional Services
- Workflow-Automation
- Collaboration
- Webhook
---
