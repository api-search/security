---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blubrry-api-restful-api-for-podcast-publishing-statistics-episode-api-openapi.yml
  format: yaml
  label: Blubrry API Episode API
  slug: blubrry-api-restful-api-for-podcast-publishing-statistics-episode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-episode-api-openapi.yml
- filename: blubrry-api-restful-api-for-podcast-publishing-statistics-media-api-openapi.yml
  format: yaml
  label: Blubrry API Media API
  slug: blubrry-api-restful-api-for-podcast-publishing-statistics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-media-api-openapi.yml
- filename: blubrry-api-restful-api-for-podcast-publishing-statistics-statistics-api-openapi.yml
  format: yaml
  label: Blubrry API Statistics API
  slug: blubrry-api-restful-api-for-podcast-publishing-statistics-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-statistics-api-openapi.yml
- filename: blubrry-api-restful-api-for-podcast-publishing-statistics-podcaster-openapi.yaml
  format: yaml
  label: Blubrry Podcast Hosting & Statistics API (v2)
  slug: blubrry-podcast-hosting-statistics-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-podcaster-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blubrry Api Restful Api For Podcast Publishing Statistics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Blubrry API secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Blubrry API
provider_slug: blubrry-api-restful-api-for-podcast-publishing-statistics
scheme_count: 1
schemes:
- authorization_code_lifetime_seconds: 300
  authorization_code_single_use: true
  description: 'OAuth 2.0 Bearer token. Client ID + secret are created by the account holder from

    Manage Account -> Developers -> Create API Key in the Blubrry dashboard. Access tokens

    expire after 1 hour; refresh tokens do not expire but can be revoked by the account

    holder or by Blubrry, after which the authorization-code flow must be repeated.'
  flows:
  - authorizationUrl: https://api.blubrry.com/oauth2/authorize
    flow: authorizationCode
    refreshUrl: https://api.blubrry.com/oauth2/token
    scopes: 0
    tokenUrl: https://api.blubrry.com/oauth2/token
  header: Authorization
  in: header
  name: OAuth2
  refresh_token_expires: false
  scheme: Bearer
  sources:
  - https://blubrry.com/developer/api/oauth-2/
  - openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-episode-api-openapi.yml
  - openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-media-api-openapi.yml
  - openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-statistics-api-openapi.yml
  token_endpoint_auth_method: client_secret_basic
  token_lifetime_seconds: 3600
  type: oauth2
slug: blubrry-api-restful-api-for-podcast-publishing-statistics-authentication
source_filename: blubrry-api-restful-api-for-podcast-publishing-statistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://blubrry.com/developer/api/oauth-2/\ndocs: https://blubrry.com/developer/api/oauth-2/\nnote: >-\n  Derived from the OpenAPI security block, then upgraded against Blubrry's own OAuth 2\n  documentation page, which states the authorize/token endpoints, the 1-hour access-token\n  lifetime, the non-expiring refresh token, and the 5-minute single-use authorization code.\n  Blubrry's published podcaster.yaml declares no components.securitySchemes, so the auth\n  model here comes from the docs, not from the contract.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  scopes_supported: false\n  credential_issuance: self-serve\nschemes:\n- name: OAuth2\n  type: oauth2\n  in: header\n  header: Authorization\n  scheme: Bearer\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.blubrry.com/oauth2/authorize\n    tokenUrl: https://api.blubrry.com/oauth2/token\n    refreshUrl: https://api.blubrry.com/oauth2/token\n\
  \    scopes: 0\n  description: |-\n    OAuth 2.0 Bearer token. Client ID + secret are created by the account holder from\n    Manage Account -> Developers -> Create API Key in the Blubrry dashboard. Access tokens\n    expire after 1 hour; refresh tokens do not expire but can be revoked by the account\n    holder or by Blubrry, after which the authorization-code flow must be repeated.\n  token_endpoint_auth_method: client_secret_basic\n  token_lifetime_seconds: 3600\n  authorization_code_lifetime_seconds: 300\n  authorization_code_single_use: true\n  refresh_token_expires: false\n  sources:\n  - https://blubrry.com/developer/api/oauth-2/\n  - openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-episode-api-openapi.yml\n  - openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-media-api-openapi.yml\n  - openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-statistics-api-openapi.yml\ncredential_provisioning:\n  method: self-serve dashboard\n  steps:\n\
  \  - Sign in to the Blubrry account.\n  - Choose \"Manage Account\" from the account menu.\n  - Under the \"Developers\" section select \"Create API Key\".\n  source: https://blubrry.com/developer/api/oauth-2/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/authentication/blubrry-api-restful-api-for-podcast-publishing-statistics-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Podcasting
- Audio
- Media
- Publishing
- Statistics
---
