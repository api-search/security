---
api_key_in:
- header
api_specs:
- filename: rockwell-factorytalk-optix-openapi.yml
  format: yaml
  label: Rockwell FactoryTalk Optix REST API
  slug: factorytalk-optix-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockwell-factorytalk/refs/heads/main/openapi/rockwell-factorytalk-optix-openapi.yml
- filename: rockwell-factorytalk-realtime-asyncapi.yml
  format: yaml
  label: Rockwell FactoryTalk Hub API
  slug: factorytalk-hub-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockwell-factorytalk/refs/heads/main/asyncapi/rockwell-factorytalk-realtime-asyncapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Rockwell Factorytalk Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: rockwell-factorytalk secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: rockwell-factorytalk
provider_slug: rockwell-factorytalk
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://optix.example.com/auth/token
  name: oauth2
  sources:
  - openapi/rockwell-factorytalk-optix-openapi.yml
  type: oauth2
- description: FactoryTalk Optix API key
  in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/rockwell-factorytalk-optix-openapi.yml
  type: apiKey
slug: rockwell-factorytalk-authentication
source_filename: rockwell-factorytalk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rockwell-factorytalk-optix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://optix.example.com/auth/token\n    scopes: 3\n  sources:\n  - openapi/rockwell-factorytalk-optix-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: FactoryTalk Optix API key\n  sources:\n  - openapi/rockwell-factorytalk-optix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockwell-factorytalk/refs/heads/main/authentication/rockwell-factorytalk-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags: []
---
