---
api_key_in:
- header
api_specs:
- filename: university-of-padua-datastream-api-openapi.yml
  format: yaml
  label: University of Padua datastream API
  slug: university-of-padua-datastream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-datastream-api-openapi.yml
- filename: university-of-padua-directory-api-openapi.yml
  format: yaml
  label: University of Padua directory API
  slug: university-of-padua-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-directory-api-openapi.yml
- filename: university-of-padua-imageserver-api-openapi.yml
  format: yaml
  label: University of Padua imageserver API
  slug: university-of-padua-imageserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-imageserver-api-openapi.yml
- filename: university-of-padua-lists-api-openapi.yml
  format: yaml
  label: University of Padua lists API
  slug: university-of-padua-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-lists-api-openapi.yml
- filename: university-of-padua-misc-api-openapi.yml
  format: yaml
  label: University of Padua misc API
  slug: university-of-padua-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-misc-api-openapi.yml
- filename: university-of-padua-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Padua oai-pmh API
  slug: university-of-padua-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-oai-pmh-api-openapi.yml
- filename: university-of-padua-object-advanced-api-openapi.yml
  format: yaml
  label: University of Padua object-advanced API
  slug: university-of-padua-object-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-object-advanced-api-openapi.yml
- filename: university-of-padua-object-basics-api-openapi.yml
  format: yaml
  label: University of Padua object-basics API
  slug: university-of-padua-object-basics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-object-basics-api-openapi.yml
- filename: university-of-padua-relationships-api-openapi.yml
  format: yaml
  label: University of Padua relationships API
  slug: university-of-padua-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-relationships-api-openapi.yml
- filename: university-of-padua-search-api-openapi.yml
  format: yaml
  label: University of Padua search API
  slug: university-of-padua-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-search-api-openapi.yml
- filename: university-of-padua-session-api-openapi.yml
  format: yaml
  label: University of Padua session API
  slug: university-of-padua-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-session-api-openapi.yml
- filename: university-of-padua-stats-api-openapi.yml
  format: yaml
  label: University of Padua stats API
  slug: university-of-padua-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-stats-api-openapi.yml
- filename: university-of-padua-templates-api-openapi.yml
  format: yaml
  label: University of Padua templates API
  slug: university-of-padua-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-templates-api-openapi.yml
- filename: university-of-padua-vocabularies-api-openapi.yml
  format: yaml
  label: University of Padua vocabularies API
  slug: university-of-padua-vocabularies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-vocabularies-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Padua Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Padua secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Padua
provider_slug: university-of-padua
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/university-of-padua-phaidra.yaml
  type: http
- in: header
  name: tokenAuth
  parameter: X-XSRF-TOKEN
  sources:
  - openapi/university-of-padua-phaidra.yaml
  type: apiKey
slug: university-of-padua-authentication
source_filename: university-of-padua-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-padua-phaidra.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/university-of-padua-phaidra.yaml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: X-XSRF-TOKEN\n  sources:\n  - openapi/university-of-padua-phaidra.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/authentication/university-of-padua-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Higher Education
- University
- Open Data
- Research Data
- Library
- Repository
- Italy
---
