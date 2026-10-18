---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: azuqua-account-api-openapi.yml
  format: yaml
  label: Azuqua Account API
  slug: azuqua-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-account-api-openapi.yml
- filename: azuqua-accounts-api-openapi.yml
  format: yaml
  label: Azuqua Accounts API
  slug: azuqua-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-accounts-api-openapi.yml
- filename: azuqua-connectors-api-openapi.yml
  format: yaml
  label: Azuqua Connectors API
  slug: azuqua-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-connectors-api-openapi.yml
- filename: azuqua-flo-api-openapi.yml
  format: yaml
  label: Azuqua Flo API
  slug: azuqua-flo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-flo-api-openapi.yml
- filename: azuqua-folder-api-openapi.yml
  format: yaml
  label: Azuqua Folder API
  slug: azuqua-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-folder-api-openapi.yml
- filename: azuqua-folders-api-openapi.yml
  format: yaml
  label: Azuqua Folders API
  slug: azuqua-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-folders-api-openapi.yml
- filename: azuqua-org-api-openapi.yml
  format: yaml
  label: Azuqua Org API
  slug: azuqua-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-org-api-openapi.yml
- filename: azuqua-user-api-openapi.yml
  format: yaml
  label: Azuqua User API
  slug: azuqua-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Azuqua Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azuqua secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Azuqua
provider_slug: azuqua
scheme_count: 3
schemes:
- in: header
  name: sec0
  parameter: x-api-accesskey
  sources:
  - openapi/azuqua-page-openapi.yml
  type: apiKey
- in: header
  name: sec1
  parameter: x-api-hash
  sources:
  - openapi/azuqua-page-openapi.yml
  type: apiKey
- in: header
  name: sec2
  parameter: x-api-timestamp
  sources:
  - openapi/azuqua-page-openapi.yml
  type: apiKey
slug: azuqua-authentication
source_filename: azuqua-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/azuqua-page-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-accesskey\n  sources:\n  - openapi/azuqua-page-openapi.yml\n- name: sec1\n  type: apiKey\n  in: header\n  parameter: x-api-hash\n  sources:\n  - openapi/azuqua-page-openapi.yml\n- name: sec2\n  type: apiKey\n  in: header\n  parameter: x-api-timestamp\n  sources:\n  - openapi/azuqua-page-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/authentication/azuqua-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Integration
- iPaaS
- Workflow Automation
- Integration Platform
- Automation
- Connectors
- No-Code
---
