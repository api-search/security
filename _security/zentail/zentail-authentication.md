---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zentail Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zentail secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zentail
provider_slug: zentail
scheme_count: 2
schemes:
- description: Zentail's Open API authenticates with a per-account API token. Generate it in the Zentail app under Account Settings > API Access > GENERATE NEW TOKEN (Account Admin permission is required to view/create tokens). Tokens can be labeled and revoked; keep the token secret.
  docs: https://help.zentail.com/en/articles/1460332-generate-api-token
  in: header
  name: OpenAPIToken
  sources:
  - searched:help.zentail.com
  type: apiKey
- description: The Sales Channel / Listings API (used to build custom sales-channel, inventory, and fulfillment integrations) authenticates integrators with a clientId and clientSecret to obtain access to its endpoints.
  docs: https://help.zentail.com/en/articles/4430986-creating-a-new-sales-channel-integration-for-zentail
  flow: clientCredentials
  name: SalesChannelClientCredentials
  sources:
  - searched:help.zentail.com
  type: oauth2
slug: zentail-authentication
source_filename: zentail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.zentail.com/en/collections/96118-open-api\ndocs: https://help.zentail.com/en/articles/1460332-generate-api-token\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: OpenAPIToken\n  type: apiKey\n  in: header\n  description: >-\n    Zentail's Open API authenticates with a per-account API token. Generate it in the\n    Zentail app under Account Settings > API Access > GENERATE NEW TOKEN (Account Admin\n    permission is required to view/create tokens). Tokens can be labeled and revoked;\n    keep the token secret.\n  docs: https://help.zentail.com/en/articles/1460332-generate-api-token\n  sources: [searched:help.zentail.com]\n- name: SalesChannelClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    The Sales Channel / Listings API (used to build custom sales-channel, inventory,\n    and fulfillment integrations) authenticates\
  \ integrators with a clientId and\n    clientSecret to obtain access to its endpoints.\n  docs: https://help.zentail.com/en/articles/4430986-creating-a-new-sales-channel-integration-for-zentail\n  sources: [searched:help.zentail.com]\nnotes: >-\n  Two distinct auth models: (1) the Open API uses an account-scoped API token\n  (apiKey, header); (2) the Sales Channel / Listings API uses clientId + clientSecret\n  (OAuth2 client-credentials style). Separately, the Zentail web application signs in\n  via signin.zentail.com (WorkOS AuthKit OIDC) — that governs app SSO, not API access.\n  Exact token header name and Sales Channel token endpoint are documented in the\n  Stoplight developer portal (developer.zentail.com), which renders client-side and\n  was not machine-extractable in this pass.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zentail/refs/heads/main/authentication/zentail-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Ecommerce
- Multichannel
- Marketplace
- Product Information Management
- Inventory Management
- Order Management
- Listing Management
- Retail
---
