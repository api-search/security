---
api_key_in:
- query
- body
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Storyclash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Storyclash secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Storyclash
provider_slug: storyclash
scheme_count: 2
schemes:
- applies_to:
  - GET /external-api/campaign/{campaign_id}
  - GET /external-api/campaigns
  description: Opaque per-customer token issued by Storyclash. Appended to the request URL on the Campaign Data and All Campaigns endpoints, e.g. GET https://app.storyclash.com/external-api/campaigns?token={YOUR_AUTH_TOKEN}
  in: query
  name: apiToken
  parameter: token
  sources:
  - https://storyclash.notion.site/Storyclash-API-Documentation-1266dc2ddd0880a79cf9e3d34c19fa01
  type: apiKey
- applies_to:
  - POST /external-api/import/creator
  description: The same token supplied as the "token" field of the JSON request body on the creator import endpoint.
  in: body
  name: apiTokenBody
  parameter: token
  sources:
  - https://storyclash.notion.site/Storyclash-API-Documentation-1266dc2ddd0880a79cf9e3d34c19fa01
  type: apiKey
slug: storyclash-authentication
source_filename: storyclash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://storyclash.notion.site/Storyclash-API-Documentation-1266dc2ddd0880a79cf9e3d34c19fa01\ndocs: https://storyclash.notion.site/Storyclash-API-Documentation-1266dc2ddd0880a79cf9e3d34c19fa01\nalso: https://www.storyclash.com/integrations/api-integration\ncorrection: >-\n  Supersedes the 2026-07-21 profile, which recorded the token as an apiKey in a request\n  HEADER. The provider's own API documentation shows it is a QUERY PARAMETER on the two GET\n  endpoints (?token={YOUR_AUTH_TOKEN}) and a JSON BODY FIELD on the POST creator-import\n  endpoint. Verified against a live unauthenticated call to\n  https://app.storyclash.com/external-api/campaigns, which returns HTTP 200 with\n  {\"message\":\"Invalid API Key\"} — an error body, not a 401 challenge, and no\n  WWW-Authenticate header.\nsummary:\n  types: [apiKey]\n  api_key_in: [query, body]\n  oauth2_flows: []\n  notes: >-\n    Storyclash publishes no machine-readable OpenAPI.\
  \ A single opaque per-customer token is\n    the whole authentication model. There is no OAuth2, no OpenID Connect, no scope surface\n    and no refresh/rotation mechanism documented, so scopes/ is not applicable. The token is\n    provisioned by Storyclash (enterprise arrangement, \"Get API access\" / \"Request Enterprise\n    Demo\"), not self-issued from a dashboard.\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: query\n    parameter: token\n    description: >-\n      Opaque per-customer token issued by Storyclash. Appended to the request URL on the\n      Campaign Data and All Campaigns endpoints, e.g.\n      GET https://app.storyclash.com/external-api/campaigns?token={YOUR_AUTH_TOKEN}\n    applies_to:\n      - GET /external-api/campaign/{campaign_id}\n      - GET /external-api/campaigns\n    sources: [https://storyclash.notion.site/Storyclash-API-Documentation-1266dc2ddd0880a79cf9e3d34c19fa01]\n  - name: apiTokenBody\n    type: apiKey\n    in: body\n    parameter: token\n\
  \    description: >-\n      The same token supplied as the \"token\" field of the JSON request body on the creator\n      import endpoint.\n    applies_to:\n      - POST /external-api/import/creator\n    sources: [https://storyclash.notion.site/Storyclash-API-Documentation-1266dc2ddd0880a79cf9e3d34c19fa01]\nfailure_modes:\n  - condition: token missing or invalid\n    observed_status: 200\n    body: '{\"message\":\"Invalid API Key\"}'\n    note: >-\n      Probed 2026-08-13 on https://app.storyclash.com/external-api/campaigns. The API returns\n      200 with a JSON error envelope rather than 401/403, so a client cannot rely on the HTTP\n      status to detect an auth failure and must inspect the body.\n  - condition: token valid but the feature is not enabled for that customer\n    documented_message: Invalid API Key\n    note: >-\n      The creator-import error table lists \"The supplied token is not valid or the feature is\n      not active for that token\" as producing the same \"Invalid\
  \ API Key\" response, so\n      authorization failures are indistinguishable from authentication failures.\ntransport:\n  https: true\n  hsts: true\n  note: app.storyclash.com sends strict-transport-security max-age=31536000; includeSubDomains; preload.\nsecurity_observations:\n  - >-\n      The token travels in the query string on GET requests, so it is exposed to proxy logs,\n      browser history and Referer headers. There is no header-based alternative documented.\n  - No token rotation, expiry or revocation procedure is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storyclash/refs/heads/main/authentication/storyclash-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Influencer Marketing
- Creator Economy
- Social Media Analytics
- Marketing Analytics
- Campaign Management
- Business Intelligence
- REST API
- Webhook
---
