---
api_key_in: []
api_specs:
- filename: cardlytics-partner-api-openapi.yml
  format: yaml
  label: Cardlytics Partner API
  slug: cardlytics-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-partner-api-openapi.yml
- filename: cardlytics-campaign-build-api-openapi.yml
  format: yaml
  label: Cardlytics Campaign Build API
  slug: cardlytics-campaign-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-campaign-build-api-openapi.yml
- filename: cardlytics-publisher-api-openapi.yml
  format: yaml
  label: Cardlytics Publisher API v2
  slug: cardlytics-publisher-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/openapi/cardlytics-publisher-api-openapi.yml
auth_types:
- oauth2
- mutualTLS
- http
- custom-session-token
description: ''
kind: authentication
layout: security
method: searched
name: Cardlytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cardlytics secures its APIs with oauth2, mutualTLS, http, and custom-session-token across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cardlytics
provider_slug: cardlytics
scheme_count: 6
schemes:
- additional_controls:
  - API scopes
  - optional IP allow-listing
  api: Partner API (advertiser merchant + offer ingestion)
  credentials: Cardlytics issues a unique client_id and client_secret per partner.
  docs: https://platform.cardlytics.com/advertisers/docs/api-get-started
  flows:
  - absolute_token_url: https://api.cardlytics.com/api/v1/idp/oauth2/token
    flow: clientCredentials
    scopes: 1
    tokenUrl: /v1/idp/oauth2/token
  name: oauth2
  sources:
  - openapi/cardlytics-partner-api-openapi.yml
  type: oauth2
- api: Campaign Build API (Ads Manager advertiser campaign objects)
  flows:
  - authorizationUrl: https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/token
  name: oauth2-cognito
  note: The spec ships the PRE-PRODUCTION Amazon Cognito user pool (advertiser-auth-preprod). Cardlytics publishes no production authorization server URL for this API, and no anonymous OIDC discovery document is served.
  sources:
  - openapi/cardlytics-campaign-build-api-openapi.yml
  token_name: id_token
  type: oauth2
- api: Publisher API v2 (financial-institution rewards platform)
  description: Publisher traffic runs over two-way TLS plus an IP-address allow list. The publisher generates an RSA private key and CSR (a separate certificate for pre-production and production); Cardlytics signs it and returns client.crt. Sandbox and production endpoints both require the client certificate on every call.
  name: mutualTLS
  sources:
  - https://docs.cardlytics.com/ads/v2/integrations/connectivity-via-mTLS.html
  type: mutualTLS
- api: Publisher API v2
  expiry_behavior: A 401 is returned when the session expires, with no distinguishing body; clients must cache tokens and re-call startSession on 401.
  in: header
  name: X-CDLX-Session-Token
  obtained_via: POST /v2/session/startSession
  parameter_name: X-CDLX-Session-Token
  scopes:
  - api:institution
  - api:customer
  sources:
  - openapi/cardlytics-publisher-api-openapi.yml
  - https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html
  token_format: JSON Web Token encoding institution and customer metadata
  type: apiKey
- algorithm: HS256
  api: Powered by Cardlytics marketplace webhooks + SDK
  bearerFormat: JWT
  name: Cardlytics JWT (Powered by Cardlytics)
  required_claims:
  - iss (the Cardlytics-assigned applicationId, form cdlx:<uuid>)
  - sub (hex-encoded MD5 digest of the JSON request body)
  - exp (no more than 60 minutes in the future)
  - jti (random uuid)
  scheme: bearer
  signing_key: shared secretKey issued by Cardlytics per applicationId
  sources:
  - https://docs.cardlytics.com/poweredby/api-reference-authentication.html
  type: http
- api: CSR API (customer-service representative tooling)
  authorization_server: Ping Identity
  flows:
  - flow: clientCredentials
    note: app-to-app, backend integrations
  - flow: authorizationCode
    note: user-to-app; supports FI SSO federation to the bank's own IdP
    pkce: true
  header: 'Authorization: Bearer {access_token}'
  name: OAuth 2.0 (CSR / servicing API)
  sources:
  - https://docs.cardlytics.com/csr/common/authentication.html
  type: oauth2
