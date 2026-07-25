---
api_key_in:
- header
api_specs:
- filename: nuclino-collections-api-openapi.yml
  format: yaml
  label: Nuclino Collections API
  slug: nuclino-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/openapi/nuclino-collections-api-openapi.yml
- filename: nuclino-files-api-openapi.yml
  format: yaml
  label: Nuclino Files API
  slug: nuclino-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/openapi/nuclino-files-api-openapi.yml
- filename: nuclino-items-api-openapi.yml
  format: yaml
  label: Nuclino Items API
  slug: nuclino-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/openapi/nuclino-items-api-openapi.yml
- filename: nuclino-teams-api-openapi.yml
  format: yaml
  label: Nuclino Teams API
  slug: nuclino-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/openapi/nuclino-teams-api-openapi.yml
- filename: nuclino-users-api-openapi.yml
  format: yaml
  label: Nuclino Users API
  slug: nuclino-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/openapi/nuclino-users-api-openapi.yml
- filename: nuclino-workspaces-api-openapi.yml
  format: yaml
  label: Nuclino Workspaces API
  slug: nuclino-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/openapi/nuclino-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nuclino Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuclino secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nuclino
provider_slug: nuclino
scheme_count: 1
schemes:
- description: API key authentication. Pass your API key in the Authorization header.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/nuclino-openapi.json
  type: apiKey
slug: nuclino-authentication
source_filename: nuclino-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nuclino-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication. Pass your API key in the Authorization header.\n  sources:\n  - openapi/nuclino-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuclino/refs/heads/main/authentication/nuclino-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Knowledge Management
- Team Workspace
- Documentation
- Wiki
- Collaboration
- Project Management
- REST API
---
