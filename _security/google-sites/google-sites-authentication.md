---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Google Sites Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Sites declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Google Sites
provider_slug: google-sites
scheme_count: 1
schemes:
- authorization_endpoint: https://accounts.google.com/o/oauth2/v2/auth
  consent: Google shows the user a consent screen for the requested scope; approval returns a short-lived access token. Refresh tokens are used to mint new access tokens.
  discovery: well-known/google-sites-openid-configuration.json
  flows:
  - authorizationCode
  id: oauth2
  issuer: https://accounts.google.com
  note: Endpoint and PKCE values confirmed against the live OAuth 2.0 / OIDC discovery documents saved at well-known/ (accounts.google.com), fetched 2026-09-12.
  pkce: true
  pkce_methods:
  - plain
  - S256
  registration: Register the application in the Google API Console to obtain a client ID and client secret, then activate the Google Sites Data API for the project.
  revocation_endpoint: https://oauth2.googleapis.com/revoke
  scopes:
  - https://sites.google.com/feeds/
  token_endpoint: https://oauth2.googleapis.com/token
  transport: Authorization request header
  type: oauth2
slug: google-sites-authentication
source_filename: google-sites-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://developers.google.com/workspace/sites/docs/1.0/developers_guide_protocol\ndocs: https://developers.google.com/workspace/sites/docs/1.0/developers_guide_protocol\nnote: >-\n  Authored from the Google Sites Data API protocol guide, not derived from a spec -\n  this API publishes no OpenAPI or discovery document, so there are no securitySchemes\n  to read. The guide is explicit: \"Your application must use OAuth 2.0 to authorize\n  requests. No other authorization protocols are supported.\"\nschemes:\n  - id: oauth2\n    type: oauth2\n    flows:\n      - authorizationCode\n    authorization_endpoint: https://accounts.google.com/o/oauth2/v2/auth\n    token_endpoint: https://oauth2.googleapis.com/token\n    revocation_endpoint: https://oauth2.googleapis.com/revoke\n    issuer: https://accounts.google.com\n    pkce: true\n    pkce_methods:\n      - plain\n      - S256\n    discovery: well-known/google-sites-openid-configuration.json\n\
  \    scopes:\n      - https://sites.google.com/feeds/\n    registration: >-\n      Register the application in the Google API Console to obtain a client ID and\n      client secret, then activate the Google Sites Data API for the project.\n    consent: >-\n      Google shows the user a consent screen for the requested scope; approval returns\n      a short-lived access token. Refresh tokens are used to mint new access tokens.\n    transport: Authorization request header\n    note: >-\n      Endpoint and PKCE values confirmed against the live OAuth 2.0 / OIDC discovery\n      documents saved at well-known/ (accounts.google.com), fetched 2026-09-12.\nretired_schemes:\n  - id: oauth1\n    type: oauth1\n    status: removed\n    removed: '2012-04-20'\n    note: >-\n      OAuth 1.0 is documented in the Python and Java guides but both pages carry the\n      banner \"The auth options described in this document (OAuth 1.0, AuthSub, and\n      ClientLogin) have been officially deprecated as of April\
  \ 20, 2012 and are no\n      longer available.\"\n  - id: authsub\n    type: proprietary\n    status: removed\n    removed: '2012-04-20'\n  - id: clientlogin\n    type: proprietary\n    status: removed\n    removed: '2012-04-20'\nanonymous_access:\n  supported: partial\n  note: >-\n    The Content feed \"may or may not require authentication, depending on the Site's\n    (published) settings\". The Activity, Revision, Site and ACL feeds state that all\n    requests must be authenticated.\napi_keys:\n  supported: false\n  note: >-\n    No API-key scheme is documented for the sites.google.com/feeds surface. (The\n    unrelated sites.googleapis.com host returns HTTP 403 \"Method doesn't allow\n    unregistered callers\" to anonymous callers, but publishes no discovery document\n    and is not the API this record documents.)\nmutual_tls:\n  supported: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-sites/refs/heads/main/authentication/google-sites-authentication.yml
summary_line: 1 scheme
tags:
- Collaboration
- Content Management
- Google Workspace
- Websites
- Website Builder
- CMS
- Publishing
- Productivity
- Deprecated APIs
- GData
---