slug: cardlytics-authentication
source_filename: cardlytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/cardlytics-campaign-build-api-openapi.yml, openapi/cardlytics-partner-api-openapi.yml, openapi/cardlytics-publisher-api-openapi.yml\ndocs:\n- https://platform.cardlytics.com/advertisers/docs/api-get-started\n- https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html\n- https://docs.cardlytics.com/ads/v2/integrations/connectivity-via-mTLS.html\n- https://docs.cardlytics.com/poweredby/api-reference-authentication.html\n- https://docs.cardlytics.com/csr/common/authentication.html\nsummary:\n  types:\n  - oauth2\n  - mutualTLS\n  - http\n  - custom-session-token\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  note: >-\n    Cardlytics runs four distinct authentication models across four API families.\n    Nothing is self-service — every credential (OAuth client, mTLS client\n    certificate, JWT secretKey, SDK applicationId) is issued by a Cardlytics\n    account manager or integration\
  \ consultant after a partner agreement.\nschemes:\n- name: oauth2\n  type: oauth2\n  api: Partner API (advertiser merchant + offer ingestion)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/idp/oauth2/token\n    absolute_token_url: https://api.cardlytics.com/api/v1/idp/oauth2/token\n    scopes: 1\n  credentials: Cardlytics issues a unique client_id and client_secret per partner.\n  additional_controls:\n  - API scopes\n  - optional IP allow-listing\n  sources:\n  - openapi/cardlytics-partner-api-openapi.yml\n  docs: https://platform.cardlytics.com/advertisers/docs/api-get-started\n- name: oauth2-cognito\n  type: oauth2\n  api: Campaign Build API (Ads Manager advertiser campaign objects)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://advertiser-auth-preprod.auth.us-east-1.amazoncognito.com/oauth2/token\n    scopes: 1\n  token_name: id_token\n  sources:\n  - openapi/cardlytics-campaign-build-api-openapi.yml\n\
  \  note: >-\n    The spec ships the PRE-PRODUCTION Amazon Cognito user pool\n    (advertiser-auth-preprod). Cardlytics publishes no production authorization\n    server URL for this API, and no anonymous OIDC discovery document is served.\n- name: mutualTLS\n  type: mutualTLS\n  api: Publisher API v2 (financial-institution rewards platform)\n  sources:\n  - https://docs.cardlytics.com/ads/v2/integrations/connectivity-via-mTLS.html\n  description: >-\n    Publisher traffic runs over two-way TLS plus an IP-address allow list.\n    The publisher generates an RSA private key and CSR (a separate certificate\n    for pre-production and production); Cardlytics signs it and returns\n    client.crt. Sandbox and production endpoints both require the client\n    certificate on every call.\n- name: X-CDLX-Session-Token\n  type: apiKey\n  in: header\n  parameter_name: X-CDLX-Session-Token\n  api: Publisher API v2\n  obtained_via: POST /v2/session/startSession\n  token_format: JSON Web Token encoding\
  \ institution and customer metadata\n  expiry_behavior: >-\n    A 401 is returned when the session expires, with no distinguishing body;\n    clients must cache tokens and re-call startSession on 401.\n  scopes:\n  - api:institution\n  - api:customer\n  sources:\n  - openapi/cardlytics-publisher-api-openapi.yml\n  - https://docs.cardlytics.com/ads/v2/getting-started/get-session-token.html\n- name: Cardlytics JWT (Powered by Cardlytics)\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  api: Powered by Cardlytics marketplace webhooks + SDK\n  algorithm: HS256\n  signing_key: shared secretKey issued by Cardlytics per applicationId\n  required_claims:\n  - iss (the Cardlytics-assigned applicationId, form cdlx:<uuid>)\n  - sub (hex-encoded MD5 digest of the JSON request body)\n  - exp (no more than 60 minutes in the future)\n  - jti (random uuid)\n  sources:\n  - https://docs.cardlytics.com/poweredby/api-reference-authentication.html\n- name: OAuth 2.0 (CSR / servicing API)\n  type: oauth2\n\
  \  api: CSR API (customer-service representative tooling)\n  authorization_server: Ping Identity\n  flows:\n  - flow: clientCredentials\n    note: app-to-app, backend integrations\n  - flow: authorizationCode\n    pkce: true\n    note: user-to-app; supports FI SSO federation to the bank's own IdP\n  header: 'Authorization: Bearer {access_token}'\n  sources:\n  - https://docs.cardlytics.com/csr/common/authentication.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/authentication/cardlytics-authentication.yml
summary_line: oauth2/mutualTLS/http/custom-session-token · 6 schemes
tags:
- Company
- Advertising
- Commerce Media
- Card-Linked Offers
- Purchase Intelligence
- Financial Services
- Loyalty and Rewards
- Marketing
- Banking
- Retail Media
- Attribution
- Offers
---
