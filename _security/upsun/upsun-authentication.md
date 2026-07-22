---
api_key_in: []
api_specs:
- filename: upsun-openapi-original.json
  format: json
  label: Upsun REST API
  slug: upsun-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upsun/refs/heads/main/openapi/upsun-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Upsun Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Upsun secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Upsun
provider_slug: upsun
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://auth.api.platform.sh/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.api.platform.sh/oauth2/token
  name: OAuth2
  sources:
  - openapi/upsun-openapi-original.json
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://auth.api.platform.sh/oauth2/token
  name: OAuth2Admin
  sources:
  - openapi/upsun-openapi-original.json
  type: oauth2
slug: upsun-authentication
source_filename: upsun-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/upsun-openapi-original.json\ndocs: https://developer.upsun.com/api/rest/authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  api_token_exchange: true\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.api.platform.sh/oauth2/authorize\n    tokenUrl: https://auth.api.platform.sh/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/upsun-openapi-original.json\n- name: OAuth2Admin\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.api.platform.sh/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/upsun-openapi-original.json\ntoken_exchange:\n  description: >-\n    The Upsun REST API uses OAuth2 bearer tokens. Users create an API token in\n    the Console, then exchange it for a short-lived access token via\n    grant_type=api_token at https://auth.upsun.com/oauth2/token\
  \ (HTTP basic\n    user platform-api-user). The bearer access token expires in 900 seconds\n    (15 minutes); clients re-exchange on 401 Unauthorized. All API requests go\n    to https://api.upsun.com.\n  exchange_endpoint: https://auth.upsun.com/oauth2/token\n  grant_type: api_token\n  token_type: bearer\n  expires_in_seconds: 900\noidc_discovery:\n  url: https://auth.upsun.com/.well-known/openid-configuration\n  grant_types_supported: [authorization_code, client_credentials]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg: ES256\n  resource_indicators_supported: true\nmfa_docs: https://developer.upsun.com/docs/administration/security/mfa\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upsun/refs/heads/main/authentication/upsun-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Infrastructure Saas
- Cloud
- PaaS
- Hosting
- Deployment
- DevOps
- Containers
- Observability
---
