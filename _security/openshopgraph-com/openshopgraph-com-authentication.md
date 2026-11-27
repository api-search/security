---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: OpenShopGraph Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenShopGraph secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenShopGraph
provider_slug: openshopgraph-com
scheme_count: 1
schemes:
- in: header
  name: ApiToken
  parameter: x-api-token
  sources:
  - openapi/openshopgraph-com-openapi.yml
  type: apiKey
slug: openshopgraph-com-authentication
source_filename: openshopgraph-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/openshopgraph-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: x-api-token\n  sources:\n  - openapi/openshopgraph-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/openshopgraph-com/authentication/openshopgraph-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-Commerce
- Data Aggregation
- Shopping Assistant
- Transparency
- Open Source
---
