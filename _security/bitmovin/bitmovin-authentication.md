---
api_key_in:
- header
api_specs:
- filename: bitmovin-config-api-openapi.yml
  format: yaml
  label: Bitmovin Config API
  slug: bitmovin-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-config-api-openapi.yml
- filename: bitmovin-configurations-api-openapi.yml
  format: yaml
  label: Bitmovin Configurations API
  slug: bitmovin-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-configurations-api-openapi.yml
- filename: bitmovin-emails-api-openapi.yml
  format: yaml
  label: Bitmovin Emails API
  slug: bitmovin-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-emails-api-openapi.yml
- filename: bitmovin-encodings-api-openapi.yml
  format: yaml
  label: Bitmovin Encodings API
  slug: bitmovin-encodings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-encodings-api-openapi.yml
- filename: bitmovin-filters-api-openapi.yml
  format: yaml
  label: Bitmovin Filters API
  slug: bitmovin-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-filters-api-openapi.yml
- filename: bitmovin-infrastructure-api-openapi.yml
  format: yaml
  label: Bitmovin Infrastructure API
  slug: bitmovin-infrastructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-infrastructure-api-openapi.yml
- filename: bitmovin-inputs-api-openapi.yml
  format: yaml
  label: Bitmovin Inputs API
  slug: bitmovin-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-inputs-api-openapi.yml
- filename: bitmovin-live-api-openapi.yml
  format: yaml
  label: Bitmovin Live API
  slug: bitmovin-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-live-api-openapi.yml
- filename: bitmovin-manifests-api-openapi.yml
  format: yaml
  label: Bitmovin Manifests API
  slug: bitmovin-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-manifests-api-openapi.yml
- filename: bitmovin-notifications-api-openapi.yml
  format: yaml
  label: Bitmovin Notifications API
  slug: bitmovin-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-notifications-api-openapi.yml
- filename: bitmovin-outputs-api-openapi.yml
  format: yaml
  label: Bitmovin Outputs API
  slug: bitmovin-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-outputs-api-openapi.yml
- filename: bitmovin-search-api-openapi.yml
  format: yaml
  label: Bitmovin Search API
  slug: bitmovin-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-search-api-openapi.yml
- filename: bitmovin-signing-keys-api-openapi.yml
  format: yaml
  label: Bitmovin Signing-keys API
  slug: bitmovin-signing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-signing-keys-api-openapi.yml
- filename: bitmovin-templates-api-openapi.yml
  format: yaml
  label: Bitmovin Templates API
  slug: bitmovin-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-templates-api-openapi.yml
- filename: bitmovin-video-api-openapi.yml
  format: yaml
  label: Bitmovin Video API
  slug: bitmovin-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-video-api-openapi.yml
- filename: bitmovin-webhooks-api-openapi.yml
  format: yaml
  label: Bitmovin Webhooks API
  slug: bitmovin-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/openapi/bitmovin-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bitmovin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitmovin secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bitmovin
provider_slug: bitmovin
scheme_count: 2
schemes:
- description: Your Bitmovin API key
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/bitmovin-encoding-api-openapi.yml
  - openapi/bitmovin-platform-openapi.yml
  type: apiKey
- description: Your Bitmovin account organization
  in: header
  name: TenantOrgId
  parameter: X-Tenant-Org-Id
  sources:
  - openapi/bitmovin-encoding-api-openapi.yml
  - openapi/bitmovin-platform-openapi.yml
  type: apiKey
slug: bitmovin-authentication
source_filename: bitmovin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitmovin-encoding-api-openapi.yml, openapi/bitmovin-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Your Bitmovin API key\n  sources:\n  - openapi/bitmovin-encoding-api-openapi.yml\n  - openapi/bitmovin-platform-openapi.yml\n- name: TenantOrgId\n  type: apiKey\n  in: header\n  parameter: X-Tenant-Org-Id\n  description: Your Bitmovin account organization\n  sources:\n  - openapi/bitmovin-encoding-api-openapi.yml\n  - openapi/bitmovin-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitmovin/refs/heads/main/authentication/bitmovin-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Video
- Encoding
- Streaming
- Live Streaming
- VOD
- Adaptive Bitrate
- HLS
- DASH
- DRM
- Player
- Analytics
- Media
- Cloud
---
