---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Crazy Egg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crazy Egg declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Crazy Egg
provider_slug: crazyegg
scheme_count: 2
schemes:
- access_levels:
  - read-only
  - read & write
  api: crazyegg:platform-api
  expiry: Tokens created on the settings page do not expire; a token with an expiry date is rejected with "Expired token" once that date passes.
  header: 'Authorization: Bearer ce_pat_...'
  issuance: Created in account settings at https://auth.app.crazyegg.com/settings under Personal Access Tokens; shown only once.
  name: personalAccessToken
  notes:
  - Read-only tokens are rejected for every mutation ("Personal access token is read-only").
  - A token has the creating user's role and site access in the account; some features depend on the account's subscription.
  - The app endpoint /gql rejects personal access tokens; integrations must use /api.
  - Subscriptions are not supported for personal access token integrations.
  - Send only from servers; the API does not accept browser requests from other websites.
  revocation: Revoke stops a token immediately; a revoked token stays listed until deleted.
  scheme: bearer
  token_prefix: ce_pat_
  type: http
- api: crazyegg:conversion-tracking-api
  header: 'Authorization: key YOUR_API_KEY'
  in: header
  issuance: Enable the Conversion Tracking API Key for the site under Options > site Settings > API Keys.
  name: siteApiKey
  source: https://support.crazyegg.com/knowledge-base/conversion-tracking-api/
  type: apiKey
slug: crazyegg-authentication
source_filename: crazyegg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://platform-api-docs.crazyegg.com/guides/getting-started\ndocs: https://platform-api-docs.crazyegg.com/guides/getting-started\nschemes:\n- name: personalAccessToken\n  api: crazyegg:platform-api\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer ce_pat_...'\n  token_prefix: ce_pat_\n  access_levels: [read-only, read & write]\n  issuance: Created in account settings at https://auth.app.crazyegg.com/settings under Personal Access Tokens; shown only once.\n  expiry: Tokens created on the settings page do not expire; a token with an expiry date is rejected with \"Expired token\" once that date passes.\n  revocation: Revoke stops a token immediately; a revoked token stays listed until deleted.\n  notes:\n  - Read-only tokens are rejected for every mutation (\"Personal access token is read-only\").\n  - A token has the creating user's role and site access in the account; some features depend on the account's subscription.\n\
  \  - The app endpoint /gql rejects personal access tokens; integrations must use /api.\n  - Subscriptions are not supported for personal access token integrations.\n  - Send only from servers; the API does not accept browser requests from other websites.\n- name: siteApiKey\n  api: crazyegg:conversion-tracking-api\n  type: apiKey\n  in: header\n  header: 'Authorization: key YOUR_API_KEY'\n  issuance: Enable the Conversion Tracking API Key for the site under Options > site Settings > API Keys.\n  source: https://support.crazyegg.com/knowledge-base/conversion-tracking-api/\n"
source_yaml_url: https://artifacts.apis.io/crazyegg/authentication/crazyegg-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Analytics
- Heatmaps
- Session Recording
- A/B Testing
- Conversion Optimization
- GraphQL
- MCP
---
