---
api_key_in:
- query
api_specs:
- filename: bridge-mls-agents-api-openapi.yml
  format: yaml
  label: Bridge Agents API
  slug: bridge-mls-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-agents-api-openapi.yml
- filename: bridge-mls-listings-api-openapi.yml
  format: yaml
  label: Bridge Listings API
  slug: bridge-mls-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-listings-api-openapi.yml
- filename: bridge-mls-media-api-openapi.yml
  format: yaml
  label: Bridge Media API
  slug: bridge-mls-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-media-api-openapi.yml
- filename: bridge-mls-member-api-openapi.yml
  format: yaml
  label: Bridge Member API
  slug: bridge-mls-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-member-api-openapi.yml
- filename: bridge-mls-metadata-api-openapi.yml
  format: yaml
  label: Bridge Metadata API
  slug: bridge-mls-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-metadata-api-openapi.yml
- filename: bridge-mls-office-api-openapi.yml
  format: yaml
  label: Bridge Office API
  slug: bridge-mls-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-office-api-openapi.yml
- filename: bridge-mls-offices-api-openapi.yml
  format: yaml
  label: Bridge Offices API
  slug: bridge-mls-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-offices-api-openapi.yml
- filename: bridge-mls-openhouse-api-openapi.yml
  format: yaml
  label: Bridge OpenHouse API
  slug: bridge-mls-openhouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-openhouse-api-openapi.yml
- filename: bridge-mls-openhouses-api-openapi.yml
  format: yaml
  label: Bridge OpenHouses API
  slug: bridge-mls-openhouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-openhouses-api-openapi.yml
- filename: bridge-mls-property-api-openapi.yml
  format: yaml
  label: Bridge Property API
  slug: bridge-mls-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-property-api-openapi.yml
- filename: bridge-mls-webhooks-api-openapi.yml
  format: yaml
  label: Bridge Webhooks API
  slug: bridge-mls-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bridge Mls Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bridge secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bridge
provider_slug: bridge-mls
scheme_count: 2
schemes:
- bearerFormat: opaque
  description: '`Authorization: Bearer {access_token}` issued by Bridge per dataset.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/bridge-reso-web-api-openapi.yml
  type: http
- description: Per-dataset access token passed as a query parameter.
  in: query
  name: AccessToken
  parameter: access_token
  sources:
  - openapi/bridge-reso-web-api-openapi.yml
  - openapi/bridge-web-api-openapi.yml
  - openapi/bridge-webhooks-api-openapi.yml
  type: apiKey
slug: bridge-mls-authentication
source_filename: bridge-mls-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bridge-reso-web-api-openapi.yml, openapi/bridge-web-api-openapi.yml, openapi/bridge-webhooks-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  description: '`Authorization: Bearer {access_token}` issued by Bridge per dataset.'\n  sources:\n  - openapi/bridge-reso-web-api-openapi.yml\n- name: AccessToken\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: Per-dataset access token passed as a query parameter.\n  sources:\n  - openapi/bridge-reso-web-api-openapi.yml\n  - openapi/bridge-web-api-openapi.yml\n  - openapi/bridge-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/authentication/bridge-mls-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Real-Estate
- MLS
- RESO
- Listings
- Property Data
- Brokers
- Data Distribution
---
