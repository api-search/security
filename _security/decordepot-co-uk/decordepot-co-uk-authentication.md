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
name: Decordepot Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Decor Depot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Decor Depot
provider_slug: decordepot-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/decordepot-co-uk-openapi.json
  type: http
slug: decordepot-co-uk-authentication
source_filename: decordepot-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/decordepot-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/decordepot-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/decordepot-co-uk/authentication/decordepot-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- E-Commerce
- Furniture
- United Kingdom
- Retail
---
