---
api_key_in: []
api_specs:
- filename: google-indexing-urlnotifications-api-openapi.yml
  format: yaml
  label: Google Indexing urlNotifications API
  slug: google-indexing-urlnotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/openapi/google-indexing-urlnotifications-api-openapi.yml
- filename: google-indexing-urlnotifications-publish-api-openapi.yml
  format: yaml
  label: Google Indexing urlNotifications:publish API
  slug: google-indexing-urlnotifications-publish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/openapi/google-indexing-urlnotifications-publish-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Google Indexing Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- jwt-bearer (service account)
overview: Google Indexing secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and jwt-bearer (service account) flow(s).
provider_name: Google Indexing
provider_slug: google-indexing
scheme_count: 1
schemes:
- challenge:
    body_reason: CREDENTIALS_MISSING
    body_status: UNAUTHENTICATED
    http_status: 401
    probed: '2026-08-13'
    url: https://indexing.googleapis.com/v3/urlNotifications/metadata?url=https%3A%2F%2Fexample.com
    www_authenticate: Bearer realm="https://accounts.google.com/"
  flows:
  - credential: JSON private key downloaded at service-account creation
    flow: jwt-bearer
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    note: The documented onboarding path. Not expressible as a standard OpenAPI oauth2 flow, which is why the derived baseline missed it.
    preferred: true
    principal: Google Cloud service account
    scopes:
    - https://www.googleapis.com/auth/indexing
    source: https://developers.google.com/search/apis/indexing-api/v3/prereqs
    tokenUrl: https://oauth2.googleapis.com/token
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    note: Present in the spec and usable (the OAuth 2.0 Playground exercises it), but Google's docs describe the service-account path.
    scopes:
    - https://www.googleapis.com/auth/indexing
    source: openapi/google-indexing-urlnotifications-publish-api-openapi.yml
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  primary: true
  sources:
  - openapi/google-indexing-urlnotifications-api-openapi.yml
  - openapi/google-indexing-urlnotifications-publish-api-openapi.yml
  - openapi/_original/google-indexing-discovery-v3.json
  - https://developers.google.com/search/apis/indexing-api/v3/prereqs
  transport:
    header: Authorization
    scheme: Bearer
    value: Bearer <access_token>
  type: oauth2
slug: google-indexing-authentication
source_filename: google-indexing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.google.com/search/apis/indexing-api/v3/prereqs\ndocs: https://developers.google.com/search/apis/indexing-api/v3/prereqs\nauthorizing_docs: https://developers.google.com/search/apis/indexing-api/v3/authorizing\nnote: >-\n  Upgraded from derived to searched on 2026-08-13. The OpenAPI-derived baseline captured only the\n  authorizationCode flow. Google's own prerequisites page documents a different primary path — a Google\n  Cloud SERVICE ACCOUNT with a JSON private key, exchanging a signed JWT assertion for an access token —\n  plus a second, non-OAuth authorization gate that no securityScheme can express: the service account\n  must be a delegated site owner on a verified Search Console property. Missing that gate is the single\n  most common failure on this API, and it returns 403, not 401.\nsummary:\n  types:\n    - oauth2\n  oauth2_flows:\n    - authorizationCode\n    - jwt-bearer (service account)\n  api_key_supported:\
  \ false\n  anonymous_access: false\n  scopes: 1\nschemes:\n  - name: OAuth2\n    type: oauth2\n    primary: true\n    flows:\n      - flow: jwt-bearer\n        preferred: true\n        grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n        tokenUrl: https://oauth2.googleapis.com/token\n        principal: Google Cloud service account\n        credential: JSON private key downloaded at service-account creation\n        scopes:\n          - https://www.googleapis.com/auth/indexing\n        source: https://developers.google.com/search/apis/indexing-api/v3/prereqs\n        note: >-\n          The documented onboarding path. Not expressible as a standard OpenAPI oauth2 flow, which is\n          why the derived baseline missed it.\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n        scopes:\n          - https://www.googleapis.com/auth/indexing\n        source: openapi/google-indexing-urlnotifications-publish-api-openapi.yml\n\
  \        note: >-\n          Present in the spec and usable (the OAuth 2.0 Playground exercises it), but Google's docs\n          describe the service-account path.\n    transport:\n      header: Authorization\n      scheme: Bearer\n      value: Bearer <access_token>\n    challenge:\n      probed: '2026-08-13'\n      url: https://indexing.googleapis.com/v3/urlNotifications/metadata?url=https%3A%2F%2Fexample.com\n      http_status: 401\n      www_authenticate: Bearer realm=\"https://accounts.google.com/\"\n      body_status: UNAUTHENTICATED\n      body_reason: CREDENTIALS_MISSING\n    sources:\n      - openapi/google-indexing-urlnotifications-api-openapi.yml\n      - openapi/google-indexing-urlnotifications-publish-api-openapi.yml\n      - openapi/_original/google-indexing-discovery-v3.json\n      - https://developers.google.com/search/apis/indexing-api/v3/prereqs\nauthorization_server:\n  issuer: https://accounts.google.com\n  metadata:\n    oauth_authorization_server:\n      url: https://accounts.google.com/.well-known/oauth-authorization-server\n\
  \      status: 200\n      file: well-known/google-indexing-oauth-authorization-server.json\n    openid_configuration:\n      url: https://accounts.google.com/.well-known/openid-configuration\n      status: 200\n      file: well-known/google-indexing-openid-configuration.json\n  token_endpoint: https://oauth2.googleapis.com/token\n  revocation_endpoint: https://oauth2.googleapis.com/revoke\n  device_authorization_endpoint: https://oauth2.googleapis.com/device/code\n  jwks_uri: https://www.googleapis.com/oauth2/v3/certs\n  pkce: true\n  note: >-\n    Served by accounts.google.com. The API host indexing.googleapis.com 404s on both well-known paths.\nsecond_gate:\n  name: Search Console delegated site ownership\n  type: out-of-band authorization\n  required: true\n  enforced_at: request time, per URL\n  failure:\n    http_status: 403\n    message: Permission denied. Failed to verify the URL ownership.\n  steps:\n    - Verify the site in Google Search Console (domain or URL-prefix property).\n\
  \    - Add the service account email as a delegated owner on that property.\n  source: https://developers.google.com/search/apis/indexing-api/v3/prereqs\n  note: >-\n    A valid token with the correct scope is NOT sufficient. Authorization on this API is per-URL and is\n    resolved against Search Console property ownership, which is invisible to the OAuth layer.\nmtls:\n  endpoint: https://indexing.mtls.googleapis.com/\n  source: openapi/_original/google-indexing-discovery-v3.json\ncross_links:\n  scopes: scopes/google-indexing-scopes.yml\n  conventions: conventions/google-indexing-conventions.yml\n  errors: errors/google-indexing-error-codes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/authentication/google-indexing-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Crawling
- Google
- Indexing
- Search
- SEO
- URLs
---
