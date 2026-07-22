---
api_key_in:
- header
api_specs:
- filename: materials-zone-openapi.json
  format: json
  label: Materials Zone API
  slug: materials-zone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/openapi/materials-zone-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Materials Zone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Materials Zone secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Materials Zone
provider_slug: materials-zone
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: Authorization
  sources:
  - openapi/materials-zone-openapi.json
  type: apiKey
slug: materials-zone-authentication
source_filename: materials-zone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/materials-zone-openapi.json\ndocs: https://developer.materials.zone/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Each user within the organization requests a private API key. The key is passed\n  in the `authorization` request header on every call (e.g. `--header 'authorization: <api-key>'`).\n  API keys can be rotated on request at any frequency and provide an audit trail. Data is\n  segregated per organization and encrypted in transit and at rest. No OAuth2/OIDC surface.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/materials-zone-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materials-zone/refs/heads/main/authentication/materials-zone-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Materials Informatics
- Materials Science
- Research and Development
- Laboratory Data
- Data Management
- Life Sciences
---
