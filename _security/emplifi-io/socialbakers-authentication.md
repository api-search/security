---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emplifi-io-ads-api-openapi.yml
  format: yaml
  label: Emplifi Ads API
  slug: emplifi-io-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-ads-api-openapi.yml
- filename: emplifi-io-assets-api-openapi.yml
  format: yaml
  label: Emplifi Assets API
  slug: emplifi-io-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-assets-api-openapi.yml
- filename: emplifi-io-care-api-openapi.yml
  format: yaml
  label: Emplifi Care API
  slug: emplifi-io-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-care-api-openapi.yml
- filename: emplifi-io-community-api-openapi.yml
  format: yaml
  label: Emplifi Community API
  slug: emplifi-io-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-community-api-openapi.yml
- filename: emplifi-io-listening-api-openapi.yml
  format: yaml
  label: Emplifi Listening API
  slug: emplifi-io-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-listening-api-openapi.yml
- filename: emplifi-io-posts-api-openapi.yml
  format: yaml
  label: Emplifi Posts API
  slug: emplifi-io-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-posts-api-openapi.yml
- filename: emplifi-io-profile-metrics-api-openapi.yml
  format: yaml
  label: Emplifi Profile Metrics API
  slug: emplifi-io-profile-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-profile-metrics-api-openapi.yml
- filename: emplifi-io-reference-api-openapi.yml
  format: yaml
  label: Emplifi Reference API
  slug: emplifi-io-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/openapi/emplifi-io-reference-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Socialbakers Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Emplifi secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Emplifi
provider_slug: emplifi-io
scheme_count: 2
schemes:
- description: 'HTTP Basic authorization; credentials are the API token and secret base64-encoded as `token:secret`. Sent as `Authorization: Basic <base64>`.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/_original/socialbakers-emplifi-public-api-openapi.yml
  type: http
- description: OAuth 2.0 authorization code flow. Register a Custom integration in Emplifi Settings to obtain client credentials, then exchange an authorization code for an access token.
  flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    revocationUrl: https://api.emplifi.io/oauth2/0/token/revocation
    scopes: 0
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  sources:
  - openapi/_original/socialbakers-emplifi-public-api-openapi.yml
  - https://api.emplifi.io/
  type: oauth2
slug: socialbakers-authentication
source_filename: socialbakers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.emplifi.io/\ndocs: https://api.emplifi.io/\nsummary:\n  types: [http, oauth2]\n  http_schemes: [basic]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    The Emplifi (Socialbakers) Public API v3 accepts two authentication\n    methods. HTTP Basic uses your API token and secret base64-encoded as\n    `token:secret`. OAuth 2.0 uses the authorization code flow via a Custom\n    integration created in Emplifi Settings. A custom `x-api-consumer` header\n    is also sent by first-party integrations.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authorization; credentials are the API token and secret\n      base64-encoded as `token:secret`. Sent as `Authorization: Basic <base64>`.\n    sources: [openapi/_original/socialbakers-emplifi-public-api-openapi.yml]\n  - name: oauth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://api.emplifi.io/oauth2/0/auth\n        tokenUrl: https://api.emplifi.io/oauth2/0/token\n        revocationUrl: https://api.emplifi.io/oauth2/0/token/revocation\n        scopes: 0\n    description: >-\n      OAuth 2.0 authorization code flow. Register a Custom integration in\n      Emplifi Settings to obtain client credentials, then exchange an\n      authorization code for an access token.\n    sources: [openapi/_original/socialbakers-emplifi-public-api-openapi.yml, https://api.emplifi.io/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emplifi-io/refs/heads/main/authentication/socialbakers-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Marketing
- Social Media
- Analytics
- Social Media Analytics
- Social Listening
- Marketing Analytics
- Digital Asset Management
- Customer Care
- Emplifi
---
