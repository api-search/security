---
anonymous_access: false
api_key_in: []
api_specs:
- filename: searlo-tech-account-api-openapi.yml
  format: yaml
  label: searlo-tech Account API
  slug: searlo-tech-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-account-api-openapi.yml
- filename: searlo-tech-ai-answers-api-openapi.yml
  format: yaml
  label: searlo-tech AI Answers API
  slug: searlo-tech-ai-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-ai-answers-api-openapi.yml
- filename: searlo-tech-async-api-openapi.yml
  format: yaml
  label: searlo-tech Async API
  slug: searlo-tech-async-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-async-api-openapi.yml
- filename: searlo-tech-domain-api-openapi.yml
  format: yaml
  label: searlo-tech Domain API
  slug: searlo-tech-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-domain-api-openapi.yml
- filename: searlo-tech-rankings-api-openapi.yml
  format: yaml
  label: searlo-tech Rankings API
  slug: searlo-tech-rankings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-rankings-api-openapi.yml
- filename: searlo-tech-search-api-openapi.yml
  format: yaml
  label: searlo-tech Search API
  slug: searlo-tech-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-search-api-openapi.yml
- filename: searlo-tech-serp-api-openapi.yml
  format: yaml
  label: searlo-tech SERP API
  slug: searlo-tech-serp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-serp-api-openapi.yml
- filename: searlo-tech-tools-api-openapi.yml
  format: yaml
  label: searlo-tech Tools API
  slug: searlo-tech-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-tools-api-openapi.yml
- filename: searlo-tech-web-data-api-openapi.yml
  format: yaml
  label: searlo-tech Web Data API
  slug: searlo-tech-web-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searlo-tech/openapi/searlo-tech-web-data-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Searlo Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: searlo-tech declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: searlo-tech
provider_slug: searlo-tech
scheme_count: 3
schemes:
- description: API key from your Searlo dashboard, e.g. sk_....
  id: ApiKeyAuth
  in: header
  name: x-api-key
  type: apiKey
- description: 'The same API key, sent as Authorization: Bearer sk_....'
  id: BearerAuth
  scheme: bearer
  type: http
- description: The Searlo API key as the key query parameter, used by /customsearch/v1.
  id: CseKeyParam
  in: query
  name: key
  type: apiKey
slug: searlo-tech-authentication
source_filename: searlo-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://searlo.tech/openapi.yaml\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: >-\n      API key from your Searlo dashboard, e.g. sk_....\n    id: ApiKeyAuth\n  - type: http\n    scheme: bearer\n    description: >-\n      The same API key, sent as Authorization: Bearer sk_....\n    id: BearerAuth\n  - type: apiKey\n    name: key\n    in: query\n    description: >-\n      The Searlo API key as the key query parameter, used by /customsearch/v1.\n    id: CseKeyParam\n"
source_yaml_url: https://artifacts.apis.io/searlo-tech/authentication/searlo-tech-authentication.yml
summary_line: 3 schemes
tags:
- Search
- SERP
- API
- AI
- Data
---
