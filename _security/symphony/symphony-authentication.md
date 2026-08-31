---
api_key_in:
- query
api_specs:
- filename: symphony-all-api-openapi.yml
  format: yaml
  label: Symphony All API
  slug: symphony-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-all-api-openapi.yml
- filename: symphony-app-api-openapi.yml
  format: yaml
  label: Symphony App API
  slug: symphony-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-app-api-openapi.yml
- filename: symphony-audittrail-api-openapi.yml
  format: yaml
  label: Symphony Audittrail API
  slug: symphony-audittrail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-audittrail-api-openapi.yml
- filename: symphony-authenticate-api-openapi.yml
  format: yaml
  label: Symphony Authenticate API
  slug: symphony-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-authenticate-api-openapi.yml
- filename: symphony-channelco-api-openapi.yml
  format: yaml
  label: Symphony Channelco API
  slug: symphony-channelco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-channelco-api-openapi.yml
- filename: symphony-datafeeds-api-openapi.yml
  format: yaml
  label: Symphony Datafeeds API
  slug: symphony-datafeeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-datafeeds-api-openapi.yml
- filename: symphony-dlp-api-openapi.yml
  format: yaml
  label: Symphony Dlp API
  slug: symphony-dlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-dlp-api-openapi.yml
- filename: symphony-events-api-openapi.yml
  format: yaml
  label: Symphony Events API
  slug: symphony-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-events-api-openapi.yml
- filename: symphony-groups-api-openapi.yml
  format: yaml
  label: Symphony Groups API
  slug: symphony-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-groups-api-openapi.yml
- filename: symphony-health-api-openapi.yml
  format: yaml
  label: Symphony Health API
  slug: symphony-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-health-api-openapi.yml
- filename: symphony-idm-api-openapi.yml
  format: yaml
  label: Symphony Idm API
  slug: symphony-idm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-idm-api-openapi.yml
- filename: symphony-info-api-openapi.yml
  format: yaml
  label: Symphony Info API
  slug: symphony-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-info-api-openapi.yml
- filename: symphony-logout-api-openapi.yml
  format: yaml
  label: Symphony Logout API
  slug: symphony-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-logout-api-openapi.yml
- filename: symphony-message-api-openapi.yml
  format: yaml
  label: Symphony Message API
  slug: symphony-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-message-api-openapi.yml
- filename: symphony-onboarding-api-openapi.yml
  format: yaml
  label: Symphony Onboarding API
  slug: symphony-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-onboarding-api-openapi.yml
- filename: symphony-pubkey-api-openapi.yml
  format: yaml
  label: Symphony Pubkey API
  slug: symphony-pubkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-pubkey-api-openapi.yml
- filename: symphony-signals-api-openapi.yml
  format: yaml
  label: Symphony Signals API
  slug: symphony-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-signals-api-openapi.yml
- filename: symphony-stream-api-openapi.yml
  format: yaml
  label: Symphony Stream API
  slug: symphony-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-stream-api-openapi.yml
- filename: symphony-types-api-openapi.yml
  format: yaml
  label: Symphony Types API
  slug: symphony-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-types-api-openapi.yml
- filename: symphony-util-api-openapi.yml
  format: yaml
  label: Symphony Util API
  slug: symphony-util-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-util-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Symphony Authentication
name_suffix: Authentication
oauth_flows: []
overview: Symphony secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Symphony
provider_slug: symphony
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: ExtApp JWT
  name: JwtAuth
  scheme: bearer
  sources:
  - openapi/community-connect-openapi-original.yml
  - openapi/pod-openapi-original.yml
  - openapi/profile-manager-openapi-original.yml
  - openapi/symphony-community-connect-api-openapi.yml
  type: http
- in: query
  name: ApiKeyAuth
  parameter: token
  sources:
  - openapi/community-connect-openapi-original.yml
  - openapi/symphony-community-connect-api-openapi.yml
  type: apiKey
slug: symphony-authentication
source_filename: symphony-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/community-connect-openapi-original.yml, openapi/pod-openapi-original.yml, openapi/profile-manager-openapi-original.yml,\n  openapi/symphony-community-connect-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: JwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: ExtApp JWT\n  sources:\n  - openapi/community-connect-openapi-original.yml\n  - openapi/pod-openapi-original.yml\n  - openapi/profile-manager-openapi-original.yml\n  - openapi/symphony-community-connect-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/community-connect-openapi-original.yml\n  - openapi/symphony-community-connect-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/authentication/symphony-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Collaboration
- Communications
- Financial-Services
- Messaging
- Secure Communication
---
