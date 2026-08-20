---
api_key_in:
- header
- query
api_specs:
- filename: brandwatch-consumer-research-openapi.yml
  format: yaml
  label: Brandwatch Consumer Research API
  slug: consumer-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-consumer-research-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Brandwatch Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Brandwatch secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Brandwatch
provider_slug: brandwatch
scheme_count: 3
schemes:
- format: 'Authorization: bearer <ACCESS_TOKEN>'
  name: bearer-token
  note: 'The spec models this as `type: apiKey, in: header, name: Authorization` with `x-bearer-format: bearer`; the docs describe the same thing as a bearer token.'
  parameter: Authorization
  scheme: bearer
  sources:
  - https://developers.brandwatch.com/docs/authenticate
  - openapi/brandwatch-consumer-research-authentication-openapi.yml
  type: http
- in: query
  name: access-token-query-parameter
  note: 'The docs explicitly permit passing the token in the URL as `&access_token=[ACCESS TOKEN]`. This is a real published alternative and it is a weakness worth flagging: tokens in query strings leak into proxy logs, browser history and Referer headers, and these tokens are valid for a year by default.'
  parameter: access_token
  sources:
  - https://developers.brandwatch.com/docs/authenticate
  type: apiKey
- flows:
  - client_id: brandwatch-api-client
    flow: password
    grant_type: api-password
    scopes_returned:
    - read
    - trust
    - write
    tokenUrl: https://api.brandwatch.com/oauth/token
  name: oauth2-token-endpoint
  note: 'The published spec declares `clientCredentials` with `tokenUrl: https://example.com/oauth2/token` — a ReadMe scaffold default that was never filled in. The real endpoint and grant, per the provider''s own authentication page, are recorded above. The spec value is left untouched in openapi/; the correction lives here and in overlays/brandwatch-consumer-research-overlay.yaml.'
  sources:
  - https://developers.brandwatch.com/docs/authenticate
  - openapi/brandwatch-consumer-research-openapi.yml
  type: oauth2
slug: brandwatch-authentication
source_filename: brandwatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/brandwatch-consumer-research-authentication-openapi.yml, openapi/brandwatch-consumer-research-openapi.yml\ndocs: https://developers.brandwatch.com/docs/authenticate\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n    - query\n  oauth2_flows:\n    - password\n  token_endpoint: https://api.brandwatch.com/oauth/token\n  token_lifetime_seconds: 31535999\n  token_lifetime_note: one year by default for an API User\nmodel: >-\n  Brandwatch uses a single bearer access token for the whole Consumer Research\n  API surface. The token is minted from an OAuth 2.0-shaped token endpoint using\n  a Brandwatch-specific `grant_type=api-password` with the account's own username\n  and password plus a fixed `client_id` of `brandwatch-api-client` — it is a\n  resource-owner-password exchange, not a client-credentials one, despite what\n  the published spec declares. The same token is then presented on every\
  \ request.\nschemes:\n  - name: bearer-token\n    type: http\n    scheme: bearer\n    parameter: Authorization\n    format: 'Authorization: bearer <ACCESS_TOKEN>'\n    sources:\n      - https://developers.brandwatch.com/docs/authenticate\n      - openapi/brandwatch-consumer-research-authentication-openapi.yml\n    note: >-\n      The spec models this as `type: apiKey, in: header, name: Authorization`\n      with `x-bearer-format: bearer`; the docs describe the same thing as a\n      bearer token.\n  - name: access-token-query-parameter\n    type: apiKey\n    in: query\n    parameter: access_token\n    sources:\n      - https://developers.brandwatch.com/docs/authenticate\n    note: >-\n      The docs explicitly permit passing the token in the URL as\n      `&access_token=[ACCESS TOKEN]`. This is a real published alternative and\n      it is a weakness worth flagging: tokens in query strings leak into proxy\n      logs, browser history and Referer headers, and these tokens are valid for\n\
  \      a year by default.\n  - name: oauth2-token-endpoint\n    type: oauth2\n    flows:\n      - flow: password\n        tokenUrl: https://api.brandwatch.com/oauth/token\n        grant_type: api-password\n        client_id: brandwatch-api-client\n        scopes_returned:\n          - read\n          - trust\n          - write\n    sources:\n      - https://developers.brandwatch.com/docs/authenticate\n      - openapi/brandwatch-consumer-research-openapi.yml\n    note: >-\n      The published spec declares `clientCredentials` with\n      `tokenUrl: https://example.com/oauth2/token` — a ReadMe scaffold default\n      that was never filled in. The real endpoint and grant, per the provider's\n      own authentication page, are recorded above. The spec value is left\n      untouched in openapi/; the correction lives here and in\n      overlays/brandwatch-consumer-research-overlay.yaml.\nmulti_tenancy:\n  parameter: platform_client_id\n  applies_to: token request\n  docs: https://developers.brandwatch.com/docs/authenticate\n\
  \  note: >-\n    Accounts using Consumer Research organization switching must pass an\n    additional `platform_client_id` on the token request to bind the token to\n    the right Consumer Research client. The list of valid platform client IDs is\n    not self-service — the docs say to ask Brandwatch support for it.\naccess_prerequisites:\n  - Only \"Regular\" or \"Admin\" Consumer Research users can call the API at all.\n  - The Data Upload API must be enabled per-account by a Customer Success Manager.\n  - The Analysis API is not in standard contracts; it is sold on a cost-per-query basis.\ngaps:\n  - No self-service credential issuance — every path to a token runs through an existing paid seat.\n  - No documented token refresh or revocation endpoint.\n  - No scope selection at token-request time; the token comes back with whatever the user already has.\n  - No mTLS, no OIDC discovery document, no JWKS endpoint published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/authentication/brandwatch-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Analytics
- Social-Media
- Social Media Monitoring
- Consumer Intelligence
- Brand Management
- Sentiment Analysis
---
