---
api_key_in:
- cookie
api_specs:
- filename: ankorstore-main-openapi-original.yml
  format: yaml
  label: Ankorstore Public API
  slug: ankorstore-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankorstore/refs/heads/main/openapi/ankorstore-main-openapi-original.yml
- filename: ankorstore-astral-openapi-original.yml
  format: yaml
  label: Ankorstore Stock Tracking and Logistics API (ASTRAL)
  slug: ankorstore-stock-tracking-and-logistics-api-astral
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankorstore/refs/heads/main/openapi/ankorstore-astral-openapi-original.yml
- filename: ankorstore-fulfillment-openapi-original.yml
  format: yaml
  label: Ankorstore Fulfillment Service API
  slug: ankorstore-fulfillment-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankorstore/refs/heads/main/openapi/ankorstore-fulfillment-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ankorstore Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ankorstore secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ankorstore
provider_slug: ankorstore
scheme_count: 2
schemes:
- in: cookie
  name: CookieKey
  parameter: ankorstore_session
  sources:
  - openapi/ankorstore-astral-openapi-original.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://www.ankorstore.com/oauth/token
  name: ProductionOAuth2ClientCredentials
  sources:
  - openapi/ankorstore-main-openapi-original.yml
  type: oauth2
slug: ankorstore-authentication
source_filename: ankorstore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/ankorstore-astral-openapi-original.yml, openapi/ankorstore-main-openapi-original.yml\ndocs: https://ankorstore.github.io/api-docs/#section/Authentication\nnotes: >-\n  The Ankorstore Public API uses OAuth2 Client Credentials. Exchange client_id/client_secret at\n  POST https://www.ankorstore.com/oauth/token (sandbox: https://www.public.ankorstore-sandbox.com/oauth/token)\n  with scope=* to receive a Bearer token valid for 3600s. The /oauth/token endpoint is rate-limited to\n  60 requests/hour. Applications and their client credentials are created in the Integrations area of the\n  Ankorstore account (https://ankorstore.com/account/integrations). The ASTRAL spec additionally declares a\n  session-cookie apiKey scheme (ankorstore_session) for browser-context calls.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: CookieKey\n  type: apiKey\n\
  \  in: cookie\n  parameter: ankorstore_session\n  sources:\n  - openapi/ankorstore-astral-openapi-original.yml\n- name: ProductionOAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.ankorstore.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/ankorstore-main-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ankorstore/refs/heads/main/authentication/ankorstore-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Retail
- Wholesale
- Marketplace
- E-commerce
- Ordering
- Fulfillment
- Catalog
- Webhooks
- JSON:API
---
