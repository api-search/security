---
api_key_in: []
api_specs:
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Members API
  slug: yourmembership-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Events API
  slug: yourmembership-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Certifications API
  slug: yourmembership-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YMCareers API
  slug: yourmembership-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Content and Community API
  slug: yourmembership-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Commerce and Sales API
  slug: yourmembership-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Yourmembership Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: YourMembership secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: YourMembership
provider_slug: yourmembership
scheme_count: 1
schemes:
- description: OAuth authentication for the YM REST API, established via POST /Ams/Authenticate. The YMCareers API instead uses an API_ACCESS_TOKEN (15-minute) Authorization header or a non-expiring X-API-KEY header.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://ws.yourmembership.com/Ams/Authenticate
  name: oauth2
  sources:
  - openapi/yourmembership-openapi.yml
  type: oauth2
slug: yourmembership-authentication
source_filename: yourmembership-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yourmembership-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ws.yourmembership.com/Ams/Authenticate\n    scopes: 0\n  description: OAuth authentication for the YM REST API, established via POST /Ams/Authenticate.\n    The YMCareers API instead uses an API_ACCESS_TOKEN (15-minute) Authorization header or a\n    non-expiring X-API-KEY header.\n  sources:\n  - openapi/yourmembership-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/authentication/yourmembership-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Membership Management
- Association Management
- AMS
- Nonprofit
- Events
- Careers
- Community Brands
- Momentive Software
---
