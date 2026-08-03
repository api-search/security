---
api_key_in: []
api_specs:
- filename: artlist-search-openapi-original.yml
  format: yaml
  label: Artlist Enterprise Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/openapi/artlist-search-openapi-original.yml
- filename: artlist-download-openapi-original.yml
  format: yaml
  label: Artlist Enterprise Download API
  slug: download
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/openapi/artlist-download-openapi-original.yml
auth_types:
- oauth2
description: The Artlist Enterprise API is protected by an OAuth 2.0 client-credentials flow against an Amazon Cognito authorization server, with credentials issued out-of-band by an Artlist account manager. Neither published OpenAPI document declares a securityScheme, so this profile is captured from the documentation rather than derived from the spec — see `spec_gap` below.
kind: authentication
layout: security
method: searched
name: Artlist Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Artlist secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Artlist
provider_slug: artlist
scheme_count: 1
schemes:
- applies_to:
  - openapi/artlist-search-openapi-original.yml
  - openapi/artlist-download-openapi-original.yml
  flow: clientCredentials
  name: OAuth2ClientCredentials
  request:
    authorization_header: Basic <base64(client_id:client_secret)>
    body: grant_type=client_credentials
    content_type: application/x-www-form-urlencoded
  response_fields:
  - access_token
  - token_type
  - expires_in
  scopes: []
  sources:
  - https://developer.artlist.io/authentication
  token_endpoint_auth_method: client_secret_basic
  token_lifetime_seconds: 3600
  token_url: https://artlist-business-api-prod-cognito.artlist.io/oauth2/token
  type: oauth2
slug: artlist-authentication
source_filename: artlist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://developer.artlist.io/authentication\ndocs: https://developer.artlist.io/authentication\ndescription: >-\n  The Artlist Enterprise API is protected by an OAuth 2.0 client-credentials flow against an\n  Amazon Cognito authorization server, with credentials issued out-of-band by an Artlist\n  account manager. Neither published OpenAPI document declares a securityScheme, so this\n  profile is captured from the documentation rather than derived from the spec — see\n  `spec_gap` below.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  token_type: Bearer\n  scopes_documented: false\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://artlist-business-api-prod-cognito.artlist.io/oauth2/token\n  token_endpoint_auth_method: client_secret_basic\n  request:\n    content_type: application/x-www-form-urlencoded\n    body: grant_type=client_credentials\n\
  \    authorization_header: >-\n      Basic <base64(client_id:client_secret)>\n  response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  token_lifetime_seconds: 3600\n  scopes: []\n  applies_to:\n  - openapi/artlist-search-openapi-original.yml\n  - openapi/artlist-download-openapi-original.yml\n  sources:\n  - https://developer.artlist.io/authentication\nrequest_authorization:\n  header: Authorization\n  format: Bearer <access_token>\ncredential_issuance:\n  self_service: false\n  process: >-\n    client_id and client_secret are issued and managed by an Artlist account manager. The\n    documentation states that a self-service developer portal is \"available soon\".\n  contact: enterprise-api-support@artlist.io\nprovider_guidance:\n- Never expose client_secret in client-side code.\n- Store client credentials securely.\n- Rotate client credentials periodically.\n- Access tokens expire after one hour; refresh before expiry.\nobserved:\n  unauthenticated_call:\n    url: https://business.artlist.io/search/v1/song\n\
  \    http_status: 401\n    fetched: '2026-08-02'\n  token_endpoint:\n    url: https://artlist-business-api-prod-cognito.artlist.io/oauth2/token\n    unauthenticated_post_status: 400\n    fetched: '2026-08-02'\n  oidc_discovery: not published (404 on /.well-known/openid-configuration)\nspec_gap: >-\n  openapi/artlist-search-openapi-original.yml and openapi/artlist-download-openapi-original.yml\n  contain no components.securitySchemes and no security requirement on any operation, so the\n  machine-readable contract does not express the auth model that the docs describe. The\n  overlays in overlays/ add the missing oauth2 scheme as an API Evangelist enhancement without\n  mutating the harvested originals.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/authentication/artlist-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Music
- Audio
- Media
- Stock Media
- Content Licensing
- Creative Tools
- Search
- Generative AI
- Video
---
