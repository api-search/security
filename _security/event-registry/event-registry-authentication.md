---
api_key_in:
- query
api_specs:
- filename: event-registry-articles-api-openapi.yml
  format: yaml
  label: Event Registry Articles API
  slug: event-registry-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-articles-api-openapi.yml
- filename: event-registry-events-api-openapi.yml
  format: yaml
  label: Event Registry Events API
  slug: event-registry-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-events-api-openapi.yml
- filename: event-registry-suggest-api-openapi.yml
  format: yaml
  label: Event Registry Suggest API
  slug: event-registry-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-suggest-api-openapi.yml
- filename: event-registry-topic-pages-api-openapi.yml
  format: yaml
  label: Event Registry Topic Pages API
  slug: event-registry-topic-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-topic-pages-api-openapi.yml
- filename: event-registry-usage-api-openapi.yml
  format: yaml
  label: Event Registry Usage API
  slug: event-registry-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/openapi/event-registry-usage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Event Registry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Event Registry secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Event Registry
provider_slug: event-registry
scheme_count: 1
schemes:
- description: API key obtained from newsapi.ai/register. Include as a field in the JSON POST body or as a query parameter named apiKey.
  in: query
  name: apiKeyAuth
  parameter: apiKey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: event-registry-authentication
source_filename: event-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key obtained from newsapi.ai/register. Include as a field in the JSON POST\n    body or as a query parameter named apiKey.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/authentication/event-registry-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- Media Monitoring
- News Intelligence
- Event Detection
- Named Entity Recognition
- Sentiment Analysis
- Media Analytics
- News API
---
