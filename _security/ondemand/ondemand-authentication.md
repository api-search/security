---
api_key_in:
- header
api_specs:
- filename: ondemand-openapi.json
  format: json
  label: OnDemand AI API
  slug: ondemand-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ondemand/refs/heads/main/openapi/ondemand-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ondemand Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ondemand secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ondemand
provider_slug: ondemand
scheme_count: 1
schemes:
- in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/ondemand-openapi.json
  type: apiKey
slug: ondemand-authentication
source_filename: ondemand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/ondemand-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/ondemand-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ondemand/refs/heads/main/authentication/ondemand-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- RAG
- Agents
- LLM
- Platform as a Service
- Chat
- Workflow Automation
- Vector Search
---
