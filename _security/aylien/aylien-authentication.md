---
api_key_in:
- header
api_specs:
- filename: apis
  format: yaml
  label: AYLIEN News API
  slug: news-api
  spec_type: OpenAPI
  url: https://github.com/AYLIEN/apis
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
