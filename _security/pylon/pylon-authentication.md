---
api_key_in: []
api_specs:
- filename: pylon-accounts-api-openapi.yml
  format: yaml
  label: Pylon Accounts API
  slug: pylon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-accounts-api-openapi.yml
- filename: pylon-contacts-api-openapi.yml
  format: yaml
  label: Pylon Contacts API
  slug: pylon-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-contacts-api-openapi.yml
- filename: pylon-custom-fields-api-openapi.yml
  format: yaml
  label: Pylon Custom Fields API
  slug: pylon-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-custom-fields-api-openapi.yml
- filename: pylon-issues-api-openapi.yml
  format: yaml
  label: Pylon Issues API
  slug: pylon-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-issues-api-openapi.yml
- filename: pylon-knowledge-base-api-openapi.yml
  format: yaml
  label: Pylon Knowledge Base API
  slug: pylon-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-knowledge-base-api-openapi.yml
- filename: pylon-tags-api-openapi.yml
  format: yaml
  label: Pylon Tags API
  slug: pylon-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-tags-api-openapi.yml
- filename: pylon-tasks-api-openapi.yml
  format: yaml
  label: Pylon Tasks API
  slug: pylon-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-tasks-api-openapi.yml
- filename: pylon-teams-api-openapi.yml
  format: yaml
  label: Pylon Teams API
  slug: pylon-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-teams-api-openapi.yml
- filename: pylon-users-api-openapi.yml
  format: yaml
  label: Pylon Users API
  slug: pylon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pylon/refs/heads/main/openapi/pylon-users-api-openapi.yml
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
- Customer-Support
- Customer Operations
- Ticketing
- Knowledge Base
- B2B
- Help Desk
---
