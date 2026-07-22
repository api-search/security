---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Stream Labs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Stream Labs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Stream Labs
provider_slug: stream-labs
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://streamlabs.com/api/v2.0/authorize
    flow: authorizationCode
    refresh: true
    tokenUrl: https://streamlabs.com/api/v2.0/token
  name: OAuth2
  notes: All endpoints require authentication. In v2.0 the access token cannot be passed as a query parameter; it must be sent in an Authorization Bearer header. Per-feature OAuth scopes gate each resource (see scopes/stream-labs-scopes.yml).
  type: oauth2
slug: stream-labs-authentication
source_filename: stream-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://dev.streamlabs.com/docs/oauth-2\ndocs: https://dev.streamlabs.com/docs/oauth-2\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  token_delivery: bearer-header-only\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://streamlabs.com/api/v2.0/authorize\n    tokenUrl: https://streamlabs.com/api/v2.0/token\n    refresh: true\n  notes: >-\n    All endpoints require authentication. In v2.0 the access token cannot be\n    passed as a query parameter; it must be sent in an Authorization Bearer\n    header. Per-feature OAuth scopes gate each resource (see\n    scopes/stream-labs-scopes.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stream-labs/refs/heads/main/authentication/stream-labs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Live Streaming
- Creator Economy
- Alerts
- Donations
- Loyalty Points
- Media Share
- OAuth
- Real-time
- Streaming Tools
---
