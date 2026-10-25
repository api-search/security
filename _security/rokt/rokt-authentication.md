---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: rokt-query-api-openapi.yml
  format: yaml
  label: Rokt Query API
  slug: rokt-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rokt/refs/heads/main/openapi/rokt-query-api-openapi.yml
- filename: rokt-partnerships-api-openapi.yml
  format: yaml
  label: Rokt Partnerships API
  slug: rokt-partnerships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rokt/refs/heads/main/openapi/rokt-partnerships-api-openapi.yml
- filename: rokt-catalog-api-openapi.yml
  format: yaml
  label: Rokt Catalog API
  slug: rokt-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rokt/refs/heads/main/openapi/rokt-catalog-api-openapi.yml
- filename: rokt-session-api-openapi.yml
  format: yaml
  label: Rokt Session API
  slug: rokt-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rokt/refs/heads/main/openapi/rokt-session-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Rokt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rokt secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rokt
provider_slug: rokt
scheme_count: 4
schemes:
- description: Your Application ID, from Settings > API Credentials in the Rokt Catalog app.
  in: header
  name: platformAppId
  parameter: X-CANAL-APP-ID
  sources:
  - openapi/rokt-catalog-api-openapi.yml
  type: apiKey
- description: Your API Access Token, from Settings > API Credentials in the Rokt Catalog app. Keep it server-side.
  in: header
  name: platformAppToken
  parameter: X-CANAL-APP-TOKEN
  sources:
  - openapi/rokt-catalog-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Short-lived access token (JWT), exchanged from your platform''s API

    credentials (`client_id` + `client_secret`). Rokt issues the API

    credentials once, during onboarding. They are not self-serve;

    request them from **smb-partnerships@rokt.com**. The same long-lived

    credentials are reused for every token exchange. Pass the access

    token as `Authorization: Bearer <token>`. See

    [Authentication](/develope'
  name: ApiToken
  scheme: bearer
  sources:
  - openapi/rokt-partnerships-api-openapi.yml
  - openapi/rokt-query-api-openapi.yml
  type: http
- description: '`Basic base64(rpub:rsec)` — your Rokt public and secret API keys, joined

    with a colon and base64-encoded. Provided by your Rokt account team.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/rokt-session-api-openapi.yml
  type: http
slug: rokt-authentication
source_filename: rokt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource:\n- https://docs.rokt.com/developer-reference/apis/partnerships-api/authentication/\n- https://docs.rokt.com/developer-reference/apis/reporting-apis/query-api/\n- https://docs.rokt.com/integration-guides/ecommerce/catalog/authentication/\n- openapi/rokt-catalog-api-openapi.yml\n- openapi/rokt-partnerships-api-openapi.yml\n- openapi/rokt-query-api-openapi.yml\n- openapi/rokt-session-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: platformAppId\n  type: apiKey\n  in: header\n  parameter: X-CANAL-APP-ID\n  description: Your Application ID, from Settings > API Credentials in the Rokt Catalog app.\n  sources:\n  - openapi/rokt-catalog-api-openapi.yml\n- name: platformAppToken\n  type: apiKey\n  in: header\n  parameter: X-CANAL-APP-TOKEN\n  description: Your API Access Token, from Settings > API Credentials in the Rokt Catalog app. Keep it server-side.\n  sources:\n  - openapi/rokt-catalog-api-openapi.yml\n\
  - name: ApiToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Short-lived access token (JWT), exchanged from your platform''s API\n\n    credentials (`client_id` + `client_secret`). Rokt issues the API\n\n    credentials once, during onboarding. They are not self-serve;\n\n    request them from **smb-partnerships@rokt.com**. The same long-lived\n\n    credentials are reused for every token exchange. Pass the access\n\n    token as `Authorization: Bearer <token>`. See\n\n    [Authentication](/develope'\n  sources:\n  - openapi/rokt-partnerships-api-openapi.yml\n  - openapi/rokt-query-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: '`Basic base64(rpub:rsec)` — your Rokt public and secret API keys, joined\n\n    with a colon and base64-encoded. Provided by your Rokt account team.'\n  sources:\n  - openapi/rokt-session-api-openapi.yml\ndocs: https://docs.rokt.com/developer-reference/apis/partnerships-api/authentication/\ntoken_flows:\n\
  - api: Partnerships API\n  grant_type: client_credentials\n  token_url: https://auth.rokt.com/api/v1/oauth/token\n  client_auth: client_id + client_secret form fields\n  expires_in: 300\n  credential_issuance: Issued by Rokt during onboarding via smb-partnerships@rokt.com; not self-serve.\n  extra_headers:\n  - X-Platform-Parent-Account-Id (required on writes; missing 422, mismatched 403)\n  - Idempotency-Key (required on writes)\n  source: https://docs.rokt.com/developer-reference/apis/partnerships-api/authentication/\n- api: Query API\n  grant_type: client_credentials\n  token_url: https://api.rokt.com/auth/oauth2/token\n  client_auth: HTTP Basic base64(App ID:App Secret)\n  expires_in_text: The access token expires after one hour\n  source: https://docs.rokt.com/developer-reference/apis/reporting-apis/query-api/\n- api: Catalog API\n  note: x-canal-app-id and x-canal-app-token headers; \"automatically generated for you when your account is created\",\n    found under Settings > API\
  \ Credentials in the Rokt Catalog App.\n  source: https://docs.rokt.com/integration-guides/ecommerce/catalog/authentication/\nscopes_documented: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rokt/refs/heads/main/authentication/rokt-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- E-Commerce
- Advertising
- Transaction Moment
- Personalization
- Offers
- Analytics
- Reporting
---
