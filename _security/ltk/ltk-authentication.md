---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ltk Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LTK secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LTK
provider_slug: ltk
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    note: Live token endpoint returns RFC 6749 errors (POST with no credentials -> HTTP 400 {"error":"invalid_client"}), confirming an OAuth2 client-authenticated token endpoint. Client credentials are issued through the gated rewardStyle Developer Portal (registration at https://api.rewardstyle.com/register).
    tokenUrl: https://api.rewardstyle.com/oauth/token
  name: OAuth2
  sources:
  - https://api.rewardstyle.com/oauth/token
  type: oauth2
slug: ltk-authentication
source_filename: ltk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.rewardstyle.com/\ndocs: https://api.rewardstyle.com/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  registration: gated\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.rewardstyle.com/oauth/token\n        note: >-\n          Live token endpoint returns RFC 6749 errors (POST with no\n          credentials -> HTTP 400 {\"error\":\"invalid_client\"}), confirming an\n          OAuth2 client-authenticated token endpoint. Client credentials are\n          issued through the gated rewardStyle Developer Portal\n          (registration at https://api.rewardstyle.com/register).\n    sources: [https://api.rewardstyle.com/oauth/token]\nnotes: >-\n  The rewardStyle Developer Portal (api.rewardstyle.com) is registration-gated;\n  the full API reference, OpenAPI/Swagger spec, and scope list are only visible\n  to approved partners after\
  \ login, so scopes could not be enumerated publicly.\n  The public, verifiable surface is the OAuth2 token endpoint behavior above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ltk/refs/heads/main/authentication/ltk-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Consumer
- Creator Commerce
- Affiliate
- E-Commerce
- Influencer Marketing
- Retail
- Shopping
---
