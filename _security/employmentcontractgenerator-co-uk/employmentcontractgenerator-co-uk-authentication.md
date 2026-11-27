---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Employment Contract Generator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Employment Contract Generator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Employment Contract Generator
provider_slug: employmentcontractgenerator-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/employmentcontractgenerator-co-uk-openapi.json
  type: http
slug: employmentcontractgenerator-co-uk-authentication
source_filename: employmentcontractgenerator-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/employmentcontractgenerator-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/employmentcontractgenerator-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/employmentcontractgenerator-co-uk/authentication/employmentcontractgenerator-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Employment
- United Kingdom
- Contracts
- Legal
- Templates
- Human Resources
---
