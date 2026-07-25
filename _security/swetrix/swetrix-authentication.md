---
api_key_in:
- header
api_specs:
- filename: swetrix-events-api-openapi.yml
  format: yaml
  label: Swetrix Events API
  slug: swetrix-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-events-api-openapi.yml
- filename: swetrix-annotations-api-openapi.yml
  format: yaml
  label: Swetrix Annotations API
  slug: swetrix-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-annotations-api-openapi.yml
- filename: swetrix-custom-events-api-openapi.yml
  format: yaml
  label: Swetrix Custom Events API
  slug: swetrix-custom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-custom-events-api-openapi.yml
- filename: swetrix-errors-api-openapi.yml
  format: yaml
  label: Swetrix Errors API
  slug: swetrix-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-errors-api-openapi.yml
- filename: swetrix-feature-flags-api-openapi.yml
  format: yaml
  label: Swetrix Feature Flags API
  slug: swetrix-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-feature-flags-api-openapi.yml
- filename: swetrix-funnels-api-openapi.yml
  format: yaml
  label: Swetrix Funnels API
  slug: swetrix-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-funnels-api-openapi.yml
- filename: swetrix-organisations-api-openapi.yml
  format: yaml
  label: Swetrix Organisations API
  slug: swetrix-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-organisations-api-openapi.yml
- filename: swetrix-performance-api-openapi.yml
  format: yaml
  label: Swetrix Performance API
  slug: swetrix-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-performance-api-openapi.yml
- filename: swetrix-projects-api-openapi.yml
  format: yaml
  label: Swetrix Projects API
  slug: swetrix-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-projects-api-openapi.yml
- filename: swetrix-revenue-api-openapi.yml
  format: yaml
  label: Swetrix Revenue API
  slug: swetrix-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-revenue-api-openapi.yml
- filename: swetrix-sessions-api-openapi.yml
  format: yaml
  label: Swetrix Sessions API
  slug: swetrix-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-sessions-api-openapi.yml
- filename: swetrix-traffic-api-openapi.yml
  format: yaml
  label: Swetrix Traffic API
  slug: swetrix-traffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-traffic-api-openapi.yml
- filename: swetrix-views-api-openapi.yml
  format: yaml
  label: Swetrix Views API
  slug: swetrix-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-views-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Swetrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swetrix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Swetrix
provider_slug: swetrix
scheme_count: 1
schemes:
- description: API key from Swetrix account settings (https://swetrix.com/user-settings)
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/swetrix-admin-api-openapi.yml
  - openapi/swetrix-events-api-openapi.yml
  - openapi/swetrix-statistics-api-openapi.yml
  type: apiKey
slug: swetrix-authentication
source_filename: swetrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swetrix-admin-api-openapi.yml, openapi/swetrix-events-api-openapi.yml, openapi/swetrix-statistics-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key from Swetrix account settings (https://swetrix.com/user-settings)\n  sources:\n  - openapi/swetrix-admin-api-openapi.yml\n  - openapi/swetrix-events-api-openapi.yml\n  - openapi/swetrix-statistics-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/authentication/swetrix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Cookieless Tracking
- GDPR Compliant
- Open Source
- Privacy
- Real-Time Analytics
- Web Analytics
---
