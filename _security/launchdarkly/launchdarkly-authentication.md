---
api_key_in:
- header
api_specs:
- filename: launchdarkly-rest-api-openapi.yml
  format: yaml
  label: LaunchDarkly REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/openapi/launchdarkly-rest-api-openapi.yml
- filename: launchdarkly-webhooks-asyncapi.yml
  format: yaml
  label: LaunchDarkly Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/asyncapi/launchdarkly-webhooks-asyncapi.yml
- filename: launchdarkly-relay-proxy-openapi.yml
  format: yaml
  label: LaunchDarkly Relay Proxy
  slug: relay-proxy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/openapi/launchdarkly-relay-proxy-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Launchdarkly Authentication
name_suffix: Authentication
oauth_flows: []
overview: launchdarkly secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: launchdarkly
provider_slug: launchdarkly
scheme_count: 2
schemes:
- description: Server-side SDK key for authenticating with the Relay Proxy.
  in: header
  name: sdkKeyAuth
  parameter: Authorization
  sources:
  - openapi/launchdarkly-relay-proxy-openapi.yml
  type: apiKey
- description: LaunchDarkly API access token. Create personal or service tokens in the LaunchDarkly dashboard under Account Settings.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/launchdarkly-rest-api-openapi.yml
  type: http
slug: launchdarkly-authentication
source_filename: launchdarkly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/launchdarkly-relay-proxy-openapi.yml, openapi/launchdarkly-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: sdkKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Server-side SDK key for authenticating with the Relay Proxy.\n  sources:\n  - openapi/launchdarkly-relay-proxy-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: LaunchDarkly API access token. Create personal or service tokens in the LaunchDarkly\n    dashboard under Account Settings.\n  sources:\n  - openapi/launchdarkly-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/authentication/launchdarkly-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
