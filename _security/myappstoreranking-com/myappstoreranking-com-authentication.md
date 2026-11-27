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
name: My App Store Ranking Authentication
name_suffix: Authentication
oauth_flows: []
overview: My App Store Ranking secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: My App Store Ranking
provider_slug: myappstoreranking-com
scheme_count: 1
schemes:
- description: An OAuth access token from the MCP connection flow, or a personal access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/myappstoreranking-com-openapi.json
  type: http
slug: myappstoreranking-com-authentication
source_filename: myappstoreranking-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myappstoreranking-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An OAuth access token from the MCP connection flow, or a personal access token.\n  sources:\n  - openapi/myappstoreranking-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/myappstoreranking-com/authentication/myappstoreranking-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AppRanking
- Mobile Analytics
- Competitor Intelligence
- Artificial Intelligence
- Software-as-a-Service
---
