---
api_key_in:
- header
api_specs:
- filename: microsoft-bing-openapi.yml
  format: yaml
  label: Bing Web Search API
  slug: web-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Bing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft Bing secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft Bing
provider_slug: microsoft-bing
scheme_count: 1
schemes:
- in: header
  name: subscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/microsoft-bing-openapi.yml
  type: apiKey
slug: microsoft-bing-authentication
source_filename: microsoft-bing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-bing-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/microsoft-bing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/authentication/microsoft-bing-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Search
- Web Search
- Images
- Videos
- News
- Azure AI
- Autosuggest
- Visual Search
---
