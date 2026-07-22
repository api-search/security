---
api_key_in: []
api_specs:
- filename: paxos-v2-openapi-original.json
  format: json
  label: Paxos API v2
  slug: paxos-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/openapi/paxos-v2-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Paxos Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Paxos secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Paxos
provider_slug: paxos
scheme_count: 1
schemes:
- description: 'Paxos APIs use [OAuth 2](https://tools.ietf.org/html/rfc6749) with the [client credentials](https://tools.ietf.org/html/rfc6749#section-4.4) grant flow.


    **Token URLs:**

    - Production: https://oauth.paxos.com/oauth2/token

    - Sandbox: https://oauth.sandbox.paxos.com/oauth2/token


    Learn more in the [API credentials guide →](https://docs.paxos.com/developer/credentials)'
  flows:
  - flow: clientCredentials
    scopes: 36
    tokenUrl: https://oauth.paxos.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/paxos-v2-openapi-original.json
  type: oauth2
slug: paxos-authentication
source_filename: paxos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/paxos-v2-openapi-original.json\ndocs: https://docs.paxos.com/api-reference/introduction\noidc_discovery: well-known/paxos-openid-configuration.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.paxos.com/oauth2/token\n    scopes: 36\n  description: |-\n    Paxos APIs use [OAuth 2](https://tools.ietf.org/html/rfc6749) with the [client credentials](https://tools.ietf.org/html/rfc6749#section-4.4) grant flow.\n\n    **Token URLs:**\n    - Production: https://oauth.paxos.com/oauth2/token\n    - Sandbox: https://oauth.sandbox.paxos.com/oauth2/token\n\n    Learn more in the [API credentials guide →](https://docs.paxos.com/developer/credentials)\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/authentication/paxos-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Stablecoins
- Cryptocurrency
- Payments
- Crypto Brokerage
- Trading
- Custody
- Blockchain
- Financial Services
- Digital Assets
---
