---
api_key_in:
- header
api_specs:
- filename: epsilon-ads-api-openapi.yml
  format: yaml
  label: Epsilon Ads API
  slug: epsilon-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-ads-api-openapi.yml
- filename: epsilon-catalog-products-api-openapi.yml
  format: yaml
  label: Epsilon Catalog Products API
  slug: epsilon-catalog-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-catalog-products-api-openapi.yml
- filename: epsilon-catalogs-api-openapi.yml
  format: yaml
  label: Epsilon Catalogs API
  slug: epsilon-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-catalogs-api-openapi.yml
- filename: epsilon-crosssellcategory-api-openapi.yml
  format: yaml
  label: Epsilon Cross Sell Category API
  slug: epsilon-crosssellcategory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-crosssellcategory-api-openapi.yml
- filename: epsilon-customers-api-openapi.yml
  format: yaml
  label: Epsilon Customers API
  slug: epsilon-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-customers-api-openapi.yml
- filename: epsilon-filtermapping-api-openapi.yml
  format: yaml
  label: Epsilon Filter Mapping API
  slug: epsilon-filtermapping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-filtermapping-api-openapi.yml
- filename: epsilon-orders-api-openapi.yml
  format: yaml
  label: Epsilon Orders API
  slug: epsilon-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/openapi/epsilon-orders-api-openapi.yml
auth_types:
- apiKey
- http-basic
- oauth2
- jwt-bearer
description: 'Epsilon Retail Media uses three overlapping credential models across one platform. The default is an HTTP Basic API key issued per team (retailer) and per environment (sandbox vs production), retrieved from the platform UI under Integration Settings. The /ads endpoints additionally accept OAuth 2.0 client-credentials bearer tokens minted at /v1/oauth2/token. The Filter Mapping and Cross-Sell Category APIs declare a JWT bearer token in the Authorization header. There is no self-service credential issuance: the team ID, API key, and OAuth client_id/client_secret are all provisioned by an Epsilon Technical Account Manager.'
kind: authentication
layout: security
method: searched
name: Epsilon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Epsilon secures its APIs with apiKey, http-basic, oauth2, and jwt-bearer across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Epsilon
provider_slug: epsilon
scheme_count: 4
schemes:
- applies_to:
  - Epsilon Retail Media Integration API (all endpoints)
  - Epsilon Retail Media Brand Pages API
  compatibility_form: 'The platform also accepts the raw API key value passed directly in the Authorization header ("Authorization: Basic <existing_api_key>") for compatibility with established client integrations — documented explicitly on the Brand Pages authentication page.'
  docs: https://developers.citrusad.com/integration/reference/before-you-start
  environments:
  - name: sandbox
    note: Separate team ID and API key; provisioned by the Technical Account Manager.
  - name: production
    note: Separate team ID and API key; values differ from sandbox.
  format: 'Authorization: Basic base64(<apiKey>:)'
  name: api-key-basic
  parameter: Authorization
  scheme: basic
  sources:
  - https://developers.citrusad.com/integration/reference/before-you-start
  - https://developers.citrusad.com/integration/reference/authentication-1
  type: http
- applies_to:
  - Epsilon Retail Media Integration API — /ads endpoints ONLY
  docs: https://developers.citrusad.com/integration/reference/oauth-20-authentication
  errors:
  - code: invalid_client
    meaning: client_id or client_secret is incorrect.
  - code: invalid_request
    meaning: Missing/invalid/duplicated parameter, or malformed request.
  expires_in: 3600
  flow: clientCredentials
  name: oauth2-client-credentials
  request: POST with Content-Type application/x-www-form-urlencoded and body grant_type=client_credentials
  restriction: 'Documented restriction: "OAuth 2.0 is only available on the /ads endpoint." Order reporting via /orders must use HTTP Basic with the secret API key.'
  scopes: []
  scopes_note: No scopes are defined or accepted. The token request takes only grant_type=client_credentials; there is no scope parameter and no scope reference page. Authorization is entirely a property of the issued client, which is why no scopes/ artifact is written for this provider.
  sources:
  - https://developers.citrusad.com/integration/reference/oauth-20-authentication
  token_endpoint: https://$BASE_URL/v1/oauth2/token
  token_endpoint_auth_method: client_secret_basic
  token_type: Bearer
  type: oauth2
- applies_to:
  - Epsilon Retail Media Filter Mapping API
  - Epsilon Retail Media Cross-Sell Category API
  description: 'Declared in the published OpenAPI for the Filter Mapping and Cross-Sell Category APIs: "For accessing the API a valid JWT must be passed in all queries in the ''Authorization'' header."'
  format: Bearer xxx.yyy.zzz (JWT)
  in: header
  name: TokenSecurity
  parameter: Authorization
  sources:
  - openapi/epsilon-retail-media-filter-mapping-openapi.json
  - openapi/epsilon-retail-media-cross-sell-category-openapi.json
  type: apiKey
- description: The security scheme as declared in the published Integration API OpenAPI. It is modelled as apiKey-in-header with x-bearer-format basic, which is the spec-level expression of the HTTP Basic API key above.
  in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/epsilon-retail-media-integration-openapi.json
  type: apiKey
  x_bearer_format: basic
