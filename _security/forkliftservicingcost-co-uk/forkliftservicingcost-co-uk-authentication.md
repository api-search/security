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
name: Forklift Servicing Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forklift Servicing Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forklift Servicing Cost
provider_slug: forkliftservicingcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/forkliftservicingcost-co-uk-openapi.json
  type: http
slug: forkliftservicingcost-co-uk-authentication
source_filename: forkliftservicingcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/forkliftservicingcost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/forkliftservicingcost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/forkliftservicingcost-co-uk/authentication/forkliftservicingcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Forklift
- Servicing
- LOLER
- HSE
---
