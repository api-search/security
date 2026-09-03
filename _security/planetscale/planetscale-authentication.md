---
api_key_in:
- header
api_specs:
- filename: planetscale-backups-api-openapi.yml
  format: yaml
  label: planetscale Backups API
  slug: planetscale-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-backups-api-openapi.yml
- filename: planetscale-billing-api-openapi.yml
  format: yaml
  label: planetscale Billing API
  slug: planetscale-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-billing-api-openapi.yml
- filename: planetscale-bouncers-api-openapi.yml
  format: yaml
  label: planetscale Bouncers API
  slug: planetscale-bouncers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-bouncers-api-openapi.yml
- filename: planetscale-branches-api-openapi.yml
  format: yaml
  label: planetscale Branches API
  slug: planetscale-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-branches-api-openapi.yml
- filename: planetscale-cluster-sizes-api-openapi.yml
  format: yaml
  label: planetscale Cluster Sizes API
  slug: planetscale-cluster-sizes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-cluster-sizes-api-openapi.yml
- filename: planetscale-databases-api-openapi.yml
  format: yaml
  label: planetscale Databases API
  slug: planetscale-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-databases-api-openapi.yml
- filename: planetscale-deploy-requests-api-openapi.yml
  format: yaml
  label: planetscale Deploy Requests API
  slug: planetscale-deploy-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-deploy-requests-api-openapi.yml
- filename: planetscale-ip-restrictions-api-openapi.yml
  format: yaml
  label: planetscale IP Restrictions API
  slug: planetscale-ip-restrictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-ip-restrictions-api-openapi.yml
- filename: planetscale-organization-members-api-openapi.yml
  format: yaml
  label: planetscale Organization Members API
  slug: planetscale-organization-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-organization-members-api-openapi.yml
- filename: planetscale-organizations-api-openapi.yml
  format: yaml
  label: planetscale Organizations API
  slug: planetscale-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-organizations-api-openapi.yml
- filename: planetscale-passwords-api-openapi.yml
  format: yaml
  label: planetscale Passwords API
  slug: planetscale-passwords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-passwords-api-openapi.yml
- filename: planetscale-query-patterns-api-openapi.yml
  format: yaml
  label: planetscale Query Patterns API
  slug: planetscale-query-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-query-patterns-api-openapi.yml
- filename: planetscale-roles-api-openapi.yml
  format: yaml
  label: planetscale Roles API
  slug: planetscale-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-roles-api-openapi.yml
- filename: planetscale-schema-recommendations-api-openapi.yml
  format: yaml
  label: planetscale Schema Recommendations API
  slug: planetscale-schema-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-schema-recommendations-api-openapi.yml
- filename: planetscale-service-tokens-api-openapi.yml
  format: yaml
  label: planetscale Service Tokens API
  slug: planetscale-service-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-service-tokens-api-openapi.yml
- filename: planetscale-teams-api-openapi.yml
  format: yaml
  label: planetscale Teams API
  slug: planetscale-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-teams-api-openapi.yml
- filename: planetscale-webhooks-api-openapi.yml
  format: yaml
  label: planetscale Webhooks API
  slug: planetscale-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Planetscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Planetscale secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Planetscale
provider_slug: planetscale
scheme_count: 2
schemes:
- description: Service token authentication. Use the format 'ServiceToken {token_id}:{token_value}' in the Authorization header.
  in: header
  name: serviceToken
  parameter: Authorization
  sources:
  - openapi/planetscale-platform-api-openapi.yml
  type: apiKey
- description: OAuth 2.0 bearer token authentication. Obtain tokens via the PlanetScale OAuth authorization code flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/planetscale-platform-api-openapi.yml
  type: http
slug: planetscale-authentication
source_filename: planetscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/planetscale-platform-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: serviceToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Service token authentication. Use the format 'ServiceToken {token_id}:{token_value}'\n    in the Authorization header.\n  sources:\n  - openapi/planetscale-platform-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token authentication. Obtain tokens via the PlanetScale OAuth\n    authorization code flow.\n  sources:\n  - openapi/planetscale-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/authentication/planetscale-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
