---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: appskyline-com-apps-api-openapi.yml
  format: yaml
  label: AppSkyline Apps API
  slug: appskyline-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-apps-api-openapi.yml
- filename: appskyline-com-batch-api-openapi.yml
  format: yaml
  label: AppSkyline Batch API
  slug: appskyline-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-batch-api-openapi.yml
- filename: appskyline-com-google-play-publishing-api-openapi.yml
  format: yaml
  label: AppSkyline Google Play Publishing API
  slug: appskyline-com-google-play-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-google-play-publishing-api-openapi.yml
- filename: appskyline-com-keywords-api-openapi.yml
  format: yaml
  label: AppSkyline Keywords API
  slug: appskyline-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-keywords-api-openapi.yml
- filename: appskyline-com-metadata-api-openapi.yml
  format: yaml
  label: AppSkyline Metadata API
  slug: appskyline-com-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-metadata-api-openapi.yml
- filename: appskyline-com-review-status-api-openapi.yml
  format: yaml
  label: AppSkyline Review Status API
  slug: appskyline-com-review-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-review-status-api-openapi.yml
- filename: appskyline-com-sandbox-api-openapi.yml
  format: yaml
  label: AppSkyline Sandbox API
  slug: appskyline-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-sandbox-api-openapi.yml
- filename: appskyline-com-stats-api-openapi.yml
  format: yaml
  label: AppSkyline Stats API
  slug: appskyline-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-stats-api-openapi.yml
- filename: appskyline-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: AppSkyline Webhook subscriptions API
  slug: appskyline-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-webhook-subscriptions-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Appskyline Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppSkyline secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppSkyline
provider_slug: appskyline-com
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying only the API key secret: Authorization: Basic base64(<key secret>).'
  name: apiKey
  scheme: basic
  sources:
  - openapi/appskyline-com-openapi.json
  type: http
- description: 'Operator session token issued by the AppSkyline dashboard: Authorization: Token <access token>.'
  in: header
  name: accessToken
  parameter: Authorization
  sources:
  - openapi/appskyline-com-openapi.json
  type: apiKey
slug: appskyline-com-authentication
source_filename: appskyline-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/appskyline-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: http\n  scheme: basic\n  description: 'HTTP Basic auth carrying only the API key secret: Authorization: Basic base64(<key\n    secret>).'\n  sources:\n  - openapi/appskyline-com-openapi.json\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Operator session token issued by the AppSkyline dashboard: Authorization: Token\n    <access token>.'\n  sources:\n  - openapi/appskyline-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/appskyline-com/authentication/appskyline-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- App Store Optimization
- Analytics
- Marketing
- Software-as-a-Service
- Developer Tools
- Company
---
