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
- filename: se-ranking-account-system-api-openapi.yml
  format: yaml
  label: SE Ranking Account & system API
  slug: se-ranking-account-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-account-system-api-openapi.yml
- filename: se-ranking-ai-search-api-openapi.yml
  format: yaml
  label: SE Ranking AI search API
  slug: se-ranking-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-ai-search-api-openapi.yml
- filename: se-ranking-backlinks-api-openapi.yml
  format: yaml
  label: SE Ranking backlinks API
  slug: se-ranking-backlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-backlinks-api-openapi.yml
- filename: se-ranking-domain-analysis-api-openapi.yml
  format: yaml
  label: SE Ranking Domain Analysis API
  slug: se-ranking-domain-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-domain-analysis-api-openapi.yml
- filename: se-ranking-keyword-research-api-openapi.yml
  format: yaml
  label: SE Ranking Keyword Research API
  slug: se-ranking-keyword-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-keyword-research-api-openapi.yml
- filename: se-ranking-serp-results-classic-api-openapi.yml
  format: yaml
  label: SE Ranking SERP Results > classic API
  slug: se-ranking-serp-results-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-serp-results-classic-api-openapi.yml
- filename: se-ranking-website-audit-api-openapi.yml
  format: yaml
  label: SE Ranking Website Audit API
  slug: se-ranking-website-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-website-audit-api-openapi.yml
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
