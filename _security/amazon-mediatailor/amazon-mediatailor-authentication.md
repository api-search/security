---
anonymous_access: false
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
- filename: amazon-mediatailor-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Tags API
  slug: amazon-mediatailor-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-tags-api-openapi.yml
- filename: amazon-mediatailor-configure-logs-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Configure Logs API
  slug: amazon-mediatailor-configure-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-configure-logs-api-openapi.yml
- filename: amazon-mediatailor-playback-configuration-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Playback Configuration API
  slug: amazon-mediatailor-playback-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-playback-configuration-api-openapi.yml
- filename: amazon-mediatailor-playback-configurations-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Playback Configurations API
  slug: amazon-mediatailor-playback-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-playback-configurations-api-openapi.yml
- filename: amazon-mediatailor-prefetch-schedule-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Prefetch Schedule API
  slug: amazon-mediatailor-prefetch-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-prefetch-schedule-api-openapi.yml
- filename: amazon-mediatailor-source-location-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Source Location API
  slug: amazon-mediatailor-source-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-source-location-api-openapi.yml
- filename: amazon-mediatailor-source-locations-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Source Locations API
  slug: amazon-mediatailor-source-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-source-locations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
