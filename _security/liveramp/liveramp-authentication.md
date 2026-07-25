---
api_key_in: []
api_specs:
- filename: liveramp-deliveries-api-openapi.yml
  format: yaml
  label: LiveRamp Deliveries API
  slug: liveramp-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-deliveries-api-openapi.yml
- filename: liveramp-destination-integrations-api-openapi.yml
  format: yaml
  label: LiveRamp Destination Integrations API
  slug: liveramp-destination-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-destination-integrations-api-openapi.yml
- filename: liveramp-destinations-api-openapi.yml
  format: yaml
  label: LiveRamp Destinations API
  slug: liveramp-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-destinations-api-openapi.yml
- filename: liveramp-distribution-managers-api-openapi.yml
  format: yaml
  label: LiveRamp Distribution Managers API
  slug: liveramp-distribution-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-distribution-managers-api-openapi.yml
- filename: liveramp-integration-connections-api-openapi.yml
  format: yaml
  label: LiveRamp Integration Connections API
  slug: liveramp-integration-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-integration-connections-api-openapi.yml
- filename: liveramp-oauth-connections-api-openapi.yml
  format: yaml
  label: LiveRamp OAuth Connections API
  slug: liveramp-oauth-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-oauth-connections-api-openapi.yml
- filename: liveramp-segment-configurations-api-openapi.yml
  format: yaml
  label: LiveRamp Segment Configurations API
  slug: liveramp-segment-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-segment-configurations-api-openapi.yml
- filename: liveramp-segments-api-openapi.yml
  format: yaml
  label: LiveRamp Segments API
  slug: liveramp-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-segments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Liveramp Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiveRamp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LiveRamp
provider_slug: liveramp
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token obtained from the LiveRamp service account token URI; passed as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/liveramp-openapi.yml
  type: http
slug: liveramp-authentication
source_filename: liveramp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/liveramp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 access token obtained from the LiveRamp service account token URI;\n    passed as `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/liveramp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/authentication/liveramp-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Connectivity
- Identity Resolution
- Activation
- Clean Room
- Privacy
- AdTech
---
