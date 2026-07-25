---
api_key_in: []
api_specs:
- filename: pirsch-access-links-api-openapi.yml
  format: yaml
  label: Pirsch Access Links API
  slug: pirsch-access-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-access-links-api-openapi.yml
- filename: pirsch-authentication-api-openapi.yml
  format: yaml
  label: Pirsch Authentication API
  slug: pirsch-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-authentication-api-openapi.yml
- filename: pirsch-clients-api-openapi.yml
  format: yaml
  label: Pirsch Clients API
  slug: pirsch-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-clients-api-openapi.yml
- filename: pirsch-conversion-goals-api-openapi.yml
  format: yaml
  label: Pirsch Conversion Goals API
  slug: pirsch-conversion-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-conversion-goals-api-openapi.yml
- filename: pirsch-domains-api-openapi.yml
  format: yaml
  label: Pirsch Domains API
  slug: pirsch-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-domains-api-openapi.yml
- filename: pirsch-email-reports-api-openapi.yml
  format: yaml
  label: Pirsch Email Reports API
  slug: pirsch-email-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-email-reports-api-openapi.yml
- filename: pirsch-funnels-api-openapi.yml
  format: yaml
  label: Pirsch Funnels API
  slug: pirsch-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-funnels-api-openapi.yml
- filename: pirsch-members-api-openapi.yml
  format: yaml
  label: Pirsch Members API
  slug: pirsch-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-members-api-openapi.yml
- filename: pirsch-short-links-api-openapi.yml
  format: yaml
  label: Pirsch Short Links API
  slug: pirsch-short-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-short-links-api-openapi.yml
- filename: pirsch-statistics-api-openapi.yml
  format: yaml
  label: Pirsch Statistics API
  slug: pirsch-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-statistics-api-openapi.yml
- filename: pirsch-tracking-api-openapi.yml
  format: yaml
  label: Pirsch Tracking API
  slug: pirsch-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-tracking-api-openapi.yml
- filename: pirsch-traffic-management-api-openapi.yml
  format: yaml
  label: Pirsch Traffic Management API
  slug: pirsch-traffic-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-traffic-management-api-openapi.yml
- filename: pirsch-user-api-openapi.yml
  format: yaml
  label: Pirsch User API
  slug: pirsch-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-user-api-openapi.yml
- filename: pirsch-views-api-openapi.yml
  format: yaml
  label: Pirsch Views API
  slug: pirsch-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-views-api-openapi.yml
- filename: pirsch-webhooks-api-openapi.yml
  format: yaml
  label: Pirsch Webhooks API
  slug: pirsch-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pirsch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pirsch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pirsch
provider_slug: pirsch
scheme_count: 1
schemes:
- description: Pass an OAuth2 access token obtained from POST /token, or a static access key, as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/pirsch-pirsch-api-openapi.yml
  type: http
slug: pirsch-authentication
source_filename: pirsch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pirsch-pirsch-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Pass an OAuth2 access token obtained from POST /token, or a static access key,\n    as a Bearer token in the Authorization header.\n  sources:\n  - openapi/pirsch-pirsch-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/authentication/pirsch-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Web Analytics
- Privacy
- GDPR
- Cookie-Free
- Page Views
- Sessions
- Events
- Conversion Goals
- Funnels
- Traffic Sources
---
