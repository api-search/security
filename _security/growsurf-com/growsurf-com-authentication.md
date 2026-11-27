---
anonymous_access: false
api_key_in: []
api_specs:
- filename: growsurf-com-affiliate-programs-api-openapi.yml
  format: yaml
  label: GrowSurf Affiliate Programs API
  slug: growsurf-com-affiliate-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growsurf-com/openapi/growsurf-com-affiliate-programs-api-openapi.yml
- filename: growsurf-com-analytics-api-openapi.yml
  format: yaml
  label: GrowSurf Analytics API
  slug: growsurf-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growsurf-com/openapi/growsurf-com-analytics-api-openapi.yml
- filename: growsurf-com-campaign-webhooks-api-openapi.yml
  format: yaml
  label: GrowSurf Campaign Webhooks API
  slug: growsurf-com-campaign-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growsurf-com/openapi/growsurf-com-campaign-webhooks-api-openapi.yml
- filename: growsurf-com-campaigns-api-openapi.yml
  format: yaml
  label: GrowSurf Campaigns API
  slug: growsurf-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growsurf-com/openapi/growsurf-com-campaigns-api-openapi.yml
- filename: growsurf-com-participant-rewards-api-openapi.yml
  format: yaml
  label: GrowSurf Participant Rewards API
  slug: growsurf-com-participant-rewards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growsurf-com/openapi/growsurf-com-participant-rewards-api-openapi.yml
- filename: growsurf-com-participants-api-openapi.yml
  format: yaml
  label: GrowSurf Participants API
  slug: growsurf-com-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growsurf-com/openapi/growsurf-com-participants-api-openapi.yml
- filename: growsurf-com-referrals-and-invites-api-openapi.yml
  format: yaml
  label: GrowSurf Referrals and Invites API
  slug: growsurf-com-referrals-and-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growsurf-com/openapi/growsurf-com-referrals-and-invites-api-openapi.yml
- filename: growsurf-com-teams-api-openapi.yml
  format: yaml
  label: GrowSurf Teams API
  slug: growsurf-com-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growsurf-com/openapi/growsurf-com-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GrowSurf Authentication
name_suffix: Authentication
oauth_flows: []
overview: GrowSurf secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GrowSurf
provider_slug: growsurf-com
scheme_count: 1
schemes:
- bearerFormat: API key
  description: 'GrowSurf REST API key supplied as `Authorization: Bearer <api_key>`.'
  name: apiKeyAuth
  scheme: bearer
  sources:
  - openapi/growsurf-com-openapi.json
  type: http
slug: growsurf-com-authentication
source_filename: growsurf-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/growsurf-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'GrowSurf REST API key supplied as `Authorization: Bearer <api_key>`.'\n  sources:\n  - openapi/growsurf-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/growsurf-com/authentication/growsurf-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Referrals
- Marketing
- Software-as-a-Service
- Healthcare
- Fintech
- Company
---
