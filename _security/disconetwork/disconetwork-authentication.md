---
api_key_in:
- header
api_specs:
- filename: disconetwork-partner-api.yml
  format: yaml
  label: Disco Partner Integration API
  slug: disconetwork-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/openapi/disconetwork-partner-api.yml
- filename: disconetwork-reporting-api-v1.yml
  format: yaml
  label: Disco Reporting API
  slug: disconetwork-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/openapi/disconetwork-reporting-api-v1.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Disconetwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Disconetwork secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Disconetwork
provider_slug: disconetwork
scheme_count: 2
schemes:
- applies_to:
  - Disco Partner Integration API (partners.disconetwork.com)
  description: 'Key Auth: Requests contain a valid `x-api-key` in the request headers.'
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/disconetwork-partner-api.yml
  type: apiKey
- applies_to:
  - DiscoBeat Channel API (api.disconetwork.com)
  - Disco Reporting API V1 (api.disconetwork.com)
  - Disco Reporting API V2 (api.disconetwork.com)
  description: The DiscoBeat management API key. The same key authenticates the DiscoBeat Channel API and both versions of the Reporting API.
  in: header
  name: ManagementApiKey
  parameter: x-api-key
  sources:
  - openapi/disconetwork-reporting-api-v1.yml
  - openapi/disconetwork-reporting-api-v2.yml
  - https://disconetwork.com/developers/discobeat
  type: apiKey
slug: disconetwork-authentication
source_filename: disconetwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://disconetwork.com/developers/discobeat\ndocs:\n- https://disconetwork.com/developers/discobeat\n- https://docs.disconetwork.com/docs/api-ref/external-api-for-disco-integration-partners\n- https://disconetwork.com/reporting-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: Every Disco API surface authenticates with a static API key in the `x-api-key`\n    request header. There is no OAuth, no OIDC and no token exchange. Keys are issued\n    by a Disco representative, not through self-service; there is no public key-minting\n    endpoint.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Key Auth: Requests contain a valid `x-api-key` in the request headers.'\n  applies_to:\n  - Disco Partner Integration API (partners.disconetwork.com)\n  sources:\n  - openapi/disconetwork-partner-api.yml\n\
  - name: ManagementApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The DiscoBeat management API key. The same key authenticates the DiscoBeat\n    Channel API and both versions of the Reporting API.\n  applies_to:\n  - DiscoBeat Channel API (api.disconetwork.com)\n  - Disco Reporting API V1 (api.disconetwork.com)\n  - Disco Reporting API V2 (api.disconetwork.com)\n  sources:\n  - openapi/disconetwork-reporting-api-v1.yml\n  - openapi/disconetwork-reporting-api-v2.yml\n  - https://disconetwork.com/developers/discobeat\nkey_classes:\n- class: secret / management key\n  usage: Server-to-server. Authenticates the DiscoBeat Channel API and the Reporting\n    API.\n  transport: x-api-key header\n- class: publishable key\n  usage: Referenced in the DiscoBeat docs alongside the secret key; the docs draw a\n    secret-vs-publishable distinction but do not publish the publishable key's own\n    call surface.\n  transport: not documented publicly\n  observed_prefix_example:\
  \ disco_pk_live_ (shown in a DiscoBeat publisher-detail response\n    example on https://disconetwork.com/developers/discobeat)\nenvironment_binding:\n  documented: true\n  rule: Keys are environment-specific. A staging key works only against the staging\n    base URL and a production key only against production.\n  mismatch_behavior: HTTP 401 with the message \"API key environment does not match\n    service environment.\"\n  source: https://disconetwork.com/developers/discobeat\nfailure_modes:\n- status: 401\n  body: '{\"detail\": \"Invalid or expired API key.\"}'\n  cause: invalid, expired or missing key\n  source: https://disconetwork.com/developers/discobeat\n- status: 401\n  cause: missing or invalid management API key on a Reporting API request\n  source: openapi/disconetwork-reporting-api-v1.yml\nprovisioning:\n  self_service: false\n  how: A Disco representative issues the management API key; partners request one via\n    https://disconetwork.com/book-a-demo.\n  rotation_policy_published:\
  \ false\nnotes:\n- The Disco Event API (https://consumer.disconetwork.com/api/events) is documented\n  without an authentication header; identity is carried in the payload as a raw email,\n  a SHA-256 email hash, or a click identifier, plus the publisher account_id.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/authentication/disconetwork-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Commerce Media
- Retail Media
- Post-Purchase
- Advertising
- Ecommerce
- AdTech
- Marketing
- Analytics
- Reporting
---
