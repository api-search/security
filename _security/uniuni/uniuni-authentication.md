---
api_key_in:
- header
api_specs:
- filename: uniuni-platform-client-api-openapi.yml
  format: yaml
  label: UniUni Platform Client API
  slug: uniuni-platform-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniuni/refs/heads/main/openapi/uniuni-platform-client-api-openapi.yml
auth_types:
- http-bearer
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Uniuni Authentication
name_suffix: Authentication
oauth_flows: []
overview: UniUni secures its APIs with http-bearer and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UniUni
provider_slug: uniuni
scheme_count: 3
schemes:
- api: UniUni Platform Client API
  description: 'API access token generated from the UniUni Platform dashboard (New shipment → Import from integration → REST API). Up to 5 active tokens; deleting a token revokes access immediately. Sent as Authorization: Bearer <ACCESS_TOKEN> on every request.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/uniuni-platform-client-api-openapi.yml
  token_management:
    max_active_tokens: 5
    portal_production: https://ship.uniuni.com/integrations/rest-api
    portal_sandbox: https://sandbox.unigo.ca/integrations/rest-api
  type: http
- api: UniUni Partner API
  description: 'Partner vendors exchange an X-API-Key for a JWT access token via GET https://api.ship.uniuni.com/partner/auth/token; the JWT (valid 24 hours) is then sent as Authorization: Bearer <accessToken>. Keys are issued by a UniUni account representative.'
  error_codes:
  - MissingTokenError
  - ExpiredTokenError
  - InvalidTokenError
  - TokenPayloadError
  in: header
  name: partnerApiKey
  parameter: X-API-Key
  token_ttl_seconds: 86400
  type: apiKey
- api: UniUni Integration API (legacy)
  description: 'The legacy Integration API (docs.uniuni.com) obtains a customer token via POST /storeauth/customertoken?grant_type=client_crendetials using a UniUni-issued Client ID and Client Secret, then sends the token on subsequent requests. Base hosts: https://prm-api.uniuni.com (production), https://prm-api.qa.uniuni.com (QA).'
  name: integrationClientCredentials
  type: apiKey
slug: uniuni-authentication
source_filename: uniuni-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.ship.uniuni.com/en/api/create-access-token\ndocs:\n  - https://help.ship.uniuni.com/en/api/create-access-token\n  - https://help.ship.uniuni.com/en/partner-api/authentication\n  - https://docs.uniuni.com/\nsummary:\n  types: [http-bearer, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    api: UniUni Platform Client API\n    description: >-\n      API access token generated from the UniUni Platform dashboard (New shipment → Import from\n      integration → REST API). Up to 5 active tokens; deleting a token revokes access\n      immediately. Sent as Authorization: Bearer <ACCESS_TOKEN> on every request.\n    token_management:\n      max_active_tokens: 5\n      portal_production: https://ship.uniuni.com/integrations/rest-api\n      portal_sandbox: https://sandbox.unigo.ca/integrations/rest-api\n    sources: [openapi/uniuni-platform-client-api-openapi.yml]\n\
  \  - name: partnerApiKey\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    api: UniUni Partner API\n    description: >-\n      Partner vendors exchange an X-API-Key for a JWT access token via GET\n      https://api.ship.uniuni.com/partner/auth/token; the JWT (valid 24 hours) is then sent as\n      Authorization: Bearer <accessToken>. Keys are issued by a UniUni account representative.\n    token_ttl_seconds: 86400\n    error_codes: [MissingTokenError, ExpiredTokenError, InvalidTokenError, TokenPayloadError]\n  - name: integrationClientCredentials\n    type: apiKey\n    api: UniUni Integration API (legacy)\n    description: >-\n      The legacy Integration API (docs.uniuni.com) obtains a customer token via POST\n      /storeauth/customertoken?grant_type=client_crendetials using a UniUni-issued Client ID and\n      Client Secret, then sends the token on subsequent requests. Base hosts:\n      https://prm-api.uniuni.com (production), https://prm-api.qa.uniuni.com (QA).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniuni/refs/heads/main/authentication/uniuni-authentication.yml
summary_line: http-bearer/apiKey · 3 schemes
tags:
- Company
- Logistics
- Shipping
- Last-Mile Delivery
- Ecommerce
- Tracking
- Delivery
---
