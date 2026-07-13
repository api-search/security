---
api_key_in:
- header
api_specs:
- filename: copper-developer-api-openapi.yml
  format: yaml
  label: Copper Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/openapi/copper-developer-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Copper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Copper secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Copper
provider_slug: copper
scheme_count: 3
schemes:
- description: API access token for the user
  in: header
  name: PWAccessToken
  parameter: X-PW-AccessToken
  sources:
  - openapi/copper-developer-api-openapi.yml
  type: apiKey
- description: Application identifier, set to 'developer_api'
  in: header
  name: PWApplication
  parameter: X-PW-Application
  sources:
  - openapi/copper-developer-api-openapi.yml
  type: apiKey
- description: Email address of the API token owner
  in: header
  name: PWUserEmail
  parameter: X-PW-UserEmail
  sources:
  - openapi/copper-developer-api-openapi.yml
  type: apiKey
slug: copper-authentication
source_filename: copper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/copper-developer-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PWAccessToken\n  type: apiKey\n  in: header\n  parameter: X-PW-AccessToken\n  description: API access token for the user\n  sources:\n  - openapi/copper-developer-api-openapi.yml\n- name: PWApplication\n  type: apiKey\n  in: header\n  parameter: X-PW-Application\n  description: Application identifier, set to 'developer_api'\n  sources:\n  - openapi/copper-developer-api-openapi.yml\n- name: PWUserEmail\n  type: apiKey\n  in: header\n  parameter: X-PW-UserEmail\n  description: Email address of the API token owner\n  sources:\n  - openapi/copper-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper/refs/heads/main/authentication/copper-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Activities
- Companies
- Contact Relationship Management
- Contacts
- CRM
- Customer Relationship Management
- Google Workspace
- Leads
- Opportunities
- People
- Projects
- Sales
- Tasks
---
