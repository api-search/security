---
api_key_in:
- query
api_specs:
- filename: overview
  format: yaml
  label: SE Ranking Data API
  slug: data-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
- filename: overview
  format: yaml
  label: SE Ranking Project API
  slug: project-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Se Ranking Authentication
name_suffix: Authentication
oauth_flows: []
overview: SE Ranking secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SE Ranking
provider_slug: se-ranking
scheme_count: 1
schemes:
- in: query
  name: apikeyAuth
  parameter: apikey
  sources:
  - openapi/se-ranking-data-api-openapi.yml
  type: apiKey
slug: se-ranking-authentication
source_filename: se-ranking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/se-ranking-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/se-ranking-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/authentication/se-ranking-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- SEO
- Keyword Research
- Rank Tracking
- Backlinks
- Competitor Analysis
- Website Audit
- AI Search
- GEO
- Digital Marketing
---
