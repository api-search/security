---
api_key_in:
- header
api_specs:
- filename: brave-browser-images-api-openapi.yml
  format: yaml
  label: Brave Images API
  slug: brave-browser-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-images-api-openapi.yml
- filename: brave-browser-local-api-openapi.yml
  format: yaml
  label: Brave Local API
  slug: brave-browser-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-local-api-openapi.yml
- filename: brave-browser-news-api-openapi.yml
  format: yaml
  label: Brave News API
  slug: brave-browser-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-news-api-openapi.yml
- filename: brave-browser-spellcheck-api-openapi.yml
  format: yaml
  label: Brave Spellcheck API
  slug: brave-browser-spellcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-spellcheck-api-openapi.yml
- filename: brave-browser-suggest-api-openapi.yml
  format: yaml
  label: Brave Suggest API
  slug: brave-browser-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-suggest-api-openapi.yml
- filename: brave-browser-summarizer-api-openapi.yml
  format: yaml
  label: Brave Summarizer API
  slug: brave-browser-summarizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-summarizer-api-openapi.yml
- filename: brave-browser-videos-api-openapi.yml
  format: yaml
  label: Brave Videos API
  slug: brave-browser-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-videos-api-openapi.yml
- filename: brave-browser-web-api-openapi.yml
  format: yaml
  label: Brave Web API
  slug: brave-browser-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-web-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Brave Browser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brave secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brave
provider_slug: brave-browser
scheme_count: 1
schemes:
- in: header
  name: SubscriptionToken
  parameter: X-Subscription-Token
  sources:
  - openapi/brave-browser-openapi.yml
  type: apiKey
slug: brave-browser-authentication
source_filename: brave-browser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brave-browser-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SubscriptionToken\n  type: apiKey\n  in: header\n  parameter: X-Subscription-Token\n  sources:\n  - openapi/brave-browser-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/authentication/brave-browser-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Browser
- Search
- Privacy
- Chromium
- Web3
- AI
- Advertising
---
