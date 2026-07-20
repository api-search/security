---
api_key_in: []
api_specs:
- filename: hopae-inc-hconnect-openapi-original.json
  format: json
  label: Hopae hConnect API
  slug: hopae-inc-hconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopae-inc/refs/heads/main/openapi/hopae-inc-hconnect-openapi-original.json
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hopae Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hopae, Inc. secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hopae, Inc.
provider_slug: hopae-inc
scheme_count: 2
schemes:
- description: 'Basic authentication using clientId and clientSecret. For direct API calls, format the Authorization header as `Authorization: Basic <base64(clientId:clientSecret)>`. In the Mintlify playground, enter the clientId and clientSecret in the Basic Auth panel and the header is generated automatically.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/hopae-inc-hconnect-openapi-original.json
  type: http
- bearerFormat: API Key
  description: 'Workspace API key authentication. Pass your workspace API key as `Authorization: Bearer [example key]`.'
  name: workspaceApiKey
  scheme: bearer
  sources:
  - openapi/hopae-inc-hconnect-openapi-original.json
  type: http
slug: hopae-inc-authentication
source_filename: hopae-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hopae-inc-hconnect-openapi-original.json\ndocs: https://docs.hopae.com/api-reference/authentication\nnote: >-\n  hConnect exposes two auth surfaces. Workspace API (managing Apps/Workflows/Providers/\n  Activation/Production Tests) uses HTTP Bearer with a workspace key\n  (sk_workspace_test_... / sk_workspace_prod_...). App API (/verifications, /userinfo)\n  uses HTTP Basic with the App's clientId:clientSecret (returned once from POST /v1/apps).\n  A separate OIDC OP surface (connect.hopae.com) handles browser sign-in — see\n  scopes/hopae-inc-scopes.yml. Console endpoints also accept a Clerk-issued JWT bearer.\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Basic authentication using clientId and clientSecret. For direct API calls,\n    format the Authorization header as `Authorization: Basic <base64(clientId:clientSecret)>`.\n    In the Mintlify\
  \ playground, enter the clientId and clientSecret in the Basic Auth panel\n    and the header is generated automatically.'\n  sources:\n  - openapi/hopae-inc-hconnect-openapi-original.json\n- name: workspaceApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'Workspace API key authentication. Pass your workspace API key as `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/hopae-inc-hconnect-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopae-inc/refs/heads/main/authentication/hopae-inc-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Company
- Identity
- Identity Verification
- Digital Identity
- eID
- Verifiable Credentials
- Authentication
- OpenID Connect
- eIDAS
- KYC
---
