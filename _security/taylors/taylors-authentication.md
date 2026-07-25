---
api_key_in: []
api_specs:
- filename: taylors-checkouts-api-openapi.yml
  format: yaml
  label: Taylor's University checkouts API
  slug: taylors-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-checkouts-api-openapi.yml
- filename: taylors-holds-api-openapi.yml
  format: yaml
  label: Taylor's University holds API
  slug: taylors-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-holds-api-openapi.yml
- filename: taylors-item-types-api-openapi.yml
  format: yaml
  label: Taylor's University item_types API
  slug: taylors-item-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-item-types-api-openapi.yml
- filename: taylors-items-api-openapi.yml
  format: yaml
  label: Taylor's University items API
  slug: taylors-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-items-api-openapi.yml
- filename: taylors-libraries-api-openapi.yml
  format: yaml
  label: Taylor's University libraries API
  slug: taylors-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-libraries-api-openapi.yml
- filename: taylors-patrons-api-openapi.yml
  format: yaml
  label: Taylor's University patrons API
  slug: taylors-patrons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-patrons-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Taylors Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Taylor's University secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Taylor's University
provider_slug: taylors
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/taylors-library-rest.yaml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/taylors-library-rest.yaml
  type: oauth2
slug: taylors-authentication
source_filename: taylors-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/taylors-library-rest.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/taylors-library-rest.yaml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/taylors-library-rest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/authentication/taylors-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Education
- Higher Education
- University
- Library
- Institutional Repository
- Open Data
- Malaysia
- Asia
---
