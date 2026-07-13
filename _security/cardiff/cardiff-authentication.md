---
api_key_in: []
api_specs:
- filename: cardiff-courses.yaml
  format: yaml
  label: Courses
  slug: courses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-courses.yaml
- filename: cardiff-modules.yaml
  format: yaml
  label: Modules
  slug: modules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-modules.yaml
- filename: cardiff-lookups.yaml
  format: yaml
  label: Lookups
  slug: lookups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-lookups.yaml
- filename: cardiff-publications.yaml
  format: yaml
  label: Publications
  slug: publications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-publications.yaml
- filename: cardiff-echo.yaml
  format: yaml
  label: EchoTest
  slug: echo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-echo.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cardiff Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Cardiff University secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Cardiff University
provider_slug: cardiff
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.data.cardiff.ac.uk/authorize
    flow: implicit
    scopes: 1
  name: default
  sources:
  - openapi/cardiff-courses.yaml
  - openapi/cardiff-echo.yaml
  - openapi/cardiff-lookups.yaml
  - openapi/cardiff-modules.yaml
  - openapi/cardiff-publications.yaml
  type: oauth2
slug: cardiff-authentication
source_filename: cardiff-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cardiff-courses.yaml, openapi/cardiff-echo.yaml, openapi/cardiff-lookups.yaml,\n  openapi/cardiff-modules.yaml, openapi/cardiff-publications.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: default\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.data.cardiff.ac.uk/authorize\n    scopes: 1\n  sources:\n  - openapi/cardiff-courses.yaml\n  - openapi/cardiff-echo.yaml\n  - openapi/cardiff-lookups.yaml\n  - openapi/cardiff-modules.yaml\n  - openapi/cardiff-publications.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/authentication/cardiff-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- United Kingdom
- Wales
- Open Data
- Courses
- Research
---
