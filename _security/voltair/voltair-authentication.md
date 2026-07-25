---
api_key_in:
- header
api_specs:
- filename: voltair-apikeys-api-openapi.yml
  format: yaml
  label: Voltair ApiKeys API
  slug: voltair-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-apikeys-api-openapi.yml
- filename: voltair-assets-api-openapi.yml
  format: yaml
  label: Voltair Assets API
  slug: voltair-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-assets-api-openapi.yml
- filename: voltair-clusters-api-openapi.yml
  format: yaml
  label: Voltair Clusters API
  slug: voltair-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-clusters-api-openapi.yml
- filename: voltair-clustervisits-api-openapi.yml
  format: yaml
  label: Voltair ClusterVisits API
  slug: voltair-clustervisits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-clustervisits-api-openapi.yml
- filename: voltair-events-api-openapi.yml
  format: yaml
  label: Voltair Events API
  slug: voltair-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-events-api-openapi.yml
- filename: voltair-identity-api-openapi.yml
  format: yaml
  label: Voltair Identity API
  slug: voltair-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-identity-api-openapi.yml
- filename: voltair-inspections-api-openapi.yml
  format: yaml
  label: Voltair Inspections API
  slug: voltair-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-inspections-api-openapi.yml
- filename: voltair-media-api-openapi.yml
  format: yaml
  label: Voltair Media API
  slug: voltair-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-media-api-openapi.yml
- filename: voltair-missions-api-openapi.yml
  format: yaml
  label: Voltair Missions API
  slug: voltair-missions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-missions-api-openapi.yml
- filename: voltair-organization-api-openapi.yml
  format: yaml
  label: Voltair Organization API
  slug: voltair-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-organization-api-openapi.yml
- filename: voltair-roles-api-openapi.yml
  format: yaml
  label: Voltair Roles API
  slug: voltair-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-roles-api-openapi.yml
- filename: voltair-sites-api-openapi.yml
  format: yaml
  label: Voltair Sites API
  slug: voltair-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-sites-api-openapi.yml
- filename: voltair-sitevisits-api-openapi.yml
  format: yaml
  label: Voltair SiteVisits API
  slug: voltair-sitevisits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-sitevisits-api-openapi.yml
- filename: voltair-transactions-api-openapi.yml
  format: yaml
  label: Voltair Transactions API
  slug: voltair-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-transactions-api-openapi.yml
- filename: voltair-users-api-openapi.yml
  format: yaml
  label: Voltair Users API
  slug: voltair-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-users-api-openapi.yml
- filename: voltair-webhooks-api-openapi.yml
  format: yaml
  label: Voltair Webhooks API
  slug: voltair-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Voltair Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voltair secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Voltair
provider_slug: voltair
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Cognito JWT access token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/voltair-api-openapi-original.yml
  type: http
- description: Organization-scoped API key
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/voltair-api-openapi-original.yml
  type: apiKey
slug: voltair-authentication
source_filename: voltair-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/voltair-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Cognito JWT access token\n  sources:\n  - openapi/voltair-api-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Organization-scoped API key\n  sources:\n  - openapi/voltair-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/authentication/voltair-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Drones
- Earth Observation
- Infrastructure Inspection
- Utilities
- Energy
- Robotics
- LiDAR
- Aerial Imagery
---
