---
api_key_in:
- header
api_specs:
- filename: cisco-catalyst-center-aaaservices-openapi.yml
  format: yaml
  label: Cisco Catalyst Center Assurance & Intent API
  slug: cisco-catalyst-center-assurance-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-center/refs/heads/main/openapi/cisco-catalyst-center-aaaservices-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cisco Catalyst Center Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Catalyst Center secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cisco Catalyst Center
provider_slug: cisco-catalyst-center
scheme_count: 2
schemes:
- description: Base64-encoded USERNAME:PASSWORD sent in the Authorization header to the token endpoint over HTTPS. The response body carries the token. Cisco also documents a CSRO-AES-256 AES-key-encryption variant for the token operation.
  name: basicAuthTokenExchange
  scheme: basic
  sources:
  - https://developer.cisco.com/docs/catalyst-center/authentication/
  token_endpoint: POST https://{catalyst-center-host}/dna/system/api/v1/auth/token
  type: http
- description: Opaque bearer token returned by the token endpoint; required on every subsequent Intent, data and system API call. Lifetime is 60 minutes. An expired or missing token returns 401 UNAUTHORIZED and the client must re-authenticate.
  in: header
  name: xAuthToken
  parameter_name: X-Auth-Token
  sources:
  - https://developer.cisco.com/docs/catalyst-center/authentication/
  token_lifetime_minutes: 60
  type: apiKey
slug: cisco-catalyst-center-authentication
source_filename: cisco-catalyst-center-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://developer.cisco.com/docs/catalyst-center/authentication/\ndocs:\n- https://developer.cisco.com/docs/catalyst-center/authentication/\n- https://developer.cisco.com/docs/catalyst-center/authentication-api/\nnote: 'None of the 27 published OpenAPI documents declares a components.securitySchemes block, so this profile is authored\n  from Cisco''s own authentication documentation rather than derived from the specs. That gap is itself a finding: an agent\n  reading only the published contracts would not learn how to authenticate.'\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: exchange HTTP Basic credentials for a short-lived opaque token, then send that token in a custom header\nschemes:\n- name: basicAuthTokenExchange\n  type: http\n  scheme: basic\n  token_endpoint: POST https://{catalyst-center-host}/dna/system/api/v1/auth/token\n  description: Base64-encoded USERNAME:PASSWORD\
  \ sent in the Authorization header to the token endpoint over HTTPS. The response\n    body carries the token. Cisco also documents a CSRO-AES-256 AES-key-encryption variant for the token operation.\n  sources:\n  - https://developer.cisco.com/docs/catalyst-center/authentication/\n- name: xAuthToken\n  type: apiKey\n  in: header\n  parameter_name: X-Auth-Token\n  description: Opaque bearer token returned by the token endpoint; required on every subsequent Intent, data and system\n    API call. Lifetime is 60 minutes. An expired or missing token returns 401 UNAUTHORIZED and the client must re-authenticate.\n  token_lifetime_minutes: 60\n  sources:\n  - https://developer.cisco.com/docs/catalyst-center/authentication/\nauthorization:\n  model: Catalyst Center role-based access control on the platform account\n  note: 'Permissions are those of the Catalyst Center user whose credentials were exchanged for the token. There is no OAuth\n    2.0 authorization server, no scope vocabulary and no\
  \ token-scoping mechanism, so scopes/ is intentionally absent from\n    this repo. Cisco''s own MCP README makes the consequence explicit: the server \"does not add an authorization layer or\n    enforce read-only access\" and executes tools with the configured account''s permissions.'\nsandbox_credentials: sandbox/cisco-catalyst-center-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-center/refs/heads/main/authentication/cisco-catalyst-center-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Network Automation
- Intent-Based Networking
- Networking
- Assurance
- Enterprise
- Campus
- Wireless
- SD-Access
- Network Management
- Observability
- Telemetry
- MCP
- Agent Native
- Cisco
---
