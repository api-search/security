---
api_key_in: []
api_specs:
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO SERP API
  slug: dataforseo-serp-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO Keywords Data API
  slug: dataforseo-keywords-data-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO Backlinks API
  slug: dataforseo-backlinks-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO Labs API
  slug: dataforseo-labs-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO Domain Analytics API
  slug: dataforseo-domain-analytics-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO On-Page API
  slug: dataforseo-on-page-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO Content Analysis API
  slug: dataforseo-content-analysis-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO Business Data API
  slug: dataforseo-business-data-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO App Data API
  slug: dataforseo-app-data-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO Merchant API
  slug: dataforseo-merchant-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO AI Optimization API
  slug: dataforseo-ai-optimization-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
- filename: OpenApiDocumentation
  format: yaml
  label: DataForSEO Social Media API
  slug: dataforseo-social-media-api
  spec_type: OpenAPI
  url: https://github.com/dataforseo/OpenApiDocumentation
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dataforseo Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataForSEO secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataForSEO
provider_slug: dataforseo
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/dataforseo-ai-optimization-openapi.yml
  - openapi/dataforseo-app-data-openapi.yml
  - openapi/dataforseo-appendix-openapi.yml
  - openapi/dataforseo-business-data-openapi.yml
  - openapi/dataforseo-keywords-data-openapi.yml
  - openapi/dataforseo-labs-openapi.yml
  - openapi/dataforseo-merchant-openapi.yml
  - openapi/dataforseo-serp-openapi.yml
  type: http
slug: dataforseo-authentication
source_filename: dataforseo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dataforseo-ai-optimization-openapi.yml, openapi/dataforseo-app-data-openapi.yml,\n  openapi/dataforseo-appendix-openapi.yml, openapi/dataforseo-business-data-openapi.yml, openapi/dataforseo-keywords-data-openapi.yml,\n  openapi/dataforseo-labs-openapi.yml, openapi/dataforseo-merchant-openapi.yml, openapi/dataforseo-serp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/dataforseo-ai-optimization-openapi.yml\n  - openapi/dataforseo-app-data-openapi.yml\n  - openapi/dataforseo-appendix-openapi.yml\n  - openapi/dataforseo-business-data-openapi.yml\n  - openapi/dataforseo-keywords-data-openapi.yml\n  - openapi/dataforseo-labs-openapi.yml\n  - openapi/dataforseo-merchant-openapi.yml\n  - openapi/dataforseo-serp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/authentication/dataforseo-authentication.yml
summary_line: http · 1 scheme
tags:
- SEO
- SERP
- Keywords
- Backlinks
- Domain Analytics
- On-Page SEO
- Competitor Research
- Search Engines
- Content Analysis
- E-Commerce
- App Store
- Business Data
- AI Optimization
- Social Media
---
