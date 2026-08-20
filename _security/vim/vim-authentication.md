---
api_key_in: []
api_specs:
- filename: vim-rest-api-openapi-original.json
  format: json
  label: Vim Applications & Organizations API
  slug: vim-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-rest-api-openapi-original.json
- filename: vim-rest-api-openapi-original.json
  format: json
  label: Vim Invitations API
  slug: vim-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-rest-api-openapi-original.json
- filename: vim-rest-api-openapi-original.json
  format: json
  label: Vim Appointments API
  slug: vim-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-rest-api-openapi-original.json
- filename: vim-rest-api-openapi-original.json
  format: json
  label: Vim Chart Retrieval API
  slug: vim-chart-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-rest-api-openapi-original.json
- filename: vim-data-source-openapi-original.json
  format: json
  label: Vim Data Source
  slug: vim-data-source
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/openapi/vim-data-source-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Vim Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Vim secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Vim
provider_slug: vim
scheme_count: 2
schemes:
- applied_to: all Vim REST API operations except POST /oauth/token
  bearerFormat: JWT
  description: Bearer token sent in the Authorization header on every authenticated resource request. Obtained from POST /oauth/token.
  name: Access token
  scheme: bearer
  sources:
  - openapi/vim-rest-api-openapi-original.json
  - openapi/vim-data-source-openapi-original.json
  type: http
- flows:
  - flow: implicit
    scopes: 0
  name: service
  note: The Data Source spec declares an oauth2 scheme with an implicit flow and no scopes; in practice the documented exchange is client_credentials. The spec block is thin, not the real grant.
  sources:
  - openapi/vim-data-source-openapi-original.json
  type: oauth2
slug: vim-authentication
source_filename: vim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\ndocs: https://docs.getvim.com/api\nsource:\n  - https://docs.getvim.com/api\n  - https://docs.getvim.com/testing/managing-account\n  - openapi/vim-data-source-openapi-original.json\n  - openapi/vim-rest-api-openapi-original.json\n  - well-known/vim-openid-configuration.json\n# Vim uses one auth model across both REST surfaces: OAuth 2.0 client\n# credentials exchanged for a short-lived bearer JWT, then sent as\n# Authorization: Bearer on every resource request. Credentials are issued by\n# Vim, not self-service - the Client ID and secret are read from the My Account\n# tab of the Vim Console (console.getvim.com) after Vim provisions a Vim Canvas\n# developer account.\nsummary:\n  types:\n    - http\n    - oauth2\n  oauth2_flows:\n    - clientCredentials\n  self_service_credentials: false\n  credential_source: https://console.getvim.com (My Account tab)\nschemes:\n  - name: Access token\n    type: http\n    scheme: bearer\n    bearerFormat:\
  \ JWT\n    description: >-\n      Bearer token sent in the Authorization header on every authenticated\n      resource request. Obtained from POST /oauth/token.\n    applied_to: all Vim REST API operations except POST /oauth/token\n    sources:\n      - openapi/vim-rest-api-openapi-original.json\n      - openapi/vim-data-source-openapi-original.json\n  - name: service\n    type: oauth2\n    flows:\n      - flow: implicit\n        scopes: 0\n    note: >-\n      The Data Source spec declares an oauth2 scheme with an implicit flow and\n      no scopes; in practice the documented exchange is client_credentials. The\n      spec block is thin, not the real grant.\n    sources:\n      - openapi/vim-data-source-openapi-original.json\ntoken_exchange:\n  endpoint: POST /oauth/token\n  base_url: https://api.getvim.com/v1\n  grant_type: client_credentials\n  request_media_type: application/json\n  request_fields:\n    - client_id\n    - client_secret\n    - grant_type\n  response_fields:\n    - access_token\n\
  \    - token_type\n    - expires_in\n  token_type: Bearer\n  token_format: JWT\n  default_ttl_seconds: 3600\n  errors:\n    - status: 400\n      meaning: Bad request - ensure all required parameters were sent.\n    - status: 401\n      meaning: Unauthorized - ensure the client id and client secret are correct.\nauthorization_server:\n  host: https://auth.getvim.com\n  kind: Auth0 tenant\n  openid_configuration: well-known/vim-openid-configuration.json\n  oauth_authorization_server: well-known/vim-oauth-authorization-server.json\n  note: >-\n    Machine-to-machine access is audience-scoped rather than scope-scoped; see\n    scopes/vim-scopes.yml.\nsdk_authentication:\n  surface: VimOS.js\n  model: >-\n    Browser applications authenticate through the Vim Connect session rather\n    than by holding a client secret; the SDK is initialised with the\n    application identity and the EHR session supplies user context. The optional\n    VimAppSettings SDK exchanges an idToken plus organization\
  \ id.\n  docs: https://docs.getvim.com/vim-os-js/authentication\nconstraints:\n  geography: >-\n    The Vim REST API is available only to application servers hosted within the\n    United States. Developers outside the US may read the docs and call via VPN,\n    but the production application server must be US-hosted.\n  source: https://docs.getvim.com/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vim/refs/heads/main/authentication/vim-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Healthcare
- United States
- Clinical AI
- EHR Integration
- Point of Care
- Interoperability
- Value-Based Care
- Care Gaps
- Authentication
---
