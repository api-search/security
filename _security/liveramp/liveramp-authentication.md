---
api_key_in: []
api_specs:
- filename: liveramp-activation-api-openapi.yml
  format: yaml
  label: LiveRamp Activation API
  slug: activation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-activation-api-openapi.yml
- filename: liveramp-clean-room-api-openapi.yml
  format: yaml
  label: LiveRamp Clean Room API
  slug: clean-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-clean-room-api-openapi.yml
- filename: liveramp-privacy-api-openapi.yml
  format: yaml
  label: LiveRamp Privacy API
  slug: privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-privacy-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Liveramp Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
overview: LiveRamp secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and clientCredentials flow(s).
provider_name: LiveRamp
provider_slug: liveramp
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.habu.com/v1/oauth/token
  name: application
  sources:
  - openapi/liveramp-clean-room-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/liveramp-privacy-api-openapi.yml
  type: http
- description: 'Authorization: Bearer <access_token>, where the access token comes from the LiveRamp service account token service. Documented for the Activation API, which publishes no securitySchemes block in its own OpenAPI.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token
  type: http
slug: liveramp-authentication
source_filename: liveramp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/liveramp-activation-api-openapi.yml, openapi/liveramp-clean-room-api-openapi.yml,\n  openapi/liveramp-privacy-api-openapi.yml\ndocs: https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token\nnotes: >-\n  LiveRamp issues API credentials as \"Service Accounts\" that are provisioned by a LiveRamp\n  representative — there is no self-serve key issuance. The Activation, AbiliTec, RampID and\n  Privacy APIs share one OAuth 2.0 token service at serviceaccounts.liveramp.com; the Clean Room\n  API (the former Habu platform, acquired by LiveRamp) runs its own client-credentials token\n  endpoint on api.habu.com.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\n  - clientCredentials\n  api_key_in: []\ntoken_services:\n- name: LiveRamp Service Accounts\n  token_url: https://serviceaccounts.liveramp.com/authn/v1/oauth2/token\n  grant_type: password\n  client_id: liveramp-api\n  scope:\
  \ openid\n  token_type: Bearer\n  expires_in_seconds: 600\n  applies_to:\n  - LiveRamp Activation API\n  - LiveRamp AbiliTec API\n  - LiveRamp RampID API\n  - LiveRamp Privacy API\n  docs: https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token\n  note: >-\n    Username is the service-account Account ID, password is the Secret Key, both delivered by a\n    LiveRamp representative as a JSON credentials file. Access tokens are short lived (the\n    documented example is 600 seconds); the docs instruct clients to fetch a new token on a 403\n    token-expiration response and to share one token across a thread rather than refresh per call.\n- name: Clean Room (Habu) OAuth\n  token_url: https://api.habu.com/v1/oauth/token\n  grant_type: client_credentials\n  applies_to:\n  - LiveRamp Clean Room API\n  source: openapi/liveramp-clean-room-api-openapi.yml\nschemes:\n- name: application\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.habu.com/v1/oauth/token\n\
  \    scopes: 0\n  sources:\n  - openapi/liveramp-clean-room-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/liveramp-privacy-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Authorization: Bearer <access_token>, where the access token comes from the LiveRamp service\n    account token service. Documented for the Activation API, which publishes no securitySchemes\n    block in its own OpenAPI.\n  sources:\n  - https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token\nrequired_headers:\n- name: LR-Org-Id\n  applies_to:\n  - LiveRamp Activation API\n  note: >-\n    Replaced the former LR-Customer-Id header (see the Activation API changelog entry \"LR-Org-Id\n    replaces LR-Customer-Id\").\n  source: https://developers.liveramp.com/activation-api/changelog/lr-org-id-replaces-lr-customer-id\ntransport:\n  tls_minimum: '1.2'\n  source: https://developers.liveramp.com/rampid-api/changelog/tls-requirement-upgrade\n\
  x-evidence:\n- url: https://developers.liveramp.com/activation-api/reference/oauth2defaultv1token.md\n  http_status: 200\n- url: https://developers.liveramp.com/activation-api/reference/getting-started-1.md\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/authentication/liveramp-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Data Connectivity
- Data Collaboration
- Identity Resolution
- Activation
- Clean Room
- Privacy
- AdTech
- Marketing
- Consent
- Audience Segments
---
