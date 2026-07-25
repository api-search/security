---
api_key_in: []
api_specs:
- filename: segment-pixel-tracking-api-openapi.yml
  format: yaml
  label: Segment Pixel Tracking API
  slug: pixel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-pixel-tracking-api-openapi.yml
- filename: segment-alias-api-openapi.yml
  format: yaml
  label: segment Alias API
  slug: segment-alias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-alias-api-openapi.yml
- filename: segment-batch-api-openapi.yml
  format: yaml
  label: segment Batch API
  slug: segment-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-batch-api-openapi.yml
- filename: segment-catalog-api-openapi.yml
  format: yaml
  label: segment Catalog API
  slug: segment-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-catalog-api-openapi.yml
- filename: segment-destinations-api-openapi.yml
  format: yaml
  label: segment Destinations API
  slug: segment-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-destinations-api-openapi.yml
- filename: segment-events-api-openapi.yml
  format: yaml
  label: segment Events API
  slug: segment-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-events-api-openapi.yml
- filename: segment-external-ids-api-openapi.yml
  format: yaml
  label: segment External IDs API
  slug: segment-external-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-external-ids-api-openapi.yml
- filename: segment-functions-api-openapi.yml
  format: yaml
  label: segment Functions API
  slug: segment-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-functions-api-openapi.yml
- filename: segment-group-api-openapi.yml
  format: yaml
  label: segment Group API
  slug: segment-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-group-api-openapi.yml
- filename: segment-identify-api-openapi.yml
  format: yaml
  label: segment Identify API
  slug: segment-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-identify-api-openapi.yml
- filename: segment-labels-api-openapi.yml
  format: yaml
  label: segment Labels API
  slug: segment-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-labels-api-openapi.yml
- filename: segment-links-api-openapi.yml
  format: yaml
  label: segment Links API
  slug: segment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-links-api-openapi.yml
- filename: segment-page-api-openapi.yml
  format: yaml
  label: segment Page API
  slug: segment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-page-api-openapi.yml
- filename: segment-profiles-api-openapi.yml
  format: yaml
  label: segment Profiles API
  slug: segment-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-profiles-api-openapi.yml
- filename: segment-regulations-api-openapi.yml
  format: yaml
  label: segment Regulations API
  slug: segment-regulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-regulations-api-openapi.yml
- filename: segment-screen-api-openapi.yml
  format: yaml
  label: segment Screen API
  slug: segment-screen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-screen-api-openapi.yml
- filename: segment-sources-api-openapi.yml
  format: yaml
  label: segment Sources API
  slug: segment-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-sources-api-openapi.yml
- filename: segment-track-api-openapi.yml
  format: yaml
  label: segment Track API
  slug: segment-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-track-api-openapi.yml
- filename: segment-tracking-plans-api-openapi.yml
  format: yaml
  label: segment Tracking Plans API
  slug: segment-tracking-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-tracking-plans-api-openapi.yml
- filename: segment-traits-api-openapi.yml
  format: yaml
  label: segment Traits API
  slug: segment-traits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-traits-api-openapi.yml
- filename: segment-transformations-api-openapi.yml
  format: yaml
  label: segment Transformations API
  slug: segment-transformations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-transformations-api-openapi.yml
- filename: segment-warehouses-api-openapi.yml
  format: yaml
  label: segment Warehouses API
  slug: segment-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-warehouses-api-openapi.yml
- filename: segment-workspaces-api-openapi.yml
  format: yaml
  label: segment Workspaces API
  slug: segment-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/openapi/segment-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Segment Authentication
name_suffix: Authentication
oauth_flows: []
overview: segment secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: segment
provider_slug: segment
scheme_count: 2
schemes:
- description: Segment Config API access token. Note that as of early 2024, Segment has stopped issuing new Config API tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/segment-config-api-openapi.yml
  - openapi/segment-public-api-openapi.yml
  type: http
- description: HTTP Basic authentication using the source write key as the username and an empty password. The write key is found in the Segment source settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/segment-http-tracking-api-openapi.yml
  - openapi/segment-profile-api-openapi.yml
  type: http
slug: segment-authentication
source_filename: segment-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/segment-config-api-openapi.yml, openapi/segment-http-tracking-api-openapi.yml,\n  openapi/segment-profile-api-openapi.yml, openapi/segment-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Segment Config API access token. Note that as of early 2024, Segment has stopped\n    issuing new Config API tokens.\n  sources:\n  - openapi/segment-config-api-openapi.yml\n  - openapi/segment-public-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the source write key as the username and an empty\n    password. The write key is found in the Segment source settings.\n  sources:\n  - openapi/segment-http-tracking-api-openapi.yml\n  - openapi/segment-profile-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segment/refs/heads/main/authentication/segment-authentication.yml
summary_line: http · 2 schemes
tags: []
---
