---
api_key_in:
- header
api_specs:
- filename: goatcounter-exports-api-openapi.yml
  format: yaml
  label: GoatCounter Exports API
  slug: goatcounter-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-exports-api-openapi.yml
- filename: goatcounter-pageviews-api-openapi.yml
  format: yaml
  label: GoatCounter Pageviews API
  slug: goatcounter-pageviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-pageviews-api-openapi.yml
- filename: goatcounter-paths-api-openapi.yml
  format: yaml
  label: GoatCounter Paths API
  slug: goatcounter-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-paths-api-openapi.yml
- filename: goatcounter-sites-api-openapi.yml
  format: yaml
  label: GoatCounter Sites API
  slug: goatcounter-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-sites-api-openapi.yml
- filename: goatcounter-statistics-api-openapi.yml
  format: yaml
  label: GoatCounter Statistics API
  slug: goatcounter-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-statistics-api-openapi.yml
- filename: goatcounter-users-api-openapi.yml
  format: yaml
  label: GoatCounter Users API
  slug: goatcounter-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/openapi/goatcounter-users-api-openapi.yml
auth_types:
- http
description: GoatCounter authenticates the JSON API with a per-site API key. The primary documented scheme is an HTTP bearer token in the Authorization header; HTTP Basic is also accepted with an empty username and the API key as the password, which the docs describe as mostly useful for testing from a browser. Note that the provider-published OpenAPI 2.0 document declares only basicAuth under securityDefinitions, so the bearer scheme — the one the docs lead with — is documented in prose but absent from the machine-readable contract. Both are recorded here.
kind: authentication
layout: security
method: searched
name: Goatcounter Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoatCounter secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GoatCounter
provider_slug: goatcounter
scheme_count: 2
schemes:
- documented: true
  format: 'Authorization: Bearer <token>'
  in: header
  in_spec: false
  name: bearerAuth
  note: The documented primary scheme. Present in the API Evangelist refined OpenAPI files but not in the provider's own api.json, whose securityDefinitions contains basicAuth only.
  parameter: Authorization
  scheme: bearer
  sources:
  - https://www.goatcounter.com/help/api
  - openapi/goatcounter-users-api-openapi.yml
  type: http
- documented: true
  evidence:
    probed: '2026-08-13'
    response_header: 'www-authenticate: Basic realm=GoatCounter'
    url: https://stats.arp242.net/api/v0/me
  in: header
  in_spec: true
  name: basicAuth
  parameter: Authorization
  password: the API key
  scheme: basic
  sources:
  - openapi/_original/goatcounter-api-swagger20.json
  - https://www.goatcounter.com/help/api
  type: http
  username: (leave empty)
slug: goatcounter-authentication
source_filename: goatcounter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/goatcounter-api-swagger20.json\ndocs: https://www.goatcounter.com/help/api\ndescription: >-\n  GoatCounter authenticates the JSON API with a per-site API key. The primary documented scheme\n  is an HTTP bearer token in the Authorization header; HTTP Basic is also accepted with an empty\n  username and the API key as the password, which the docs describe as mostly useful for testing\n  from a browser. Note that the provider-published OpenAPI 2.0 document declares only basicAuth\n  under securityDefinitions, so the bearer scheme — the one the docs lead with — is documented in\n  prose but absent from the machine-readable contract. Both are recorded here.\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n    - basic\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in:\
  \ header\n    parameter: Authorization\n    format: 'Authorization: Bearer <token>'\n    documented: true\n    in_spec: false\n    sources:\n      - https://www.goatcounter.com/help/api\n      - openapi/goatcounter-users-api-openapi.yml\n    note: >-\n      The documented primary scheme. Present in the API Evangelist refined OpenAPI files but not\n      in the provider's own api.json, whose securityDefinitions contains basicAuth only.\n  - name: basicAuth\n    type: http\n    scheme: basic\n    in: header\n    parameter: Authorization\n    documented: true\n    in_spec: true\n    username: '(leave empty)'\n    password: 'the API key'\n    sources:\n      - openapi/_original/goatcounter-api-swagger20.json\n      - https://www.goatcounter.com/help/api\n    evidence:\n      probed: '2026-08-13'\n      url: https://stats.arp242.net/api/v0/me\n      response_header: 'www-authenticate: Basic realm=GoatCounter'\ncredential:\n  kind: api-key\n  name: API key / API token\n  issuance: >-\n    Created\
  \ by the account holder in the GoatCounter dashboard under [Username in top menu] -> API.\n  scope: per-site\n  rotation: self-serve (create and delete keys in the dashboard)\n  oauth: false\n  note: >-\n    There is no OAuth or OIDC surface, so there is no scopes/ artifact for this provider. Keys carry\n    a permissions set instead — see permissions below.\npermissions:\n  model: per-key permission flags\n  discoverable_at: GET /api/v0/me\n  schema: goatcounter.APIToken (fields name, permissions, sites)\n  source: openapi/_original/goatcounter-api-swagger20.json\n  note: >-\n    The published OpenAPI types the APIToken object with a permissions field, and the docs state that\n    a key without the needed permission gets 403 Forbidden, but the individual permission names are\n    not enumerated in the public documentation or in the spec. Not guessed here.\nfailure_modes:\n  - status: 401\n    condition: API key missing or incorrect\n    source: https://www.goatcounter.com/help/api\n \
  \ - status: 403\n    condition: API key valid but lacks the needed permissions\n    source: https://www.goatcounter.com/help/api\ntransport:\n  https_required: true\n  content_type: application/json\n  note: All requests must set Content-Type application/json; all responses are JSON unless noted otherwise.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goatcounter/refs/heads/main/authentication/goatcounter-authentication.yml
summary_line: http · 2 schemes
tags:
- Analytics
- Pageviews
- Privacy
- Statistics
- Web Analytics
- Open Source
- Self-Hosted
- Events
- Data Export
- Developer Tools
---
