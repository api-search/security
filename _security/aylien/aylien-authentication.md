---
api_key_in:
- header
api_specs:
- filename: aylien-absa-api-openapi.yml
  format: yaml
  label: AYLIEN Absa API
  slug: aylien-absa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-absa-api-openapi.yml
- filename: aylien-autocomplete-api-openapi.yml
  format: yaml
  label: AYLIEN autocomplete API
  slug: aylien-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-autocomplete-api-openapi.yml
- filename: aylien-classify-api-openapi.yml
  format: yaml
  label: AYLIEN Classify API
  slug: aylien-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-classify-api-openapi.yml
- filename: aylien-cluster-api-openapi.yml
  format: yaml
  label: AYLIEN cluster API
  slug: aylien-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-cluster-api-openapi.yml
- filename: aylien-concepts-api-openapi.yml
  format: yaml
  label: AYLIEN Concepts API
  slug: aylien-concepts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-concepts-api-openapi.yml
- filename: aylien-elsa-api-openapi.yml
  format: yaml
  label: AYLIEN Elsa API
  slug: aylien-elsa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-elsa-api-openapi.yml
- filename: aylien-entities-api-openapi.yml
  format: yaml
  label: AYLIEN Entities API
  slug: aylien-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-entities-api-openapi.yml
- filename: aylien-extract-api-openapi.yml
  format: yaml
  label: AYLIEN Extract API
  slug: aylien-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-extract-api-openapi.yml
- filename: aylien-hashtags-api-openapi.yml
  format: yaml
  label: AYLIEN Hashtags API
  slug: aylien-hashtags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-hashtags-api-openapi.yml
- filename: aylien-histogram-api-openapi.yml
  format: yaml
  label: AYLIEN histogram API
  slug: aylien-histogram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-histogram-api-openapi.yml
- filename: aylien-language-api-openapi.yml
  format: yaml
  label: AYLIEN Language API
  slug: aylien-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-language-api-openapi.yml
- filename: aylien-related-story-api-openapi.yml
  format: yaml
  label: AYLIEN related_story API
  slug: aylien-related-story-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-related-story-api-openapi.yml
- filename: aylien-sentiment-api-openapi.yml
  format: yaml
  label: AYLIEN Sentiment API
  slug: aylien-sentiment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-sentiment-api-openapi.yml
- filename: aylien-story-api-openapi.yml
  format: yaml
  label: AYLIEN story API
  slug: aylien-story-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-story-api-openapi.yml
- filename: aylien-summarize-api-openapi.yml
  format: yaml
  label: AYLIEN Summarize API
  slug: aylien-summarize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-summarize-api-openapi.yml
- filename: aylien-time-series-api-openapi.yml
  format: yaml
  label: AYLIEN time_series API
  slug: aylien-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-time-series-api-openapi.yml
- filename: aylien-trends-api-openapi.yml
  format: yaml
  label: AYLIEN trends API
  slug: aylien-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-trends-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aylien Authentication
name_suffix: Authentication
oauth_flows: []
overview: AYLIEN secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AYLIEN
provider_slug: aylien
scheme_count: 4
schemes:
- description: X-AYLIEN-NewsAPI-Application-ID is the identifier of your server, script, or program with a specific application. This parameter is required if you are accessing APIs without authenticating.
  in: header
  name: app_id
  parameter: X-AYLIEN-NewsAPI-Application-ID
  sources:
  - openapi/news-api.yaml
  type: apiKey
- description: X-AYLIEN-NewsAPI-Application-Key is the secret key of your server, script, or program with a specific application. This parameter is required if you are accessing APIs without authenticating.
  in: header
  name: app_key
  parameter: X-AYLIEN-NewsAPI-Application-Key
  sources:
  - openapi/news-api.yaml
  type: apiKey
- description: X-AYLIEN-TextAPI-Application-ID is the identifier of your server, script, or program with a specific application. This parameter is required if you are accessing APIs without authenticating.
  in: header
  name: app_id
  parameter: X-AYLIEN-TextAPI-Application-ID
  sources:
  - openapi/text-api.yaml
  type: apiKey
- description: X-AYLIEN-TextAPI-Application-Key is the secret key of your server, script, or program with a specific application. This parameter is required if you are accessing APIs without authenticating.
  in: header
  name: app_key
  parameter: X-AYLIEN-TextAPI-Application-Key
  sources:
  - openapi/text-api.yaml
  type: apiKey
slug: aylien-authentication
source_filename: aylien-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/news-api.yaml, openapi/text-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: app_id\n  type: apiKey\n  in: header\n  parameter: X-AYLIEN-NewsAPI-Application-ID\n  description: X-AYLIEN-NewsAPI-Application-ID is the identifier of your server, script, or\n    program with a specific application. This parameter is required if you are accessing APIs\n    without authenticating.\n  sources:\n  - openapi/news-api.yaml\n- name: app_key\n  type: apiKey\n  in: header\n  parameter: X-AYLIEN-NewsAPI-Application-Key\n  description: X-AYLIEN-NewsAPI-Application-Key is the secret key of your server, script, or\n    program with a specific application. This parameter is required if you are accessing APIs\n    without authenticating.\n  sources:\n  - openapi/news-api.yaml\n- name: app_id\n  type: apiKey\n  in: header\n  parameter: X-AYLIEN-TextAPI-Application-ID\n  description: X-AYLIEN-TextAPI-Application-ID\
  \ is the identifier of your server, script, or\n    program with a specific application. This parameter is required if you are accessing APIs\n    without authenticating.\n  sources:\n  - openapi/text-api.yaml\n- name: app_key\n  type: apiKey\n  in: header\n  parameter: X-AYLIEN-TextAPI-Application-Key\n  description: X-AYLIEN-TextAPI-Application-Key is the secret key of your server, script, or\n    program with a specific application. This parameter is required if you are accessing APIs\n    without authenticating.\n  sources:\n  - openapi/text-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/authentication/aylien-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- News Intelligence
- Text Analysis
- NLP
- Sentiment Analysis
- Entity Recognition
- Natural Language Processing
- News API
- Article Extraction
- Summarization
- Concept Detection
---
