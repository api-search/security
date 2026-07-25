---
api_key_in:
- header
api_specs:
- filename: oneflow-comments-api-openapi.yml
  format: yaml
  label: Oneflow Comments API
  slug: oneflow-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-comments-api-openapi.yml
- filename: oneflow-contract-files-api-openapi.yml
  format: yaml
  label: Oneflow Contract Files API
  slug: oneflow-contract-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-contract-files-api-openapi.yml
- filename: oneflow-contracts-api-openapi.yml
  format: yaml
  label: Oneflow Contracts API
  slug: oneflow-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-contracts-api-openapi.yml
- filename: oneflow-data-fields-api-openapi.yml
  format: yaml
  label: Oneflow Data Fields API
  slug: oneflow-data-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-data-fields-api-openapi.yml
- filename: oneflow-participants-api-openapi.yml
  format: yaml
  label: Oneflow Participants API
  slug: oneflow-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-participants-api-openapi.yml
- filename: oneflow-parties-api-openapi.yml
  format: yaml
  label: Oneflow Parties API
  slug: oneflow-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-parties-api-openapi.yml
- filename: oneflow-ping-api-openapi.yml
  format: yaml
  label: Oneflow Ping API
  slug: oneflow-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-ping-api-openapi.yml
- filename: oneflow-templates-api-openapi.yml
  format: yaml
  label: Oneflow Templates API
  slug: oneflow-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-templates-api-openapi.yml
- filename: oneflow-users-api-openapi.yml
  format: yaml
  label: Oneflow Users API
  slug: oneflow-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-users-api-openapi.yml
- filename: oneflow-webhooks-api-openapi.yml
  format: yaml
  label: Oneflow Webhooks API
  slug: oneflow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-webhooks-api-openapi.yml
- filename: oneflow-workspaces-api-openapi.yml
  format: yaml
  label: Oneflow Workspaces API
  slug: oneflow-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oneflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oneflow secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oneflow
provider_slug: oneflow
scheme_count: 2
schemes:
- description: Account API token generated in the Oneflow Marketplace.
  in: header
  name: apiToken
  parameter: x-oneflow-api-token
  sources:
  - openapi/oneflow-openapi.yml
  type: apiKey
- description: Email of the acting Oneflow user, used for permission-scoped authorization. Optional on some endpoints; omitting it runs the request as an anonymous admin user.
  in: header
  name: userEmail
  parameter: x-oneflow-user-email
  sources:
  - openapi/oneflow-openapi.yml
  type: apiKey
slug: oneflow-authentication
source_filename: oneflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oneflow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: x-oneflow-api-token\n  description: Account API token generated in the Oneflow Marketplace.\n  sources:\n  - openapi/oneflow-openapi.yml\n- name: userEmail\n  type: apiKey\n  in: header\n  parameter: x-oneflow-user-email\n  description: Email of the acting Oneflow user, used for permission-scoped authorization. Optional\n    on some endpoints; omitting it runs the request as an anonymous admin user.\n  sources:\n  - openapi/oneflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/authentication/oneflow-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Contract Management
- Contract Lifecycle Management
- E-Signature
- Digital Contracts
- Document Automation
- CLM
---
