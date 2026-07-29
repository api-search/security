---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: Rightsline Rights API
  slug: rights-api
  spec_type: Postman
  url: https://www.postman.com/kinlaneapi/rightsline/overview
- filename: postman.yaml
  format: yaml
  label: Rightsline Royalties API
  slug: royalties-api
  spec_type: Postman
  url: https://postman.rightsline.com/
- filename: rightsline-availability-api-openapi.yml
  format: yaml
  label: Rightsline Availability API
  slug: rightsline-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-availability-api-openapi.yml
- filename: rightsline-catalog-api-openapi.yml
  format: yaml
  label: Rightsline Catalog API
  slug: rightsline-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-catalog-api-openapi.yml
- filename: rightsline-contacts-api-openapi.yml
  format: yaml
  label: Rightsline Contacts API
  slug: rightsline-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-contacts-api-openapi.yml
- filename: rightsline-lists-api-openapi.yml
  format: yaml
  label: Rightsline Lists API
  slug: rightsline-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-lists-api-openapi.yml
- filename: rightsline-rights-api-openapi.yml
  format: yaml
  label: Rightsline Rights API
  slug: rightsline-rights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-rights-api-openapi.yml
- filename: rightsline-royalties-api-openapi.yml
  format: yaml
  label: Rightsline Royalties API
  slug: rightsline-royalties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-royalties-api-openapi.yml
- filename: rightsline-templates-api-openapi.yml
  format: yaml
  label: Rightsline Templates API
  slug: rightsline-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-templates-api-openapi.yml
- filename: rightsline-workflows-api-openapi.yml
  format: yaml
  label: Rightsline Workflows API
  slug: rightsline-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rightsline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rightsline secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rightsline
provider_slug: rightsline
scheme_count: 1
schemes:
- description: Bearer token obtained by exchanging Company API Key + Access Key + Secret Access Key. Generate credentials in app.rightsline.com Profile > API Access.
  in: header
  name: ApiKey
  parameter: Authorization
  sources:
  - openapi/rightsline-openapi.yml
  type: apiKey
slug: rightsline-authentication
source_filename: rightsline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rightsline-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer token obtained by exchanging Company API Key + Access Key + Secret Access\n    Key. Generate credentials in app.rightsline.com Profile > API Access.\n  sources:\n  - openapi/rightsline-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/authentication/rightsline-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Content Management
- Entertainment
- Media
- Rights Management
- Royalties
---