slug: epsilon-authentication
source_filename: epsilon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://developers.citrusad.com/integration/reference/before-you-start,\n  https://developers.citrusad.com/integration/reference/oauth-20-authentication,\n  https://developers.citrusad.com/integration/reference/authentication-1 —\n  enriched over the profile derived from openapi/*.json securitySchemes.\ndocs: https://developers.citrusad.com/integration/reference/oauth-20-authentication\ndescription: >-\n  Epsilon Retail Media uses three overlapping credential models across one\n  platform. The default is an HTTP Basic API key issued per team (retailer) and\n  per environment (sandbox vs production), retrieved from the platform UI under\n  Integration Settings. The /ads endpoints additionally accept OAuth 2.0\n  client-credentials bearer tokens minted at /v1/oauth2/token. The Filter Mapping\n  and Cross-Sell Category APIs declare a JWT bearer token in the Authorization\n  header. There is no self-service credential issuance:\
  \ the team ID, API key, and\n  OAuth client_id/client_secret are all provisioned by an Epsilon Technical\n  Account Manager.\n\nsummary:\n  types: [apiKey, http-basic, oauth2, jwt-bearer]\n  api_key_in: [header]\n  self_service_signup: false\n  provisioning: Technical Account Manager (sandbox and production issued separately)\n\nschemes:\n- name: api-key-basic\n  type: http\n  scheme: basic\n  parameter: Authorization\n  applies_to:\n    - Epsilon Retail Media Integration API (all endpoints)\n    - Epsilon Retail Media Brand Pages API\n  format: 'Authorization: Basic base64(<apiKey>:)'\n  compatibility_form: >-\n    The platform also accepts the raw API key value passed directly in the\n    Authorization header (\"Authorization: Basic <existing_api_key>\") for\n    compatibility with established client integrations — documented explicitly on\n    the Brand Pages authentication page.\n  environments:\n    - {name: sandbox, note: 'Separate team ID and API key; provisioned by the Technical\
  \ Account Manager.'}\n    - {name: production, note: 'Separate team ID and API key; values differ from sandbox.'}\n  docs: https://developers.citrusad.com/integration/reference/before-you-start\n  sources:\n    - https://developers.citrusad.com/integration/reference/before-you-start\n    - https://developers.citrusad.com/integration/reference/authentication-1\n\n- name: oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://$BASE_URL/v1/oauth2/token\n  token_endpoint_auth_method: client_secret_basic\n  request: 'POST with Content-Type application/x-www-form-urlencoded and body grant_type=client_credentials'\n  token_type: Bearer\n  expires_in: 3600\n  scopes: []\n  scopes_note: >-\n    No scopes are defined or accepted. The token request takes only\n    grant_type=client_credentials; there is no scope parameter and no scope\n    reference page. Authorization is entirely a property of the issued client,\n    which is why no scopes/ artifact is written\
  \ for this provider.\n  applies_to:\n    - Epsilon Retail Media Integration API — /ads endpoints ONLY\n  restriction: >-\n    Documented restriction: \"OAuth 2.0 is only available on the /ads endpoint.\"\n    Order reporting via /orders must use HTTP Basic with the secret API key.\n  errors:\n    - {code: invalid_client, meaning: 'client_id or client_secret is incorrect.'}\n    - {code: invalid_request, meaning: 'Missing/invalid/duplicated parameter, or malformed request.'}\n  docs: https://developers.citrusad.com/integration/reference/oauth-20-authentication\n  sources:\n    - https://developers.citrusad.com/integration/reference/oauth-20-authentication\n\n- name: TokenSecurity\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer xxx.yyy.zzz (JWT)'\n  description: >-\n    Declared in the published OpenAPI for the Filter Mapping and Cross-Sell\n    Category APIs: \"For accessing the API a valid JWT must be passed in all\n    queries in the 'Authorization' header.\"\
  \n  applies_to:\n    - Epsilon Retail Media Filter Mapping API\n    - Epsilon Retail Media Cross-Sell Category API\n  sources:\n    - openapi/epsilon-retail-media-filter-mapping-openapi.json\n    - openapi/epsilon-retail-media-cross-sell-category-openapi.json\n\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  x_bearer_format: basic\n  description: >-\n    The security scheme as declared in the published Integration API OpenAPI.\n    It is modelled as apiKey-in-header with x-bearer-format basic, which is the\n    spec-level expression of the HTTP Basic API key above.\n  sources:\n    - openapi/epsilon-retail-media-integration-openapi.json\n\nobserved:\n  - url: https://eu-ads.rmn.dotomi.com/ads/v3/brand-pages\n    method: POST\n    sent: no credentials\n    status: 401\n    content_type: application/problem+json\n    body: '{\"title\":\"Unauthorized.\",\"status\":401,\"detail\":\"Missing or invalid API credentials.\",\"instance\":\"/ads/v3/brand-pages\"}'\n   \
  \ checked: '2026-08-12'\n  - url: https://eu-ads.rmn.dotomi.com/v1/ads/generate\n    method: POST\n    sent: no credentials, empty JSON body\n    status: 400\n    content_type: text/plain\n    body: '\"catalogId must be set\"'\n    note: >-\n      The v1 ad-generation surface validates the body before authentication and\n      answers in text/plain, unlike the v3 brand-pages surface which answers with\n      RFC 9457 problem+json. The two generations of this API do not share an error\n      or auth-failure contract.\n    checked: '2026-08-12'\n\ngaps:\n  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server is served on any Epsilon host, so the OAuth 2.0 authorization server is not machine-discoverable.\n  - The OAuth 2.0 flow is documented in prose only; it is not declared as an oauth2 securityScheme in any published OpenAPI.\n  - Token endpoint is documented as a template (https://$BASE_URL/v1/oauth2/token); the concrete host is tenant-assigned.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epsilon/refs/heads/main/authentication/epsilon-authentication.yml
summary_line: apiKey/http-basic/oauth2/jwt-bearer · 4 schemes
tags:
- Company
- Marketing
- Advertising
- Retail Media
- Advertising Technology
- Identity Resolution
- Customer Data
- Loyalty
- Retail
- Publicis Groupe
---
