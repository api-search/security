---
api_key_in: []
api_specs:
- filename: nift-partners-openapi.yml
  format: yaml
  label: Nift Partners API
  slug: nift-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nift/refs/heads/main/openapi/nift-partners-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nift Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: NIFT secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: NIFT
provider_slug: nift
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials issued by Nift; token endpoint at /oauth/token.
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://www.gonift.com/oauth/token
  name: oauth2
  sources:
  - openapi/nift-partners-openapi.yml
  type: oauth2
slug: nift-authentication
source_filename: nift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nift-partners-openapi.yml\ndocs: https://github.com/nift-sdks/nift-flow-sdk-docs/blob/main/docs/sdk/customer-status-server.md\nnotes: >-\n  Server-side Partners API uses OAuth 2.0 client_credentials (client_id + client_secret\n  issued by Nift) posted to https://www.gonift.com/oauth/token; scopes read:customers /\n  write:customers gate access. Long-lived tokens (~1 year). Client-side SDKs (web/iOS/\n  Android/React Native) authenticate the gift flow with a Nift-issued clientId + partner\n  referralCode instead of an OAuth token.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.gonift.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 client credentials issued by Nift; token endpoint at /oauth/token.\n  sources:\n  - openapi/nift-partners-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nift/refs/heads/main/authentication/nift-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Marketing
- Gifting
- Customer Acquisition
- Loyalty
- Rewards
- SDK
- Partners
---
