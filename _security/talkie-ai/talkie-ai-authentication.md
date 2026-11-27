---
anonymous_access: false
api_key_in: []
api_specs:
- filename: talkie-ai-calls-api-openapi.yml
  format: yaml
  label: Talkie.ai Calls API
  slug: talkie-ai-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talkie-ai/openapi/talkie-ai-calls-api-openapi.yml
- filename: talkie-ai-contacts-api-openapi.yml
  format: yaml
  label: Talkie.ai Contacts API
  slug: talkie-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talkie-ai/openapi/talkie-ai-contacts-api-openapi.yml
- filename: talkie-ai-data-collection-api-openapi.yml
  format: yaml
  label: Talkie.ai Data Collection API
  slug: talkie-ai-data-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talkie-ai/openapi/talkie-ai-data-collection-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Talkie.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talkie.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Talkie.ai
provider_slug: talkie-ai
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/talkie-ai-openapi.yaml
  - openapi/talkie-analytics-public-api.yaml
  type: http
slug: talkie-ai-authentication
source_filename: talkie-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/talkie-ai-openapi.yaml, openapi/talkie-analytics-public-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/talkie-ai-openapi.yaml\n  - openapi/talkie-analytics-public-api.yaml\n"
source_yaml_url: https://artifacts.apis.io/talkie-ai/authentication/talkie-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Healthcare
- MedicalReceptionist
- HIPAA
---
