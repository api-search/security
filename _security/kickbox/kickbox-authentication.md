---
api_key_in:
- query
- header
api_specs:
- filename: kickbox-account-api-openapi.yml
  format: yaml
  label: Kickbox Account API
  slug: kickbox-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-account-api-openapi.yml
- filename: kickbox-batch-api-openapi.yml
  format: yaml
  label: Kickbox Batch API
  slug: kickbox-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-batch-api-openapi.yml
- filename: kickbox-open-api-openapi.yml
  format: yaml
  label: Kickbox Open API
  slug: kickbox-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-open-api-openapi.yml
- filename: kickbox-verification-api-openapi.yml
  format: yaml
  label: Kickbox Verification API
  slug: kickbox-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-verification-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kickbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kickbox secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kickbox
provider_slug: kickbox
scheme_count: 2
schemes:
- caution: A key in a query string is logged by proxies, browser history and server access logs. Prefer the Authorization header form where the client allows it.
  description: The API key supplied as the `apikey` query-string parameter. This is the canonical form in the Kickbox documentation and the form every first-party SDK emits.
  example: GET https://api.kickbox.com/v2/verify?email=user%40example.com&apikey=YOUR_API_KEY
  in: query
  name: apikey-query
  parameter_name: apikey
  required: true
  sources:
  - https://docs.kickbox.com/docs/using-the-api
  type: apiKey
- description: The API key supplied as the access token of an Authorization header using the Bearer scheme.
  example: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  in: header
  name: bearer-header
  scheme: bearer
  sources:
  - https://docs.kickbox.com/docs/using-the-api
  type: http
slug: kickbox-authentication
source_filename: kickbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.kickbox.com/docs/using-the-api\ndocs:\n  - https://docs.kickbox.com/docs/using-the-api\n  - https://docs.kickbox.com/docs/single-verification-api\nupgraded_from: derived\nupgraded_note: >-\n  The previous derived profile read only the harvested OpenAPI, which declares a single `TokenAuth`\n  http/bearer scheme described as `Authorization: token YOUR_API_KEY`. The provider's own\n  documentation shows two accepted forms and names the Bearer scheme explicitly, so the spec was\n  thin and slightly wrong. This searched profile records what the docs publish; the spec's scheme is\n  retained below under spec_schemes for traceability.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nmodel: >-\n  A single long-lived API key per credential, created and scoped in the Kickbox dashboard. There is\n  no OAuth, no OIDC, no token\
  \ exchange and no refresh — an agent holds a static secret. The key is\n  accepted either as a query-string parameter or as an Authorization Bearer header; the query form is\n  the one used throughout the documentation and by all four first-party SDKs.\nschemes:\n  - name: apikey-query\n    type: apiKey\n    in: query\n    parameter_name: apikey\n    required: true\n    description: >-\n      The API key supplied as the `apikey` query-string parameter. This is the canonical form in the\n      Kickbox documentation and the form every first-party SDK emits.\n    example: 'GET https://api.kickbox.com/v2/verify?email=user%40example.com&apikey=YOUR_API_KEY'\n    caution: >-\n      A key in a query string is logged by proxies, browser history and server access logs. Prefer\n      the Authorization header form where the client allows it.\n    sources: [https://docs.kickbox.com/docs/using-the-api]\n  - name: bearer-header\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n\
  \    description: >-\n      The API key supplied as the access token of an Authorization header using the Bearer scheme.\n    example: 'Authorization: Bearer YOUR_API_KEY'\n    sources: [https://docs.kickbox.com/docs/using-the-api]\nspec_schemes:\n  - name: TokenAuth\n    type: http\n    scheme: bearer\n    bearerFormat: token\n    sources:\n      - openapi/kickbox-account-api-openapi.yml\n      - openapi/kickbox-batch-api-openapi.yml\n      - openapi/kickbox-open-api-openapi.yml\n      - openapi/kickbox-verification-api-openapi.yml\ncredentials:\n  issuance:\n    where: Kickbox dashboard, API > Manage Keys\n    url: https://app.kickbox.com/signup\n    self_serve: true\n  key_prefixes:\n    live: live_\n    test: test_\n    note: >-\n      The prefix is how a holder can tell a production key from a sandbox key by inspection.\n      Production keys start with `live_`, sandbox keys start with `test_`.\n  modes:\n    - {mode: production, prefix: live_, consumes_credits: true}\n    - {mode:\
  \ sandbox, prefix: test_, consumes_credits: false}\n  mode_immutable: true\n  mode_immutable_note: >-\n    A key's mode is fixed at creation. The docs state you cannot switch a key between sandbox and\n    production mode; a new key must be created instead.\n  scoping:\n    style: per-key endpoint permissions\n    note: >-\n      Each key is granted permission to specific API endpoints at creation, and permissions are\n      editable afterwards. This is the closest thing Kickbox has to OAuth scopes, but it is\n      dashboard-configured rather than declared in a token, so there is no scope string an agent can\n      request or inspect. No scopes/ artifact is emitted for this provider.\n  rotation: undocumented\n  expiry: none documented\n  revocation:\n    note: >-\n      A key can be effectively disabled by editing it and unchecking all Verify permissions, which\n      the docs present as the pause/shut-off mechanism.\nunauthenticated_surface:\n  - operation: isDisposable\n    endpoint:\
  \ GET /v1/disposable/{email}\n    host: https://open.kickbox.com\n    note: >-\n      The open disposable-domain lookup requires no authentication. Kickbox's own published OpenAPI\n      for it declares `\"security\": [{}]`, i.e. explicitly optional/no security.\n    source: openapi/kickbox-disposable-openapi.json\naccount_authentication:\n  note: Dashboard/console sign-in, distinct from API authentication.\n  methods: [password, Sign in with Google, two-factor authentication, Okta SSO]\n  docs:\n    - https://docs.kickbox.com/docs/authentication-methods\n    - https://docs.kickbox.com/docs/okta-authentication\nregional:\n  note: >-\n    EU-only accounts authenticate against api.eu.kickbox.com rather than api.kickbox.com. The host is\n    a property of the account, not a parameter, so credentials are not portable between the two.\n  hosts: [https://api.kickbox.com, https://api.eu.kickbox.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/authentication/kickbox-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email Verification
- Email Validation
- Deliverability
- Data Quality
- Email
---
