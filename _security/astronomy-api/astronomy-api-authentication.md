---
anonymous_access: false
api_key_in: []
api_specs:
- filename: astronomy-api-bodies-api-openapi.yml
  format: yaml
  label: Astronomy API Bodies API
  slug: astronomy-api-bodies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/openapi/astronomy-api-bodies-api-openapi.yml
- filename: astronomy-api-events-api-openapi.yml
  format: yaml
  label: Astronomy API Events API
  slug: astronomy-api-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/openapi/astronomy-api-events-api-openapi.yml
- filename: astronomy-api-search-api-openapi.yml
  format: yaml
  label: Astronomy API Search API
  slug: astronomy-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/openapi/astronomy-api-search-api-openapi.yml
- filename: astronomy-api-studio-api-openapi.yml
  format: yaml
  label: Astronomy API Studio API
  slug: astronomy-api-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/openapi/astronomy-api-studio-api-openapi.yml
- filename: astronomy-api-v3-openapi.yaml
  format: yaml
  label: Astronomy API v3
  slug: astronomy-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/openapi/astronomy-api-v3-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Astronomy Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Astronomy API secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Astronomy API
provider_slug: astronomy-api
scheme_count: 2
schemes:
- description: 'HTTP Basic auth: username is the Application ID and password is the

    Application Secret. The client sends

    `Authorization: Basic base64(applicationId:applicationSecret)`.'
  docs: https://docs.astronomyapi.com/
  failure_note: The docs are explicit that a v2 authentication failure returns 403 Forbidden, not 401 — "which probably means you encrypted the string incorrectly, or your credentials are wrong."
  failure_status: 403
  name: basicAuth
  scheme: basic
  sources:
  - openapi/astronomy-api-bodies-api-openapi.yml
  - openapi/astronomy-api-events-api-openapi.yml
  - openapi/astronomy-api-search-api-openapi.yml
  - openapi/astronomy-api-studio-api-openapi.yml
  - https://docs.astronomyapi.com/
  status: production
  type: http
  version: v2
- description: 'The application key, sent as `Authorization: Bearer <key>`. Keys are

    never accepted in the query string, where they would be recorded in

    logs and browser history.'
  failure_status: 401
  name: applicationKey
  scheme: bearer
  sources:
  - openapi/astronomy-api-v3-openapi.yaml
  status: reference draft
  type: http
  version: v3
slug: astronomy-api-authentication
source_filename: astronomy-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://docs.astronomyapi.com/ (Getting Started — \"Obtaining an Application ID\n  and a Secret\" and \"Basic Authentication\"), openapi/astronomy-api-v3-openapi.yaml\n  (components.securitySchemes.applicationKey) and the four v2 definitions in\n  openapi/ (basicAuth). Baseline derived by\n  0-working/derive-authentication.py, then upgraded from the provider's docs.\nsummary:\n  types:\n    - http\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  api_key_header: false\n  note: >-\n    Two schemes for two versions. Production v2 is HTTP Basic; the published v3\n    draft moves to HTTP Bearer. There is no OAuth of any kind — no\n    /.well-known/openid-configuration or /.well-known/oauth-authorization-server\n    is served on any host (see well-known/astronomy-api-well-known.yml), so no\n    scopes artifact is emitted.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    version: v2\n    status:\
  \ production\n    description: |-\n      HTTP Basic auth: username is the Application ID and password is the\n      Application Secret. The client sends\n      `Authorization: Basic base64(applicationId:applicationSecret)`.\n    docs: https://docs.astronomyapi.com/\n    failure_status: 403\n    failure_note: >-\n      The docs are explicit that a v2 authentication failure returns 403\n      Forbidden, not 401 — \"which probably means you encrypted the string\n      incorrectly, or your credentials are wrong.\"\n    sources:\n      - openapi/astronomy-api-bodies-api-openapi.yml\n      - openapi/astronomy-api-events-api-openapi.yml\n      - openapi/astronomy-api-search-api-openapi.yml\n      - openapi/astronomy-api-studio-api-openapi.yml\n      - https://docs.astronomyapi.com/\n  - name: applicationKey\n    type: http\n    scheme: bearer\n    version: v3\n    status: reference draft\n    description: |-\n      The application key, sent as `Authorization: Bearer <key>`. Keys are\n      never\
  \ accepted in the query string, where they would be recorded in\n      logs and browser history.\n    failure_status: 401\n    sources:\n      - openapi/astronomy-api-v3-openapi.yaml\ncredential_lifecycle:\n  issuance: >-\n    Self-serve. Create a free account at https://astronomyapi.com/auth/signup,\n    then \"Create Application\" in the dashboard to receive an Application ID and\n    an Application Secret.\n  secret_visibility: once\n  secret_visibility_quote: >-\n    \"The Application Secret is visible to you only once during application\n    creation. Save it somewhere because there's no way to retrieve it back. If\n    you lost your secret create a new application and delete the old\n    application.\"\n  rotation:\n    supported: false\n    note: >-\n      There is no rotation flow. Rotating a credential means creating a new\n      application and deleting the old one — and the docs warn \"once an\n      application is deleted there's no way to recover it,\" so the two cannot\n\
  \      overlap safely without a deliberate cut-over.\n  expiry: none documented\n  revocation: Delete the application in the dashboard.\n  scoping:\n    dimension: origin\n    note: >-\n      An application carries an `Origin` value which the API echoes as the\n      Access-Control-Allow-Origin header. This is the only scoping mechanism —\n      there are no permissions, roles or scopes of any kind. Every credential\n      can call every operation.\nbrowser_exposure:\n  note: >-\n    The first-party widget library takes the same base64 Basic credential\n    embedded in page JavaScript, so a browser integration necessarily exposes\n    the application secret to anyone who reads the page. Setting the\n    application's Origin is the only mitigation the provider offers. See\n    components/astronomy-api-components.yml.\nmarketplace:\n  rapidapi:\n    note: >-\n      RapidAPI callers may share a pooled key and be throttled as one consumer;\n      the docs advise getting a first-party key from\
  \ the Astronomy API console\n      instead.\n    source: https://docs.astronomyapi.com/known-issues\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astronomy-api/refs/heads/main/authentication/astronomy-api-authentication.yml
summary_line: http · 2 schemes
tags:
- Astronomy
- Celestial Data
- Space
- Moon Phases
- Star Charts
---
