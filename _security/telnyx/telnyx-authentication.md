---
api_key_in: []
api_specs:
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Voice API
  slug: telnyx-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Messaging API
  slug: telnyx-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Numbers API
  slug: telnyx-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Verify API
  slug: telnyx-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Fax API
  slug: telnyx-fax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Wireless API
  slug: telnyx-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Networking API
  slug: telnyx-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx AI API
  slug: telnyx-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Billing & Reporting API
  slug: telnyx-billing-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Telnyx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Telnyx secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Telnyx
provider_slug: telnyx
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/telnyx-openapi.yml
  type: http
- description: OAuth 2.0 authentication for Telnyx API and MCP integrations
  flows:
  - authorizationUrl: https://api.telnyx.com/v2/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.telnyx.com/v2/oauth/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.telnyx.com/v2/oauth/token
  name: oauthClientAuth
  sources:
  - openapi/telnyx-openapi.yml
  type: oauth2
slug: telnyx-authentication
source_filename: telnyx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telnyx-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/telnyx-openapi.yml\n- name: oauthClientAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.telnyx.com/v2/oauth/authorize\n    tokenUrl: https://api.telnyx.com/v2/oauth/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://api.telnyx.com/v2/oauth/token\n    scopes: 1\n  description: OAuth 2.0 authentication for Telnyx API and MCP integrations\n  sources:\n  - openapi/telnyx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/authentication/telnyx-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Communications
- CPaaS
- Voice
- SMS
- IoT
---
