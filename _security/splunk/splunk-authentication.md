---
api_key_in:
- header
api_specs:
- filename: splunk-enterprise-rest-api.yml
  format: yaml
  label: Splunk Enterprise REST API
  slug: splunk-enterprise-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/openapi/splunk-enterprise-rest-api.yml
- filename: openapi.json
  format: json
  label: Splunk Cloud ACS OpenAPI Specification
  slug: splunk-cloud-admin-config-service-openapi
  spec_type: OpenAPI
  url: https://admin.splunk.com/service/info/specs/v2/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Splunk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Splunk secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Splunk
provider_slug: splunk
scheme_count: 3
schemes:
- description: Splunk authentication token. Obtain a session key by authenticating to /services/auth/login or use a pre-configured bearer token from Settings > Tokens in Splunk Web.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/splunk-enterprise-rest-api.yml
  type: http
- description: HTTP Basic authentication with a valid Splunk username and password. The credentials are sent as a Base64-encoded string in the Authorization header.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/splunk-enterprise-rest-api.yml
  type: http
- description: HTTP Event Collector token. Send as "Splunk <token>" in the Authorization header. Tokens are configured in Splunk Web under Settings > Data Inputs > HTTP Event Collector.
  in: header
  name: HecToken
  parameter: Authorization
  sources:
  - openapi/splunk-enterprise-rest-api.yml
  type: apiKey
slug: splunk-authentication
source_filename: splunk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/splunk-enterprise-rest-api.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Splunk authentication token. Obtain a session key by authenticating to /services/auth/login\n    or use a pre-configured bearer token from Settings > Tokens in Splunk Web.\n  sources:\n  - openapi/splunk-enterprise-rest-api.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with a valid Splunk username and password. The credentials\n    are sent as a Base64-encoded string in the Authorization header.\n  sources:\n  - openapi/splunk-enterprise-rest-api.yml\n- name: HecToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HTTP Event Collector token. Send as \"Splunk <token>\" in the Authorization header.\n    Tokens are configured in Splunk Web under Settings > Data Inputs >\
  \ HTTP Event Collector.\n  sources:\n  - openapi/splunk-enterprise-rest-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/authentication/splunk-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Analytics
- Data Analysis
- Logging
- Machine Data
- Monitoring
- Observability
- Platform
- Security
- SIEM
---
