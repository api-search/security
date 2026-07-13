---
api_key_in: []
api_specs:
- filename: pylon-openapi.yml
  format: yaml
  label: Pylon Issues API
  slug: pylon-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-openapi.yml
- filename: pylon-openapi.yml
  format: yaml
  label: Pylon Accounts API
  slug: pylon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-openapi.yml
- filename: pylon-openapi.yml
  format: yaml
  label: Pylon Contacts API
  slug: pylon-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-openapi.yml
- filename: pylon-openapi.yml
  format: yaml
  label: Pylon Users and Teams API
  slug: pylon-users-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-openapi.yml
- filename: pylon-openapi.yml
  format: yaml
  label: Pylon Knowledge Base API
  slug: pylon-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-openapi.yml
- filename: pylon-openapi.yml
  format: yaml
  label: Pylon Tags and Custom Fields API
  slug: pylon-tags-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-openapi.yml
- filename: pylon-openapi.yml
  format: yaml
  label: Pylon Tasks and Projects API
  slug: pylon-tasks-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-openapi.yml
- filename: pylon-openapi.yml
  format: yaml
  label: Pylon Webhooks API
  slug: pylon-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pylon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pylon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pylon
provider_slug: pylon
scheme_count: 1
schemes:
- description: Pylon API token passed as a Bearer token in the Authorization header. Only Admin users can create API tokens in Pylon settings.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pylon-openapi.yml
  type: http
slug: pylon-authentication
source_filename: pylon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pylon-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Pylon API token passed as a Bearer token in the Authorization header. Only Admin\n    users can create API tokens in Pylon settings.\n  sources:\n  - openapi/pylon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/authentication/pylon-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Support
- Customer Operations
- Ticketing
- Knowledge Base
- B2B
- Help Desk
---
