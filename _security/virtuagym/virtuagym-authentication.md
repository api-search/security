---
api_key_in: []
api_specs:
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Club Members API
  slug: virtuagym-club-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Club Employees API
  slug: virtuagym-club-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Memberships API
  slug: virtuagym-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Billing API
  slug: virtuagym-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Visits API
  slug: virtuagym-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Events API
  slug: virtuagym-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Coaching Workouts API
  slug: virtuagym-coaching-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Virtuagym Authentication
name_suffix: Authentication
oauth_flows: []
overview: Virtuagym secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Virtuagym
provider_slug: virtuagym
scheme_count: 2
schemes:
- description: The club's API key, provisioned in the Virtuagym portal under System settings > Business info > Advanced. Passed as the `api_key` query-string parameter on every v1 request.
  in: query
  name: apiKeyAuth
  parameterName: api_key
  sources:
  - openapi/virtuagym-openapi.yml
  type: apiKey
- description: The club secret, provisioned alongside the API key in the Virtuagym portal. Required in addition to the API key on all v1 endpoints, passed as the `club_secret` query-string parameter.
  in: query
  name: clubSecretAuth
  parameterName: club_secret
  sources:
  - openapi/virtuagym-openapi.yml
  type: apiKey
slug: virtuagym-authentication
source_filename: virtuagym-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/virtuagym-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameterName: api_key\n  description: >-\n    The club's API key, provisioned in the Virtuagym portal under System\n    settings > Business info > Advanced. Passed as the `api_key` query-string\n    parameter on every v1 request.\n  sources:\n  - openapi/virtuagym-openapi.yml\n- name: clubSecretAuth\n  type: apiKey\n  in: query\n  parameterName: club_secret\n  description: >-\n    The club secret, provisioned alongside the API key in the Virtuagym portal.\n    Required in addition to the API key on all v1 endpoints, passed as the\n    `club_secret` query-string parameter.\n  sources:\n  - openapi/virtuagym-openapi.yml\nnotes: >-\n  v1 endpoints require BOTH api_key and club_secret together, over HTTPS only\n  (insecure connections are rejected). Legacy v0 endpoints (deprecated) used HTTP\n  Basic Auth\
  \ with a Virtuagym user's username/password. A separate OAuth 2.0\n  authorization-code flow (authorize at www.virtuagym.com/oauth/authorize, token\n  at virtuagym.com/oauth/token, using a client_id / client_secret) exists for\n  end-user-context calls, and the Lead API (V3) uses its own client_id /\n  client_secret - these are out of scope for the club-scoped v1 surface modeled\n  here. Authoritative auth documentation is access-gated; request access via\n  api@virtuagym.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/authentication/virtuagym-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Fitness
- Health Club Management
- Gym Management
- Coaching
- Membership Management
- Fitness Software
- Wellness
- Scheduling
- SaaS
---
