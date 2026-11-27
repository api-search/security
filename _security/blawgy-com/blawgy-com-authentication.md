---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blawgy-com-account-api-openapi.yml
  format: yaml
  label: blawgy-com Account API
  slug: blawgy-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-account-api-openapi.yml
- filename: blawgy-com-articles-api-openapi.yml
  format: yaml
  label: blawgy-com Articles API
  slug: blawgy-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-articles-api-openapi.yml
- filename: blawgy-com-builder-api-openapi.yml
  format: yaml
  label: blawgy-com Builder API
  slug: blawgy-com-builder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-builder-api-openapi.yml
- filename: blawgy-com-existing-pages-api-openapi.yml
  format: yaml
  label: blawgy-com Existing pages API
  slug: blawgy-com-existing-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-existing-pages-api-openapi.yml
- filename: blawgy-com-images-api-openapi.yml
  format: yaml
  label: blawgy-com Images API
  slug: blawgy-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-images-api-openapi.yml
- filename: blawgy-com-integrations-api-openapi.yml
  format: yaml
  label: blawgy-com Integrations API
  slug: blawgy-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-integrations-api-openapi.yml
- filename: blawgy-com-keywords-api-openapi.yml
  format: yaml
  label: blawgy-com Keywords API
  slug: blawgy-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-keywords-api-openapi.yml
- filename: blawgy-com-location-pages-api-openapi.yml
  format: yaml
  label: blawgy-com Location pages API
  slug: blawgy-com-location-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-location-pages-api-openapi.yml
- filename: blawgy-com-metrics-api-openapi.yml
  format: yaml
  label: blawgy-com Metrics API
  slug: blawgy-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-metrics-api-openapi.yml
- filename: blawgy-com-partner-api-openapi.yml
  format: yaml
  label: blawgy-com Partner API
  slug: blawgy-com-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-partner-api-openapi.yml
- filename: blawgy-com-plan-api-openapi.yml
  format: yaml
  label: blawgy-com Plan API
  slug: blawgy-com-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-plan-api-openapi.yml
- filename: blawgy-com-products-api-openapi.yml
  format: yaml
  label: blawgy-com Products API
  slug: blawgy-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-products-api-openapi.yml
- filename: blawgy-com-public-content-api-openapi.yml
  format: yaml
  label: blawgy-com Public content API
  slug: blawgy-com-public-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-public-content-api-openapi.yml
- filename: blawgy-com-refresh-api-openapi.yml
  format: yaml
  label: blawgy-com Refresh API
  slug: blawgy-com-refresh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-refresh-api-openapi.yml
- filename: blawgy-com-settings-api-openapi.yml
  format: yaml
  label: blawgy-com Settings API
  slug: blawgy-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-settings-api-openapi.yml
- filename: blawgy-com-support-api-openapi.yml
  format: yaml
  label: blawgy-com Support API
  slug: blawgy-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-support-api-openapi.yml
- filename: blawgy-com-team-and-billing-api-openapi.yml
  format: yaml
  label: blawgy-com Team and billing API
  slug: blawgy-com-team-and-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-team-and-billing-api-openapi.yml
- filename: blawgy-com-updates-api-openapi.yml
  format: yaml
  label: blawgy-com Updates API
  slug: blawgy-com-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-updates-api-openapi.yml
- filename: blawgy-com-webhooks-api-openapi.yml
  format: yaml
  label: blawgy-com Webhooks API
  slug: blawgy-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: blawgy-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: blawgy-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: blawgy-com
provider_slug: blawgy-com
scheme_count: 1
schemes:
- bearerFormat: blk_live_... API key or OAuth access token
  description: An API key from Settings > Account > AI agents in the Blawgy dashboard. Read keys may only call GET endpoints; keys scoped to specific sites cannot reach other sites or change the account.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blawgy-com-openapi.json
  type: http
slug: blawgy-com-authentication
source_filename: blawgy-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/blawgy-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: blk_live_... API key or OAuth access token\n  description: An API key from Settings > Account > AI agents in the Blawgy dashboard. Read\n    keys may only call GET endpoints; keys scoped to specific sites cannot reach other sites\n    or change the account.\n  sources:\n  - openapi/blawgy-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/blawgy-com/authentication/blawgy-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Content AI
- SEO
- Blog Publishing
- AI Search
- Agency Tools
---
