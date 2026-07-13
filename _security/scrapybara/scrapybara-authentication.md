---
api_key_in:
- header
api_specs:
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Instances API
  slug: scrapybara-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Computer Actions API
  slug: scrapybara-computer-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Browser API
  slug: scrapybara-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Code Execution API
  slug: scrapybara-code-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Filesystem API
  slug: scrapybara-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Notebook API
  slug: scrapybara-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Auth States API
  slug: scrapybara-auth-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Environment API
  slug: scrapybara-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scrapybara Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scrapybara secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scrapybara
provider_slug: scrapybara
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/scrapybara-openapi.yml
  type: apiKey
slug: scrapybara-authentication
source_filename: scrapybara-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scrapybara-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/scrapybara-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/authentication/scrapybara-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Agents
- Virtual Desktops
- Computer Use
- Browser Automation
- Code Execution
---
