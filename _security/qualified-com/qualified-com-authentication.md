---
api_key_in: []
api_specs:
- filename: qualified-com-enterprise-api-openapi.json
  format: json
  label: Qualified Enterprise API
  slug: qualified-com-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-enterprise-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Qualified Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qualified secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qualified
provider_slug: qualified-com
scheme_count: 1
schemes:
- bearerFormat: Token
  example_request: 'curl https://api.qualified.com/v2/leads -H "Authorization: Bearer YOUR_API_TOKEN"'
  header: Authorization
  in: header
  key_issuance: API keys are minted in the Qualified app with a specific set of named scopes. A key reaches only the endpoints its scopes allow.
  name: bearerToken
  scheme: bearer
  scopes_artifact: scopes/qualified-com-scopes.yml
  sources:
  - openapi/qualified-com-enterprise-api-openapi.json
  - https://app.qualified.com/docs/api
  type: http
  value_format: Bearer YOUR_API_TOKEN
slug: qualified-com-authentication
source_filename: qualified-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://app.qualified.com/docs/api\ndocs: https://app.qualified.com/docs/api\nderived_from: openapi/qualified-com-enterprise-api-openapi.json\napi: qualified-com-enterprise-api\nsummary:\n  types:\n  - http\n  model: bearer-token-with-named-scopes\n  self_serve: false\n  gate: >-\n    API access is a plan gate. \"Enterprise-Grade APIs\" first appear on the Enterprise\n    tier of https://www.qualified.com/pricing, and a 401 {\"code\":\"invalid_token\"} is\n    also returned when the API is simply not enabled for the team.\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: Token\n  in: header\n  header: Authorization\n  value_format: 'Bearer YOUR_API_TOKEN'\n  example_request: 'curl https://api.qualified.com/v2/leads -H \"Authorization: Bearer YOUR_API_TOKEN\"'\n  key_issuance: >-\n    API keys are minted in the Qualified app with a specific set of named scopes.\n    A key reaches only the endpoints\
  \ its scopes allow.\n  scopes_artifact: scopes/qualified-com-scopes.yml\n  sources:\n  - openapi/qualified-com-enterprise-api-openapi.json\n  - https://app.qualified.com/docs/api\nfailure_modes:\n- status: 401\n  body: '{\"code\": \"invalid_token\"}'\n  meaning: Missing or invalid token, or the API is not enabled for the team.\n- status: 403\n  body: '{\"code\": \"insufficient_scope\"}'\n  meaning: The token is valid but lacks the scope the endpoint requires.\nnot_supported:\n- oauth2 authorization flows (no /authorize or /token endpoint is published)\n- openIdConnect discovery (no /.well-known/openid-configuration is served on any host)\n- mutualTLS\n- basic auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/authentication/qualified-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Conversational Marketing
- Sales
- Marketing
- Artificial Intelligence
- AI Agents
- Lead Generation
- Customer Engagement
- Salesforce
- Analytics
---
