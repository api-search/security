---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-medialive-prod-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Prod API
  slug: amazon-medialive-prod-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-prod-api-openapi.yml
- filename: amazon-medialive-alerts-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Alerts API
  slug: amazon-medialive-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-alerts-api-openapi.yml
- filename: amazon-medialive-channelplacementgroups-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Channelplacementgroups API
  slug: amazon-medialive-channelplacementgroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-channelplacementgroups-api-openapi.yml
- filename: amazon-medialive-nodes-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Nodes API
  slug: amazon-medialive-nodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-nodes-api-openapi.yml
- filename: amazon-medialive-operations-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Operations API
  slug: amazon-medialive-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-operations-api-openapi.yml
- filename: amazon-medialive-programs-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Programs API
  slug: amazon-medialive-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-programs-api-openapi.yml
- filename: amazon-medialive-schedule-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Schedule API
  slug: amazon-medialive-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-schedule-api-openapi.yml
- filename: amazon-medialive-start-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Start API
  slug: amazon-medialive-start-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-start-api-openapi.yml
- filename: amazon-medialive-stop-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Stop API
  slug: amazon-medialive-stop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-stop-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Medialive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MediaLive secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-medialive-openapi-original.yml
  type: apiKey
slug: amazon-medialive-authentication
source_filename: amazon-medialive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-medialive-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-medialive-openapi-original.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-medialive/authentication/amazon-medialive-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Media Processing
- Media
---
