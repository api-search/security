---
api_key_in: []
api_specs:
- filename: kard-attributions-api-openapi.yml
  format: yaml
  label: Kard attributions API
  slug: kard-attributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-attributions-api-openapi.yml
- filename: kard-files-api-openapi.yml
  format: yaml
  label: Kard Files API
  slug: kard-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-files-api-openapi.yml
- filename: kard-notifications-notifications-api-openapi.yml
  format: yaml
  label: Kard notifications > Notifications API
  slug: kard-notifications-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-notifications-notifications-api-openapi.yml
- filename: kard-notifications-subscriptions-api-openapi.yml
  format: yaml
  label: Kard notifications > Subscriptions API
  slug: kard-notifications-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-notifications-subscriptions-api-openapi.yml
- filename: kard-organizations-api-openapi.yml
  format: yaml
  label: Kard Organizations API
  slug: kard-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-api-openapi.yml
- filename: kard-organizations-children-api-openapi.yml
  format: yaml
  label: Kard Organizations > Children API
  slug: kard-organizations-children-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-children-api-openapi.yml
- filename: kard-organizations-contentstrategies-api-openapi.yml
  format: yaml
  label: Kard Organizations > ContentStrategies API
  slug: kard-organizations-contentstrategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-contentstrategies-api-openapi.yml
- filename: kard-organizations-placements-api-openapi.yml
  format: yaml
  label: Kard Organizations > Placements API
  slug: kard-organizations-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-organizations-placements-api-openapi.yml
- filename: kard-ping-api-openapi.yml
  format: yaml
  label: Kard Ping API
  slug: kard-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-ping-api-openapi.yml
- filename: kard-rewards-api-openapi.yml
  format: yaml
  label: Kard rewards API
  slug: kard-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-rewards-api-openapi.yml
- filename: kard-transactions-api-openapi.yml
  format: yaml
  label: Kard transactions API
  slug: kard-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-transactions-api-openapi.yml
- filename: kard-users-api-openapi.yml
  format: yaml
  label: Kard users API
  slug: kard-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-api-openapi.yml
- filename: kard-users-attributions-api-openapi.yml
  format: yaml
  label: Kard users > attributions API
  slug: kard-users-attributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-attributions-api-openapi.yml
- filename: kard-users-rewards-api-openapi.yml
  format: yaml
  label: Kard users > Rewards API
  slug: kard-users-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-rewards-api-openapi.yml
- filename: kard-users-uploads-api-openapi.yml
  format: yaml
  label: Kard users > uploads API
  slug: kard-users-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-uploads-api-openapi.yml
- filename: kard-users-webview-api-openapi.yml
  format: yaml
  label: Kard users > WebView API
  slug: kard-users-webview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-users-webview-api-openapi.yml
- filename: kard-api-reference-api-openapi.yml
  format: yaml
  label: Kard API Reference API
  slug: kard-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-api-reference-api-openapi.yml
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Kard Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Kard secures its APIs with oauth2 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Kard
provider_slug: kard
scheme_count: 2
schemes:
- name: OAuthScheme
  notes: Bearer access token obtained via OAuth2 client_credentials at the /v2/auth/token endpoint.
  scheme: bearer
  sources:
  - openapi/kard-api-reference-openapi.yaml
  type: http
- name: bearer
  scheme: bearer
  sources:
  - openapi/kard-legacy-openapi.yaml
  type: http
slug: kard-authentication
source_filename: kard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kard-api-reference-openapi.yaml\ndocs: https://docs.getkard.com/api/integration-guides/authentication\nsummary:\n  types:\n  - oauth2\n  - http-bearer\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nflow:\n  grant_type: client_credentials\n  token_endpoint: https://{client-subdomain}.getkard.com/v2/auth/token\n  client_authentication: HTTP Basic with base64(client_id:client_secret) in the Authorization\n    header\n  request: grant_type=client_credentials in the request body\n  response: JSON with access_token used as a Bearer token on subsequent requests\n  token_lifetime_seconds: 3600\n  multi_issuer_header: X-Kard-Target-Issuer scopes the token to a specific issuer\n  deprecated: A legacy Amazon Cognito token endpoint exists but is being discontinued.\nschemes:\n- name: OAuthScheme\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kard-api-reference-openapi.yaml\n  notes: Bearer access token obtained\
  \ via OAuth2 client_credentials at the /v2/auth/token\n    endpoint.\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kard-legacy-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/authentication/kard-authentication.yml
summary_line: oauth2/http-bearer · 2 schemes
tags:
- Company
- Rewards
- Card-Linked Offers
- Loyalty
- Fintech
- Commerce Media
- Advertising
- Transaction
- Cashback
- Webhook
---
