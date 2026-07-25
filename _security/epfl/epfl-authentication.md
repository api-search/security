---
api_key_in:
- header
api_specs:
- filename: epfl-categories-api-openapi.yml
  format: yaml
  label: EPFL Categories API
  slug: epfl-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-categories-api-openapi.yml
- filename: epfl-channels-api-openapi.yml
  format: yaml
  label: EPFL Channels API
  slug: epfl-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-channels-api-openapi.yml
- filename: epfl-domains-api-openapi.yml
  format: yaml
  label: EPFL Domains API
  slug: epfl-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-domains-api-openapi.yml
- filename: epfl-events-api-openapi.yml
  format: yaml
  label: EPFL Events API
  slug: epfl-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-events-api-openapi.yml
- filename: epfl-faculties-api-openapi.yml
  format: yaml
  label: EPFL Faculties API
  slug: epfl-faculties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-faculties-api-openapi.yml
- filename: epfl-mementos-api-openapi.yml
  format: yaml
  label: EPFL Mementos API
  slug: epfl-mementos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-mementos-api-openapi.yml
- filename: epfl-news-api-openapi.yml
  format: yaml
  label: EPFL News API
  slug: epfl-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-news-api-openapi.yml
- filename: epfl-projects-api-openapi.yml
  format: yaml
  label: EPFL Projects API
  slug: epfl-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-projects-api-openapi.yml
- filename: epfl-publics-api-openapi.yml
  format: yaml
  label: EPFL Publics API
  slug: epfl-publics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-publics-api-openapi.yml
- filename: epfl-registrations-api-openapi.yml
  format: yaml
  label: EPFL Registrations API
  slug: epfl-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-registrations-api-openapi.yml
- filename: epfl-spoken-languages-api-openapi.yml
  format: yaml
  label: EPFL Spoken Languages API
  slug: epfl-spoken-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-spoken-languages-api-openapi.yml
- filename: epfl-themes-api-openapi.yml
  format: yaml
  label: EPFL Themes API
  slug: epfl-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-themes-api-openapi.yml
- filename: epfl-vulgarizations-api-openapi.yml
  format: yaml
  label: EPFL Vulgarizations API
  slug: epfl-vulgarizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-vulgarizations-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Epfl Authentication
name_suffix: Authentication
oauth_flows: []
overview: EPFL secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EPFL
provider_slug: epfl
scheme_count: 2
schemes:
- description: 'DRF Token authentication, e.g. "Authorization: Token <key>".'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/epfl-actu.yaml
  - openapi/epfl-memento.yaml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/epfl-actu.yaml
  - openapi/epfl-memento.yaml
  type: http
slug: epfl-authentication
source_filename: epfl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/epfl-actu.yaml, openapi/epfl-memento.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'DRF Token authentication, e.g. \"Authorization: Token <key>\".'\n  sources:\n  - openapi/epfl-actu.yaml\n  - openapi/epfl-memento.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/epfl-actu.yaml\n  - openapi/epfl-memento.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/authentication/epfl-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Switzerland
- Europe
---
