---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adslighthouse-account-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Account API
  slug: adslighthouse-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-account-api-openapi.yml
- filename: adslighthouse-alerts-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Alerts API
  slug: adslighthouse-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-alerts-api-openapi.yml
- filename: adslighthouse-checks-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Checks API
  slug: adslighthouse-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-checks-api-openapi.yml
- filename: adslighthouse-google-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Google API
  slug: adslighthouse-google-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-google-api-openapi.yml
- filename: adslighthouse-keywords-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Keywords API
  slug: adslighthouse-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-keywords-api-openapi.yml
- filename: adslighthouse-matching-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Matching API
  slug: adslighthouse-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-matching-api-openapi.yml
- filename: adslighthouse-observations-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Observations API
  slug: adslighthouse-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-observations-api-openapi.yml
- filename: adslighthouse-policy-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Policy API
  slug: adslighthouse-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-policy-api-openapi.yml
- filename: adslighthouse-prices-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Prices API
  slug: adslighthouse-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-prices-api-openapi.yml
- filename: adslighthouse-projects-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Projects API
  slug: adslighthouse-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-projects-api-openapi.yml
- filename: adslighthouse-redirect-chains-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Redirect chains API
  slug: adslighthouse-redirect-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-redirect-chains-api-openapi.yml
- filename: adslighthouse-reports-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Reports API
  slug: adslighthouse-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-reports-api-openapi.yml
- filename: adslighthouse-router-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Router API
  slug: adslighthouse-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-router-api-openapi.yml
- filename: adslighthouse-team-api-openapi.yml
  format: yaml
  label: Ads Lighthouse Team API
  slug: adslighthouse-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/openapi/adslighthouse-team-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Adslighthouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ads Lighthouse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ads Lighthouse
provider_slug: adslighthouse
scheme_count: 1
schemes:
- description: An API key from Settings > API and MCP (als_...), or an OAuth access token issued for this API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/adslighthouse-openapi.json
  type: http
slug: adslighthouse-authentication
source_filename: adslighthouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: derived\nsource: openapi/adslighthouse-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An API key from Settings > API and MCP (als_...), or an OAuth access token issued\n    for this API.\n  sources:\n  - openapi/adslighthouse-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adslighthouse/refs/heads/main/authentication/adslighthouse-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Advertising
- Monitoring
- BrandProtection
- API
---
