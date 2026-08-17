---
api_key_in:
- query
api_specs:
- filename: moosend-openapi.yml
  format: yaml
  label: Moosend API
  slug: moosend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moosend/refs/heads/main/openapi/moosend-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Moosend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moosend secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Moosend
provider_slug: moosend
scheme_count: 1
schemes:
- applied_to: all 47 operations
  description: Moosend account API key, supplied as the `apikey` query-string parameter on every request. Generated and regenerated in the account Settings menu.
  example_form: https://api.moosend.com/v3/campaigns/create.json?apikey=YOUR_API_KEY
  in: query
  name: apikeyQuery
  parameter: apikey
  provider_quote: '"Authentication is achieved through the use of an API key. This is a unique key for each account in our system... The API key must always be specified as a parameter in the query string of the requesting URL."'
  sources:
  - openapi/moosend-openapi.yml
  type: apiKey
slug: moosend-authentication
source_filename: moosend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/moosend-openapi.yml\ndocs: https://moosendapp.docs.apiary.io/api-description-document\ndocs_note: >-\n  The Authentication section of Moosend's own published API Blueprint. The help\n  centre landing page at\n  https://docs.moosend.com/developers/api-documentation/en/index-en.html is a\n  Salesforce Experience Cloud shell and carries no auth reference of its own.\n\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - query\n  oauth2_flows: []\n  scopes: false\n  mtls: false\n  openid_connect: false\n\nschemes:\n  - name: apikeyQuery\n    type: apiKey\n    in: query\n    parameter: apikey\n    description: >-\n      Moosend account API key, supplied as the `apikey` query-string parameter on\n      every request. Generated and regenerated in the account Settings menu.\n    sources:\n      - openapi/moosend-openapi.yml\n    applied_to: all 47 operations\n    provider_quote: >-\n      \"Authentication is achieved through\
  \ the use of an API key. This is a unique\n      key for each account in our system... The API key must always be specified\n      as a parameter in the query string of the requesting URL.\"\n    example_form: https://api.moosend.com/v3/campaigns/create.json?apikey=YOUR_API_KEY\n\ncredential_model:\n  granularity: one key per account\n  scopes_supported: false\n  per_integration_keys: false\n  expiry: none documented\n  rotation: manual, from the account Settings menu\n  revocation: regenerating the key invalidates the previous one\n  service_accounts: false\n\nfindings:\n  - id: key-in-query-string\n    severity: high\n    detail: >-\n      The credential travels in the request URL, so it is written into web-server,\n      proxy and CDN access logs, browser history and Referer headers. Moosend\n      documents no `Authorization` header or custom-header alternative.\n    remediation_for_provider: >-\n      Accept the same key in an `Authorization: Bearer` or `X-Api-Key` header,\n     \
  \ keeping the query parameter for backward compatibility.\n  - id: no-scopes\n    severity: high\n    detail: >-\n      A single account-wide key grants full read and write authority over every\n      mailing list, subscriber, segment and campaign — including irreversible\n      operations such as sending a campaign and unsubscribing an address\n      account-wide. There is no way to issue a reduced-privilege credential to an\n      integration or an agent.\n  - id: no-oauth\n    severity: medium\n    detail: >-\n      No OAuth 2.0 or OpenID Connect surface exists, so third-party applications\n      cannot act on a user's behalf without the user handing over their master\n      key. This also means no scopes/ artifact is emitted for this provider.\n  - id: no-expiry\n    severity: medium\n    detail: Keys do not expire and no rotation policy or reminder is documented.\n\nnot_applicable:\n  scopes: >-\n    scopes/ is deliberately absent. The API declares no oauth2 security scheme\n    and\
  \ the docs document no permission model, so an OAuthScopes artifact would\n    have nothing real to carry.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moosend/refs/heads/main/authentication/moosend-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Marketing
- Marketing Automation
- Campaigns
- Mailing Lists
- Subscribers
- Transactional Email
- SMTP
- Segmentation
- Analytics
- Email
- Newsletters
- Landing Pages
- Website Tracking
- Marketing
---
