---
api_key_in: []
api_specs:
- filename: podium-accounts-openapi.yml
  format: yaml
  label: Podium API
  slug: podium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podium/refs/heads/main/openapi/podium-accounts-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Podium Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Podium secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Podium
provider_slug: podium
scheme_count: 1
schemes:
- description: Podium API requests are authenticated with an OAuth 2.0 bearer access token issued to a developer application against a Podium user's organization/locations. There is no API-key alternative documented.
  flows:
  - authorizationUrl: https://api.podium.com/oauth/authorize
    flow: authorizationCode
    grant_type: authorization_code
    parameters:
    - client_id
    - redirect_uri
    - scope
    - state
    scope_count: 25
    tokenUrl: https://api.podium.com/oauth/token
    token_exchange_parameters:
    - client_id
    - client_secret
    - redirect_uri
    - code
    - grant_type
  - flow: refreshToken
    grant_type: refresh_token
    parameters:
    - client_id
    - client_secret
    - refresh_token
    - grant_type
    tokenUrl: https://api.podium.com/oauth/token
  name: OAuth2
  sources:
  - https://docs.podium.com/docs/oauth
  - https://docs.podium.com/reference/authentication
  type: oauth2
slug: podium-authentication
source_filename: podium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.podium.com/docs/oauth\ndocs: https://docs.podium.com/docs/oauth\nnote: >-\n  The 12 OpenAPI definitions Podium publishes through its ReadMe project declare no\n  `components.securitySchemes` and carry an empty top-level `security: []`, so the auth model\n  could not be derived from the contract. It was read instead from Podium's own OAuth guide,\n  authentication reference and getting-started guide, and the operation descriptions inside the\n  specs (each names its `Required scope:`).\nsummary:\n  types:\n    - oauth2\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n    - refreshToken\n  bearer_only: true\n  spec_declares_security: false\nschemes:\n  - name: OAuth2\n    type: oauth2\n    description: >-\n      Podium API requests are authenticated with an OAuth 2.0 bearer access token issued to a\n      developer application against a Podium user's organization/locations. There is no API-key\n     \
  \ alternative documented.\n    sources:\n      - https://docs.podium.com/docs/oauth\n      - https://docs.podium.com/reference/authentication\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.podium.com/oauth/authorize\n        tokenUrl: https://api.podium.com/oauth/token\n        parameters: [client_id, redirect_uri, scope, state]\n        token_exchange_parameters: [client_id, client_secret, redirect_uri, code, grant_type]\n        grant_type: authorization_code\n        scope_count: 25\n      - flow: refreshToken\n        tokenUrl: https://api.podium.com/oauth/token\n        parameters: [client_id, client_secret, refresh_token, grant_type]\n        grant_type: refresh_token\ntoken:\n  transport: header\n  header: Authorization\n  format: 'Bearer {access_token}'\n  type: JWT\n  lifetime: 10 hours\n  lifetime_source: https://docs.podium.com/docs/oauth\n  refresh: >-\n    A refresh_token is returned alongside the access_token and is exchanged at the same\
  \ token\n    endpoint with grant_type=refresh_token.\nregistration:\n  model: developer-portal application\n  portal: https://developer.podium.com/\n  steps:\n    - Request access to the Podium Developer Portal and wait for approval\n    - Create an app in the developer dashboard (icon, redirect URL)\n    - Select the app's scopes, following least privilege\n    - Copy the Client ID and Client Secret (the secret cannot be retrieved again)\n    - Request test organization/location access, then complete the OAuth flow\n  source: https://docs.podium.com/docs/getting-started\ntransport:\n  https_required: true\n  note: All API requests must be made over HTTPS; plain HTTP calls fail.\nscopes_artifact: scopes/podium-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podium/refs/heads/main/authentication/podium-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Customer Communication
- Reviews
- Messaging
- Payments
- Webchat
- Local Business
- SMS
- Lead Generation
---
