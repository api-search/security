---
anonymous_access: false
api_key_in: []
api_specs:
- filename: twtapi-com-admin-api-openapi.yml
  format: yaml
  label: twtapi-com Admin API
  slug: twtapi-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-admin-api-openapi.yml
- filename: twtapi-com-agent-api-openapi.yml
  format: yaml
  label: twtapi-com Agent API
  slug: twtapi-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-agent-api-openapi.yml
- filename: twtapi-com-auth-api-openapi.yml
  format: yaml
  label: twtapi-com Auth API
  slug: twtapi-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-auth-api-openapi.yml
- filename: twtapi-com-captcha-api-openapi.yml
  format: yaml
  label: twtapi-com Captcha API
  slug: twtapi-com-captcha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-captcha-api-openapi.yml
- filename: twtapi-com-myapi-api-openapi.yml
  format: yaml
  label: twtapi-com Myapi API
  slug: twtapi-com-myapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-myapi-api-openapi.yml
- filename: twtapi-com-payment-api-openapi.yml
  format: yaml
  label: twtapi-com Payment API
  slug: twtapi-com-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-payment-api-openapi.yml
- filename: twtapi-com-twitter-api-openapi.yml
  format: yaml
  label: twtapi-com Twitter API
  slug: twtapi-com-twitter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-twitter-api-openapi.yml
- filename: twtapi-com-twtapi-backend-api-openapi.yml
  format: yaml
  label: twtapi-com TwtAPI Backend API
  slug: twtapi-com-twtapi-backend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twtapi-com/openapi/twtapi-com-twtapi-backend-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Twtapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: twtapi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: twtapi-com
provider_slug: twtapi-com
scheme_count: 2
schemes:
- description: API key provided in X-API-Key header
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token authentication
  scheme: bearer
  type: http
slug: twtapi-com-authentication
source_filename: twtapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://twtapi.com/zh/docs/\nschemes:\n  - type: \"apiKey\"\n    name: \"X-API-Key\"\n    in: \"header\"\n    description: \"API key provided in X-API-Key header\"\n  - type: \"http\"\n    scheme: \"bearer\"\n    bearerFormat: \"JWT\"\n    description: \"Bearer token authentication\"\n"
source_yaml_url: https://artifacts.apis.io/twtapi-com/authentication/twtapi-com-authentication.yml
summary_line: 2 schemes
tags:
- Twitter
- X
- API
- Data
- Search
- Monitoring
- AI
---
