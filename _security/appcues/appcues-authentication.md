---
api_key_in: []
api_specs:
- filename: appcues-banners-api-openapi.yml
  format: yaml
  label: Appcues Banners API
  slug: appcues-banners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-banners-api-openapi.yml
- filename: appcues-events-api-openapi.yml
  format: yaml
  label: Appcues Events API
  slug: appcues-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-events-api-openapi.yml
- filename: appcues-exports-api-openapi.yml
  format: yaml
  label: Appcues Exports API
  slug: appcues-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-exports-api-openapi.yml
- filename: appcues-flows-api-openapi.yml
  format: yaml
  label: Appcues Flows API
  slug: appcues-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-flows-api-openapi.yml
- filename: appcues-groups-api-openapi.yml
  format: yaml
  label: Appcues Groups API
  slug: appcues-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-groups-api-openapi.yml
- filename: appcues-imports-api-openapi.yml
  format: yaml
  label: Appcues Imports API
  slug: appcues-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-imports-api-openapi.yml
- filename: appcues-jobs-api-openapi.yml
  format: yaml
  label: Appcues Jobs API
  slug: appcues-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-jobs-api-openapi.yml
- filename: appcues-launchpads-api-openapi.yml
  format: yaml
  label: Appcues Launchpads API
  slug: appcues-launchpads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-launchpads-api-openapi.yml
- filename: appcues-mobile-api-openapi.yml
  format: yaml
  label: Appcues Mobile API
  slug: appcues-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-mobile-api-openapi.yml
- filename: appcues-pins-api-openapi.yml
  format: yaml
  label: Appcues Pins API
  slug: appcues-pins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-pins-api-openapi.yml
- filename: appcues-segments-api-openapi.yml
  format: yaml
  label: Appcues Segments API
  slug: appcues-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-segments-api-openapi.yml
- filename: appcues-tags-api-openapi.yml
  format: yaml
  label: Appcues Tags API
  slug: appcues-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-tags-api-openapi.yml
- filename: appcues-users-api-openapi.yml
  format: yaml
  label: Appcues Users API
  slug: appcues-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/openapi/appcues-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appcues Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appcues secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appcues
provider_slug: appcues
scheme_count: 1
schemes:
- description: HTTP Basic authentication using API_KEY as username and API_SECRET as password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/appcues-openapi.yml
  type: http
slug: appcues-authentication
source_filename: appcues-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appcues-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using API_KEY as username and API_SECRET as password.\n  sources:\n  - openapi/appcues-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcues/refs/heads/main/authentication/appcues-authentication.yml
summary_line: http · 1 scheme
tags:
- Product
- Onboarding
- In-App Guidance
- Analytics
- Customer Success
---
