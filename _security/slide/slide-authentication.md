---
api_key_in: []
api_specs:
- filename: slide-accounts-api-openapi.yml
  format: yaml
  label: Slide Accounts API
  slug: slide-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-accounts-api-openapi.yml
- filename: slide-agents-api-openapi.yml
  format: yaml
  label: Slide Agents API
  slug: slide-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-agents-api-openapi.yml
- filename: slide-alerts-api-openapi.yml
  format: yaml
  label: Slide Alerts API
  slug: slide-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-alerts-api-openapi.yml
- filename: slide-audits-api-openapi.yml
  format: yaml
  label: Slide Audits API
  slug: slide-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-audits-api-openapi.yml
- filename: slide-backups-api-openapi.yml
  format: yaml
  label: Slide Backups API
  slug: slide-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-backups-api-openapi.yml
- filename: slide-clients-api-openapi.yml
  format: yaml
  label: Slide Clients API
  slug: slide-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-clients-api-openapi.yml
- filename: slide-devices-api-openapi.yml
  format: yaml
  label: Slide Devices API
  slug: slide-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-devices-api-openapi.yml
- filename: slide-networks-api-openapi.yml
  format: yaml
  label: Slide Networks API
  slug: slide-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-networks-api-openapi.yml
- filename: slide-restores-file-api-openapi.yml
  format: yaml
  label: Slide Restores (File) API
  slug: slide-restores-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-restores-file-api-openapi.yml
- filename: slide-restores-image-api-openapi.yml
  format: yaml
  label: Slide Restores (Image) API
  slug: slide-restores-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-restores-image-api-openapi.yml
- filename: slide-restores-push-api-openapi.yml
  format: yaml
  label: Slide Restores (Push) API
  slug: slide-restores-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-restores-push-api-openapi.yml
- filename: slide-restores-virtual-machine-api-openapi.yml
  format: yaml
  label: Slide Restores (Virtual Machine) API
  slug: slide-restores-virtual-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-restores-virtual-machine-api-openapi.yml
- filename: slide-snapshots-api-openapi.yml
  format: yaml
  label: Slide Snapshots API
  slug: slide-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-snapshots-api-openapi.yml
- filename: slide-users-api-openapi.yml
  format: yaml
  label: Slide Users API
  slug: slide-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/openapi/slide-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Slide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slide secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Slide
provider_slug: slide
scheme_count: 1
schemes:
- bearerFormat: string
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/slide-openapi-original.json
  token_source: Slide Console (user-scoped API tokens)
  type: http
slug: slide-authentication
source_filename: slide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/slide-openapi-original.json\ndocs: https://docs.slide.tech/api/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Slide authenticates every request with a static Bearer API token supplied in\n  the Authorization header (Authorization: Bearer YOUR_SECRET_TOKEN). Tokens are\n  created and managed in the Slide Console; they are user-based and inherit the\n  role and permissions of the user that created them. There is no OAuth flow and\n  no scope system.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: string\n  token_source: Slide Console (user-scoped API tokens)\n  sources:\n  - openapi/slide-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slide/refs/heads/main/authentication/slide-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Backup
- Disaster Recovery
- Business Continuity
- BCDR
- Managed Service Providers
- MSP
- Data Protection
- Cloud Storage
- Virtualization
---
