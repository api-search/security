---
api_key_in: []
api_specs:
- filename: hackmd-history-api-openapi.yml
  format: yaml
  label: HackMD History API
  slug: hackmd-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-history-api-openapi.yml
- filename: hackmd-profile-api-openapi.yml
  format: yaml
  label: HackMD Profile API
  slug: hackmd-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-profile-api-openapi.yml
- filename: hackmd-team-folders-api-openapi.yml
  format: yaml
  label: HackMD Team Folders API
  slug: hackmd-team-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-team-folders-api-openapi.yml
- filename: hackmd-team-notes-api-openapi.yml
  format: yaml
  label: HackMD Team Notes API
  slug: hackmd-team-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-team-notes-api-openapi.yml
- filename: hackmd-teams-api-openapi.yml
  format: yaml
  label: HackMD Teams API
  slug: hackmd-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-teams-api-openapi.yml
- filename: hackmd-trash-api-openapi.yml
  format: yaml
  label: HackMD Trash API
  slug: hackmd-trash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-trash-api-openapi.yml
- filename: hackmd-user-folders-api-openapi.yml
  format: yaml
  label: HackMD User Folders API
  slug: hackmd-user-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-user-folders-api-openapi.yml
- filename: hackmd-user-notes-api-openapi.yml
  format: yaml
  label: HackMD User Notes API
  slug: hackmd-user-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/openapi/hackmd-user-notes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hackmd Authentication
name_suffix: Authentication
oauth_flows: []
overview: HackMD secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HackMD
provider_slug: hackmd
scheme_count: 1
schemes:
- format: Bearer <API_ACCESS_TOKEN>
  header: Authorization
  issuance: Created under Settings > API in the HackMD web app; shown once at creation.
  name: token
  scheme: bearer
  scopes: none (token carries the full permissions of the issuing user/account)
  sources:
  - openapi/hackmd-openapi-original.json
  type: http
slug: hackmd-authentication
source_filename: hackmd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hackmd-openapi-original.json\ndocs: https://hackmd.io/@docs/api-authorization\ntoken_management: https://hackmd.io/@docs/how-to-issue-an-api-token\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  model: Personal API access token (bearer)\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer <API_ACCESS_TOKEN>'\n  issuance: Created under Settings > API in the HackMD web app; shown once at creation.\n  scopes: none (token carries the full permissions of the issuing user/account)\n  sources:\n  - openapi/hackmd-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hackmd/refs/heads/main/authentication/hackmd-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Markdown
- Collaboration
- Documentation
- Note Taking
- Knowledge Base
- Productivity
- Content
---
