---
api_key_in:
- header
api_specs:
- filename: purplebricks-property-v1-openapi.yml
  format: yaml
  label: Purplebricks Property API
  slug: purplebricks-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-property-v1-openapi.yml
- filename: purplebricks-account-v1-openapi.yml
  format: yaml
  label: Purplebricks Account API
  slug: purplebricks-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-account-v1-openapi.yml
- filename: purplebricks-valuations-v1-openapi.yml
  format: yaml
  label: Purplebricks Valuations API
  slug: purplebricks-valuations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-valuations-v1-openapi.yml
- filename: purplebricks-viewings-v1-openapi.yml
  format: yaml
  label: Purplebricks Viewings API
  slug: purplebricks-viewings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-viewings-v1-openapi.yml
- filename: purplebricks-messaging-v1-openapi.yml
  format: yaml
  label: Purplebricks Messaging API
  slug: purplebricks-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-messaging-v1-openapi.yml
- filename: purplebricks-lettings-v1-openapi.yml
  format: yaml
  label: Purplebricks Lettings API
  slug: purplebricks-lettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-lettings-v1-openapi.yml
- filename: purplebricks-branch-v1-openapi.yml
  format: yaml
  label: Purplebricks Branch API
  slug: purplebricks-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-branch-v1-openapi.yml
- filename: purplebricks-communications-v1-openapi.yml
  format: yaml
  label: Purplebricks Communications API
  slug: purplebricks-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-communications-v1-openapi.yml
- filename: purplebricks-conveyancing-v1-openapi.yml
  format: yaml
  label: Purplebricks Conveyancing API
  slug: purplebricks-conveyancing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-conveyancing-v1-openapi.yml
- filename: purplebricks-agent-v1-openapi.yml
  format: yaml
  label: Purplebricks Agent API
  slug: purplebricks-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-agent-v1-openapi.yml
- filename: purplebricks-feedback-v1-openapi.yml
  format: yaml
  label: Purplebricks Feedback API
  slug: purplebricks-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-feedback-v1-openapi.yml
- filename: purplebricks-workflow-v1-openapi.yml
  format: yaml
  label: Purplebricks Workflow API
  slug: purplebricks-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-workflow-v1-openapi.yml
- filename: purplebricks-outlook-v1-openapi.yml
  format: yaml
  label: Purplebricks Outlook Sync API
  slug: purplebricks-outlook-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/openapi/purplebricks-outlook-v1-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Purplebricks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Purplebricks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Purplebricks
provider_slug: purplebricks
scheme_count: 1
schemes:
- description: Authorization header using Bearer scheme
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/purplebricks-account-v1-openapi.yml
  - openapi/purplebricks-agent-v1-openapi.yml
  - openapi/purplebricks-branch-v1-openapi.yml
  - openapi/purplebricks-communications-v1-openapi.yml
  - openapi/purplebricks-conveyancing-v1-openapi.yml
  - openapi/purplebricks-feedback-v1-openapi.yml
  - openapi/purplebricks-lettings-v1-openapi.yml
  - openapi/purplebricks-messaging-v1-openapi.yml
  - openapi/purplebricks-messaging-v2-openapi.yml
  - openapi/purplebricks-outlook-v1-openapi.yml
  - openapi/purplebricks-property-v1-openapi.yml
  - openapi/purplebricks-property-v2-openapi.yml
  - openapi/purplebricks-valuations-v1-openapi.yml
  - openapi/purplebricks-valuations-v2-openapi.yml
  - openapi/purplebricks-viewings-v1-openapi.yml
  - openapi/purplebricks-workflow-v1-openapi.yml
  type: apiKey
slug: purplebricks-authentication
source_filename: purplebricks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/purplebricks-account-v1-openapi.yml, openapi/purplebricks-agent-v1-openapi.yml,\n  openapi/purplebricks-branch-v1-openapi.yml, openapi/purplebricks-communications-v1-openapi.yml,\n  openapi/purplebricks-conveyancing-v1-openapi.yml, openapi/purplebricks-feedback-v1-openapi.yml,\n  openapi/purplebricks-lettings-v1-openapi.yml, openapi/purplebricks-messaging-v1-openapi.yml,\n  openapi/purplebricks-messaging-v2-openapi.yml, openapi/purplebricks-outlook-v1-openapi.yml,\n  openapi/purplebricks-property-v1-openapi.yml, openapi/purplebricks-property-v2-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization header using Bearer scheme\n  sources:\n  - openapi/purplebricks-account-v1-openapi.yml\n  - openapi/purplebricks-agent-v1-openapi.yml\n  - openapi/purplebricks-branch-v1-openapi.yml\n  -\
  \ openapi/purplebricks-communications-v1-openapi.yml\n  - openapi/purplebricks-conveyancing-v1-openapi.yml\n  - openapi/purplebricks-feedback-v1-openapi.yml\n  - openapi/purplebricks-lettings-v1-openapi.yml\n  - openapi/purplebricks-messaging-v1-openapi.yml\n  - openapi/purplebricks-messaging-v2-openapi.yml\n  - openapi/purplebricks-outlook-v1-openapi.yml\n  - openapi/purplebricks-property-v1-openapi.yml\n  - openapi/purplebricks-property-v2-openapi.yml\n  - openapi/purplebricks-valuations-v1-openapi.yml\n  - openapi/purplebricks-valuations-v2-openapi.yml\n  - openapi/purplebricks-viewings-v1-openapi.yml\n  - openapi/purplebricks-workflow-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purplebricks/refs/heads/main/authentication/purplebricks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Real Estate
- United Kingdom
- Property Listings
- Online Estate Agency
- Rentals
- Lettings
- PropTech
- Mortgage
- Conveyancing
- Land Registry
- OpenAPI
- Microservices
- Swagger
- Azure
---
