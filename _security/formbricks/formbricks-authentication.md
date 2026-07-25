---
api_key_in:
- header
api_specs:
- filename: formbricks-action-classes-api-openapi.yml
  format: yaml
  label: Formbricks Action Classes API
  slug: formbricks-action-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-action-classes-api-openapi.yml
- filename: formbricks-client-api-openapi.yml
  format: yaml
  label: Formbricks Client API
  slug: formbricks-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-client-api-openapi.yml
- filename: formbricks-contacts-api-openapi.yml
  format: yaml
  label: Formbricks Contacts API
  slug: formbricks-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-contacts-api-openapi.yml
- filename: formbricks-me-api-openapi.yml
  format: yaml
  label: Formbricks Me API
  slug: formbricks-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-me-api-openapi.yml
- filename: formbricks-responses-api-openapi.yml
  format: yaml
  label: Formbricks Responses API
  slug: formbricks-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-responses-api-openapi.yml
- filename: formbricks-surveys-api-openapi.yml
  format: yaml
  label: Formbricks Surveys API
  slug: formbricks-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-surveys-api-openapi.yml
- filename: formbricks-webhooks-api-openapi.yml
  format: yaml
  label: Formbricks Webhooks API
  slug: formbricks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-webhooks-api-openapi.yml
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
