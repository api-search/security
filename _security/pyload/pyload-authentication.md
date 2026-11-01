---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: pyload-pyload-rest-api-openapi.yml
  format: yaml
  label: pyLoad pyLoad REST API
  slug: pyload-pyload-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pyload/openapi/pyload-pyload-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Pyload Authentication
name_suffix: Authentication
oauth_flows: []
overview: pyLoad secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: pyLoad
provider_slug: pyload
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/pyload-android-openapi.json
  - openapi/pyload-openapi.json
  type: apiKey
slug: pyload-authentication
source_filename: pyload-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/pyload-android-openapi.json, openapi/pyload-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/pyload-android-openapi.json\n  - openapi/pyload-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/pyload/authentication/pyload-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Download Manager
- Open Source
- Python
- Automation
- File Transfer
---
