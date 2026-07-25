---
api_key_in:
- header
api_specs:
- filename: university-of-vienna-datastream-api-openapi.yml
  format: yaml
  label: University of Vienna datastream API
  slug: university-of-vienna-datastream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-datastream-api-openapi.yml
- filename: university-of-vienna-directory-api-openapi.yml
  format: yaml
  label: University of Vienna directory API
  slug: university-of-vienna-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-directory-api-openapi.yml
- filename: university-of-vienna-imageserver-api-openapi.yml
  format: yaml
  label: University of Vienna imageserver API
  slug: university-of-vienna-imageserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-imageserver-api-openapi.yml
- filename: university-of-vienna-lists-api-openapi.yml
  format: yaml
  label: University of Vienna lists API
  slug: university-of-vienna-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-lists-api-openapi.yml
- filename: university-of-vienna-misc-api-openapi.yml
  format: yaml
  label: University of Vienna misc API
  slug: university-of-vienna-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-misc-api-openapi.yml
- filename: university-of-vienna-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Vienna oai-pmh API
  slug: university-of-vienna-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-oai-pmh-api-openapi.yml
- filename: university-of-vienna-object-advanced-api-openapi.yml
  format: yaml
  label: University of Vienna object-advanced API
  slug: university-of-vienna-object-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-object-advanced-api-openapi.yml
- filename: university-of-vienna-object-basics-api-openapi.yml
  format: yaml
  label: University of Vienna object-basics API
  slug: university-of-vienna-object-basics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-object-basics-api-openapi.yml
- filename: university-of-vienna-relationships-api-openapi.yml
  format: yaml
  label: University of Vienna relationships API
  slug: university-of-vienna-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-relationships-api-openapi.yml
- filename: university-of-vienna-search-api-openapi.yml
  format: yaml
  label: University of Vienna search API
  slug: university-of-vienna-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-search-api-openapi.yml
- filename: university-of-vienna-session-api-openapi.yml
  format: yaml
  label: University of Vienna session API
  slug: university-of-vienna-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-session-api-openapi.yml
- filename: university-of-vienna-stats-api-openapi.yml
  format: yaml
  label: University of Vienna stats API
  slug: university-of-vienna-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-stats-api-openapi.yml
- filename: university-of-vienna-templates-api-openapi.yml
  format: yaml
  label: University of Vienna templates API
  slug: university-of-vienna-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-templates-api-openapi.yml
- filename: university-of-vienna-vocabularies-api-openapi.yml
  format: yaml
  label: University of Vienna vocabularies API
  slug: university-of-vienna-vocabularies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-vocabularies-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Vienna Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Vienna secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Vienna
provider_slug: university-of-vienna
scheme_count: 2
schemes:
- in: header
  name: tokenAuth
  parameter: X-XSRF-TOKEN
  sources:
  - openapi/university-of-vienna-phaidra-api.yaml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/university-of-vienna-phaidra-api.yaml
  type: http
slug: university-of-vienna-authentication
source_filename: university-of-vienna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-vienna-phaidra-api.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-XSRF-TOKEN\n  sources:\n  - openapi/university-of-vienna-phaidra-api.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/university-of-vienna-phaidra-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/authentication/university-of-vienna-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Higher Education
- University
- Research
- Repository
- Open Data
- Austria
- Europe
---
