---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rice-datasets-api-openapi.yml
  format: yaml
  label: Rice University Datasets API
  slug: rice-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/openapi/rice-datasets-api-openapi.yml
- filename: rice-reference-api-openapi.yml
  format: yaml
  label: Rice University Reference API
  slug: rice-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/openapi/rice-reference-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Rice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rice University secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rice University
provider_slug: rice
scheme_count: 1
schemes:
- description: Undocumented. Inferred only from the API Gateway authorizer's 401 envelope on /user/catalog. Not verified — no credentials were obtained or used.
  name: memberSession
  scheme: bearer
  sources:
  - openapi/rice-datasets-api-openapi.yml
  - openapi/rice-reference-api-openapi.yml
  type: http
slug: rice-authentication
source_filename: rice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/rice-datasets-api-openapi.yml, openapi/rice-reference-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: memberSession\n  type: http\n  scheme: bearer\n  description: Undocumented. Inferred only from the API Gateway authorizer's 401 envelope on\n    /user/catalog. Not verified — no credentials were obtained or used.\n  sources:\n  - openapi/rice-datasets-api-openapi.yml\n  - openapi/rice-reference-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/authentication/rice-authentication.yml
summary_line: http · 1 scheme
tags:
- University
- Higher Education
- Education
- United States
- Texas
- Private Research University
- Association of American Universities
- Research Data
- Open Data
- Research Repository
- Course Catalog
- Identity Federation
- Library
- Urban Research
---
