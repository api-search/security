---
api_key_in:
- header
api_specs:
- filename: vessel-accounts-api-openapi.yml
  format: yaml
  label: Vessel Accounts API
  slug: vessel-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-accounts-api-openapi.yml
- filename: vessel-authentication-api-openapi.yml
  format: yaml
  label: Vessel Authentication API
  slug: vessel-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-authentication-api-openapi.yml
- filename: vessel-connections-api-openapi.yml
  format: yaml
  label: Vessel Connections API
  slug: vessel-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-connections-api-openapi.yml
- filename: vessel-contacts-api-openapi.yml
  format: yaml
  label: Vessel Contacts API
  slug: vessel-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-contacts-api-openapi.yml
- filename: vessel-deals-api-openapi.yml
  format: yaml
  label: Vessel Deals API
  slug: vessel-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-deals-api-openapi.yml
- filename: vessel-engagement-unifications-api-openapi.yml
  format: yaml
  label: Vessel Engagement Unifications API
  slug: vessel-engagement-unifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-engagement-unifications-api-openapi.yml
- filename: vessel-integrations-api-openapi.yml
  format: yaml
  label: Vessel Integrations API
  slug: vessel-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-integrations-api-openapi.yml
- filename: vessel-leads-api-openapi.yml
  format: yaml
  label: Vessel Leads API
  slug: vessel-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-leads-api-openapi.yml
- filename: vessel-notes-api-openapi.yml
  format: yaml
  label: Vessel Notes API
  slug: vessel-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-notes-api-openapi.yml
- filename: vessel-passthrough-api-openapi.yml
  format: yaml
  label: Vessel Passthrough API
  slug: vessel-passthrough-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-passthrough-api-openapi.yml
- filename: vessel-tasks-api-openapi.yml
  format: yaml
  label: Vessel Tasks API
  slug: vessel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-tasks-api-openapi.yml
- filename: vessel-users-api-openapi.yml
  format: yaml
  label: Vessel Users API
  slug: vessel-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-users-api-openapi.yml
- filename: vessel-webhooks-api-openapi.yml
  format: yaml
  label: Vessel Webhooks API
  slug: vessel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vessel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vessel secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vessel
provider_slug: vessel
scheme_count: 4
schemes:
- description: Your Vessel API token for server-side authentication
  in: header
  name: apiToken
  parameter: vessel-api-token
  sources:
  - openapi/vessel-crm-openapi.yml
  type: apiKey
- description: Your Vessel API token for server-side authentication
  in: header
  name: apiToken
  parameter: x-vessel-api-token
  sources:
  - openapi/vessel-platform-openapi.yml
  type: apiKey
- description: User connection access token for user-scoped API calls
  in: header
  name: accessToken
  parameter: x-vessel-access-token
  sources:
  - openapi/vessel-platform-openapi.yml
  type: apiKey
- description: Temporary session token from the auth flow
  in: header
  name: sessionToken
  parameter: x-vessel-session-token
  sources:
  - openapi/vessel-platform-openapi.yml
  type: apiKey
slug: vessel-authentication
source_filename: vessel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vessel-crm-openapi.yml, openapi/vessel-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: vessel-api-token\n  description: Your Vessel API token for server-side authentication\n  sources:\n  - openapi/vessel-crm-openapi.yml\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: x-vessel-api-token\n  description: Your Vessel API token for server-side authentication\n  sources:\n  - openapi/vessel-platform-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: x-vessel-access-token\n  description: User connection access token for user-scoped API calls\n  sources:\n  - openapi/vessel-platform-openapi.yml\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: x-vessel-session-token\n  description: Temporary session token from the auth flow\n  sources:\n  - openapi/vessel-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/authentication/vessel-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- CRM
- Embedded Integrations
- GTM
- Integrations
- iPaaS
- Sales Engagement
- Unified API
---
