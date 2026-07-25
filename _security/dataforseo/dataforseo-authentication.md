---
api_key_in: []
api_specs:
- filename: dataforseo-aioptimization-api-openapi.yml
  format: yaml
  label: DataForSEO AiOptimization API
  slug: dataforseo-aioptimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-aioptimization-api-openapi.yml
- filename: dataforseo-appdata-api-openapi.yml
  format: yaml
  label: DataForSEO AppData API
  slug: dataforseo-appdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-appdata-api-openapi.yml
- filename: dataforseo-appendix-api-openapi.yml
  format: yaml
  label: DataForSEO Appendix API
  slug: dataforseo-appendix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-appendix-api-openapi.yml
- filename: dataforseo-backlinks-api-openapi.yml
  format: yaml
  label: DataForSEO Backlinks API
  slug: dataforseo-backlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-backlinks-api-openapi.yml
- filename: dataforseo-businessdata-api-openapi.yml
  format: yaml
  label: DataForSEO BusinessData API
  slug: dataforseo-businessdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-businessdata-api-openapi.yml
- filename: dataforseo-contentanalysis-api-openapi.yml
  format: yaml
  label: DataForSEO ContentAnalysis API
  slug: dataforseo-contentanalysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-contentanalysis-api-openapi.yml
- filename: dataforseo-dataforseolabs-api-openapi.yml
  format: yaml
  label: DataForSEO DataforseoLabs API
  slug: dataforseo-dataforseolabs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-dataforseolabs-api-openapi.yml
- filename: dataforseo-domainanalytics-api-openapi.yml
  format: yaml
  label: DataForSEO DomainAnalytics API
  slug: dataforseo-domainanalytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-domainanalytics-api-openapi.yml
- filename: dataforseo-keywordsdata-api-openapi.yml
  format: yaml
  label: DataForSEO KeywordsData API
  slug: dataforseo-keywordsdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-keywordsdata-api-openapi.yml
- filename: dataforseo-merchant-api-openapi.yml
  format: yaml
  label: DataForSEO Merchant API
  slug: dataforseo-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-merchant-api-openapi.yml
- filename: dataforseo-onpage-api-openapi.yml
  format: yaml
  label: DataForSEO OnPage API
  slug: dataforseo-onpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-onpage-api-openapi.yml
- filename: dataforseo-serp-api-openapi.yml
  format: yaml
  label: DataForSEO Serp API
  slug: dataforseo-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-serp-api-openapi.yml
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
