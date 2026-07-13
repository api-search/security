---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Relational Data Modeling Authentication
name_suffix: Authentication
oauth_flows: []
overview: Relational Data Modeling secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Relational Data Modeling
provider_slug: relational-data-modeling
scheme_count: 1
schemes:
- description: 'Bearer token issued from the SqlDBM workspace. See the

    Authorization section in the SqlDBM developer documentation for

    details on obtaining and using API credentials.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/relational-data-modeling-openapi.yml
  type: http
slug: relational-data-modeling-authentication
source_filename: relational-data-modeling-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/relational-data-modeling-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token issued from the SqlDBM workspace. See the\n    Authorization section in the SqlDBM developer documentation for\n    details on obtaining and using API credentials.\n  sources:\n  - openapi/relational-data-modeling-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relational-data-modeling/refs/heads/main/authentication/relational-data-modeling-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Architecture
- Database Design
- Entity Relationship
- Normalization
- SQL
- Schema Design
- Data Modeling
---
