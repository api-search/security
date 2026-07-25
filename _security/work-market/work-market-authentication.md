---
api_key_in:
- header
api_specs:
- filename: work-market-addressbook-api-openapi.yml
  format: yaml
  label: Work Market Addressbook API
  slug: work-market-addressbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-addressbook-api-openapi.yml
- filename: work-market-assignments-api-openapi.yml
  format: yaml
  label: Work Market Assignments API
  slug: work-market-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-assignments-api-openapi.yml
- filename: work-market-authorization-api-openapi.yml
  format: yaml
  label: Work Market Authorization API
  slug: work-market-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-authorization-api-openapi.yml
- filename: work-market-constants-api-openapi.yml
  format: yaml
  label: Work Market Constants API
  slug: work-market-constants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-constants-api-openapi.yml
- filename: work-market-custom-fields-api-openapi.yml
  format: yaml
  label: Work Market Custom Fields API
  slug: work-market-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-custom-fields-api-openapi.yml
- filename: work-market-labels-api-openapi.yml
  format: yaml
  label: Work Market Labels API
  slug: work-market-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-labels-api-openapi.yml
- filename: work-market-locations-api-openapi.yml
  format: yaml
  label: Work Market Locations API
  slug: work-market-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-locations-api-openapi.yml
- filename: work-market-projects-api-openapi.yml
  format: yaml
  label: Work Market Projects API
  slug: work-market-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-projects-api-openapi.yml
- filename: work-market-talent-pools-api-openapi.yml
  format: yaml
  label: Work Market Talent Pools API
  slug: work-market-talent-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-talent-pools-api-openapi.yml
- filename: work-market-updatecheckin-api-openapi.yml
  format: yaml
  label: Work Market UpdateCheckIn API
  slug: work-market-updatecheckin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-updatecheckin-api-openapi.yml
auth_types:
- accessToken
description: The WorkMarket Employer API uses an API token/secret pair exchanged for a short-lived access token. Credentials are generated in the WorkMarket web app; the client POSTs them to the authorization endpoint and then sends the returned access token as a Bearer credential in the Authorization header on subsequent requests. The published Swagger 2.0 spec declares no securityDefinitions; the scheme below is taken from the live API reference (which models it as an apiKey-style Authorization header) and the authorization operation in the spec.
kind: authentication
layout: security
method: searched
name: Work Market Authentication
name_suffix: Authentication
oauth_flows: []
overview: Work Market secures its APIs with accessToken across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Work Market
provider_slug: work-market
scheme_count: 1
schemes:
- format: Bearer <access token>
  in: header
  name: sec0
  parameter: Authorization
  sources:
  - https://employer-api.workmarket.com/reference/get-access-token
  type: apiKey
slug: work-market-authentication
source_filename: work-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://employer-api.workmarket.com/reference/get-access-token\ndocs: https://employer-api.workmarket.com/reference/get-access-token\ndescription: >-\n  The WorkMarket Employer API uses an API token/secret pair exchanged for a\n  short-lived access token. Credentials are generated in the WorkMarket web\n  app; the client POSTs them to the authorization endpoint and then sends the\n  returned access token as a Bearer credential in the Authorization header on\n  subsequent requests. The published Swagger 2.0 spec declares no\n  securityDefinitions; the scheme below is taken from the live API reference\n  (which models it as an apiKey-style Authorization header) and the\n  authorization operation in the spec.\nsummary:\n  types: [accessToken]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: sec0\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Bearer <access token>'\n    sources:\n\
  \      - https://employer-api.workmarket.com/reference/get-access-token\ntoken_exchange:\n  operation: openapi/work-market-employer-api-openapi.yml#request\n  path: POST /v1/employer/authorization/request\n  parameters:\n    - name: token\n      in: query\n      required: true\n      description: API token generated in the WorkMarket application\n    - name: secret\n      in: query\n      required: true\n      description: API secret generated in the WorkMarket application\n  returns: access token (Authorization definition) used as Bearer credential\nnotes:\n  - No OAuth 2.0 / OpenID Connect surface is published; scopes/ is not applicable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/authentication/work-market-authentication.yml
summary_line: accessToken · 1 scheme
tags:
- Workforce Management
- Contractors
- Freelance
- Gig Economy
- Human Resources
- Payments
- Field Services
- Staffing
---
