---
api_key_in:
- header
- query
api_specs:
- filename: knowledgeapi.yaml
  format: yaml
  label: Yext Knowledge API
  slug: yext-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/knowledgeapi.yaml
- filename: answersapi.yaml
  format: yaml
  label: Yext Answers API
  slug: yext-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/answersapi.yaml
- filename: chatapi.yaml
  format: yaml
  label: Yext Chat API
  slug: yext-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/chatapi.yaml
- filename: eventsapi.yaml
  format: yaml
  label: Yext Events API
  slug: yext-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/eventsapi.yaml
- filename: liveapi.yaml
  format: yaml
  label: Yext Live API
  slug: yext-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/liveapi.yaml
- filename: adminapi.yaml
  format: yaml
  label: Yext Admin API
  slug: yext-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/adminapi.yaml
- filename: publisherlistingsapi.yaml
  format: yaml
  label: Yext Publisher Listings API
  slug: yext-publisher-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/publisherlistingsapi.yaml
- filename: publishereclapi.yaml
  format: yaml
  label: Yext Publisher ECL API
  slug: yext-publisher-ecl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/publishereclapi.yaml
- filename: publishernotifyreviewapi.yaml
  format: yaml
  label: Yext Publisher Notify Review API
  slug: yext-publisher-notify-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/publishernotifyreviewapi.yaml
- filename: publishertrackingpixelapi.yaml
  format: yaml
  label: Yext Publisher Tracking Pixel API
  slug: yext-publisher-tracking-pixel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/publishertrackingpixelapi.yaml
- filename: webhooks.yaml
  format: yaml
  label: Yext Webhooks
  slug: yext-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/yext/openapi/main/yaml/webhooks.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yext Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yext secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yext
provider_slug: yext
scheme_count: 4
schemes:
- in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/yext-admin-api-openapi.yml
  - openapi/yext-answers-api-openapi.yml
  - openapi/yext-chat-api-openapi.yml
  - openapi/yext-knowledge-api-openapi.yml
  - openapi/yext-live-api-openapi.yml
  type: apiKey
- in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/yext-admin-api-openapi.yml
  - openapi/yext-answers-api-openapi.yml
  - openapi/yext-chat-api-openapi.yml
  - openapi/yext-knowledge-api-openapi.yml
  - openapi/yext-live-api-openapi.yml
  type: apiKey
- bearerFormat: api-key
  name: api-key
  scheme: KEY
  sources:
  - openapi/yext-events-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: jwt
  scheme: Bearer
  sources:
  - openapi/yext-events-api-openapi.yml
  type: http
slug: yext-authentication
source_filename: yext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yext-admin-api-openapi.yml, openapi/yext-answers-api-openapi.yml, openapi/yext-chat-api-openapi.yml,\n  openapi/yext-events-api-openapi.yml, openapi/yext-knowledge-api-openapi.yml, openapi/yext-live-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/yext-admin-api-openapi.yml\n  - openapi/yext-answers-api-openapi.yml\n  - openapi/yext-chat-api-openapi.yml\n  - openapi/yext-knowledge-api-openapi.yml\n  - openapi/yext-live-api-openapi.yml\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/yext-admin-api-openapi.yml\n  - openapi/yext-answers-api-openapi.yml\n  - openapi/yext-chat-api-openapi.yml\n  - openapi/yext-knowledge-api-openapi.yml\n  - openapi/yext-live-api-openapi.yml\n- name: api-key\n  type: http\n  scheme: KEY\n  bearerFormat:\
  \ api-key\n  sources:\n  - openapi/yext-events-api-openapi.yml\n- name: jwt\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/yext-events-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yext/refs/heads/main/authentication/yext-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Digital Presence
- Business Listings
- Location Data
- Reviews
- AI Search
- Knowledge Graph
---
