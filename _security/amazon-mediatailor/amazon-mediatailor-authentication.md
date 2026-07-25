---
api_key_in:
- header
api_specs:
- filename: amazon-mediatailor-alerts-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Alerts#resourceArn API
  slug: amazon-mediatailor-alerts-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-alerts-resourcearn-api-openapi.yml
- filename: amazon-mediatailor-channel-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Channel API
  slug: amazon-mediatailor-channel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-channel-api-openapi.yml
- filename: amazon-mediatailor-channels-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Channels API
  slug: amazon-mediatailor-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-channels-api-openapi.yml
- filename: amazon-mediatailor-configurelogs-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor ConfigureLogs API
  slug: amazon-mediatailor-configurelogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-configurelogs-api-openapi.yml
- filename: amazon-mediatailor-playbackconfiguration-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor PlaybackConfiguration API
  slug: amazon-mediatailor-playbackconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-playbackconfiguration-api-openapi.yml
- filename: amazon-mediatailor-playbackconfigurations-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor PlaybackConfigurations API
  slug: amazon-mediatailor-playbackconfigurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-playbackconfigurations-api-openapi.yml
- filename: amazon-mediatailor-prefetchschedule-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor PrefetchSchedule API
  slug: amazon-mediatailor-prefetchschedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-prefetchschedule-api-openapi.yml
- filename: amazon-mediatailor-sourcelocation-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor SourceLocation API
  slug: amazon-mediatailor-sourcelocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-sourcelocation-api-openapi.yml
- filename: amazon-mediatailor-sourcelocations-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor SourceLocations API
  slug: amazon-mediatailor-sourcelocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-sourcelocations-api-openapi.yml
- filename: amazon-mediatailor-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Tags API
  slug: amazon-mediatailor-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Mediatailor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MediaTailor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mediatailor-openapi-original.yml
  type: apiKey
slug: amazon-mediatailor-authentication
source_filename: amazon-mediatailor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mediatailor-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mediatailor-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/authentication/amazon-mediatailor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
