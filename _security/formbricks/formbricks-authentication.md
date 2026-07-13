---
api_key_in:
- header
api_specs:
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Surveys API
  slug: surveys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Responses API
  slug: responses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Contacts and Attributes API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Management API
  slug: management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Formbricks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formbricks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Formbricks
provider_slug: formbricks
scheme_count: 1
schemes:
- description: Personal API key generated in Formbricks under Settings > API Keys.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/formbricks-openapi.yml
  type: apiKey
slug: formbricks-authentication
source_filename: formbricks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formbricks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Personal API key generated in Formbricks under Settings > API Keys.\n  sources:\n  - openapi/formbricks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/authentication/formbricks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Surveys
- Experience Management
- Feedback
- Forms
- Open Source
---
