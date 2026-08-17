---
api_key_in:
- query
api_specs:
- filename: mailboxlayer-verification-api-openapi.yml
  format: yaml
  label: mailboxlayer Verification API
  slug: mailboxlayer-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailboxlayer/refs/heads/main/openapi/mailboxlayer-verification-api-openapi.yml
auth_types:
- apiKey
description: Authentication profile for the mailboxlayer Verification API. Derived from the OpenAPI security schemes and upgraded to searched on 2026-08-14 against the provider's own "API Access Key & Authentication" documentation.
kind: authentication
layout: security
method: searched
name: Mailboxlayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: mailboxlayer secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: mailboxlayer
provider_slug: mailboxlayer
scheme_count: 2
schemes:
- description: Mailboxlayer API Access Key, required on every request to every operation. Issued at signup — one key per APILayer account, covering every APILayer product on that account.
  in: query
  name: AccessKeyQuery
  parameter: access_key
  required: true
  sources:
  - openapi/_original/mailboxlayer-swaggerhub-openapi.json
  type: apiKey
- description: Same scheme under the name used in this repo's refined spec. AccessKeyQuery (the provider's own name) and AccessKeyAuth are the same credential.
  in: query
  name: AccessKeyAuth
  parameter: access_key
  sources:
  - openapi/mailboxlayer-verification-api-openapi.yml
  type: apiKey
slug: mailboxlayer-authentication
source_filename: mailboxlayer-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.apilayer.com/mailboxlayer/docs/getting-started
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.apilayer.com/mailboxlayer/docs/getting-started\ndocs: https://docs.apilayer.com/mailboxlayer/docs/getting-started\nsources:\n  - https://docs.apilayer.com/mailboxlayer/docs/getting-started\n  - openapi/_original/mailboxlayer-swaggerhub-openapi.json\n  - openapi/mailboxlayer-verification-api-openapi.yml\ndescription: >-\n  Authentication profile for the mailboxlayer Verification API. Derived from the OpenAPI\n  security schemes and upgraded to searched on 2026-08-14 against the provider's own\n  \"API Access Key & Authentication\" documentation.\n\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n\nschemes:\n- name: AccessKeyQuery\n  type: apiKey\n  in: query\n  parameter: access_key\n  required: true\n  description: >-\n    Mailboxlayer API Access Key, required on every request to every operation. Issued at\n    signup — one key per APILayer\
  \ account, covering every APILayer product on that account.\n  sources:\n  - openapi/_original/mailboxlayer-swaggerhub-openapi.json\n- name: AccessKeyAuth\n  type: apiKey\n  in: query\n  parameter: access_key\n  description: >-\n    Same scheme under the name used in this repo's refined spec. AccessKeyQuery (the\n    provider's own name) and AccessKeyAuth are the same credential.\n  sources:\n  - openapi/mailboxlayer-verification-api-openapi.yml\n\ncredential:\n  issuance: >-\n    Self-serve. Signing up at https://mailboxlayer.com/product or\n    https://app.apilayer.com/signup assigns a personal API Access Key immediately; no\n    credit card is required for the Free plan.\n  dashboard: https://app.apilayer.com/\n  scope: >-\n    One account, one key, every APILayer API. The key is not scoped to mailboxlayer — it is\n    the account credential across the whole APILayer marketplace, so its blast radius is the\n    entire product portfolio the account subscribes to.\n  rotation:\n    documented:\
  \ false\n    note: No key-rotation procedure, expiry, or revocation policy is documented publicly.\n  multiple_keys:\n    supported: false\n    note: >-\n      No per-environment or per-application key issuance is documented. finops/ recommends\n      one key per environment for cost allocation, but the provider does not document a\n      mechanism for issuing more than one.\n\nusage:\n  example: 'https://apilayer.net/api/check?access_key=YOUR_ACCESS_KEY&email=support@apilayer.com'\n  quote: >-\n    \"After signing up, every user is assigned a personal API Access Key — a unique\n    'password' used to access the API's data and features. To authenticate with the\n    Mailboxlayer API, simply attach your access_key to the base endpoint URL.\"\n  transport:\n    https: true\n    note: >-\n      256-bit HTTPS is listed as available on all plans including Free on both the pricing\n      page and the Getting Started docs (checked 2026-08-14). Error 105\n      (https_access_restricted) nonetheless\
  \ remains in the published error catalog. The\n      documentation's own worked examples still use http:// URLs.\n\nhazards:\n  - id: key-in-query-string\n    severity: high\n    description: >-\n      The credential is a query parameter, so it is recorded wherever URLs are recorded:\n      proxy and CDN logs, browser history, Referer headers, error trackers, and any agent\n      trace that logs request URLs. There is no header-based alternative.\n    mitigation: >-\n      Call server-side, never from a browser with a production key, and redact `access_key`\n      from every log sink and agent transcript.\n  - id: no-scoping\n    severity: medium\n    description: >-\n      A single key authorizes every APILayer product on the account. A leaked mailboxlayer\n      key is a leaked marketstack / ipstack / scrapestack key.\n  - id: auth-failure-returns-200\n    severity: high\n    description: >-\n      Authentication failure has historically been returned with HTTP 200 and a\n      `success:false`\
  \ body (code 101). The current published spec also declares a real 401.\n      Handle both — a 200 is not evidence the call was authorized.\n    reference: errors/mailboxlayer-problem-types.yml\n  - id: no-oauth-no-scopes\n    severity: informational\n    description: >-\n      No OAuth 2.0, no OpenID Connect, no scopes, no token exchange. There is no\n      delegation model, so an agent acting for a user necessarily holds the account's full\n      credential. No scopes/ artifact is emitted — there is no scope surface to record.\n\nrelated:\n  conventions: conventions/mailboxlayer-conventions.yml\n  errors: errors/mailboxlayer-problem-types.yml\n  domain_security: security/mailboxlayer-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailboxlayer/refs/heads/main/authentication/mailboxlayer-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Email
- Email Verification
- Email Validation
- SMTP
- MX Records
- Catch-All Detection
- Disposable Email
- Free Email Provider
- Role Address
- Quality Score
- apilayer
- Public APIs
---
