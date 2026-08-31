---
api_key_in:
- header
api_specs:
- filename: factiva-apis
  format: yaml
  label: Factiva Snapshots API
  slug: factiva-snapshots-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Streams API
  slug: factiva-streams-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Extractions API
  slug: factiva-extractions-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Analytics API
  slug: factiva-analytics-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva DJID Taxonomy API
  slug: factiva-djid-taxonomy-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-apis
  format: yaml
  label: Factiva Code API
  slug: factiva-code-api
  spec_type: Postman
  url: https://www.postman.com/dj-cse/dow-jones-apis/documentation/l9tpql6/factiva-apis
- filename: factiva-content-api-openapi.yml
  format: yaml
  label: Factiva Content API
  slug: factiva-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-content-api-openapi.yml
- filename: factiva-content-search-api-openapi.yml
  format: yaml
  label: Factiva Content Search API
  slug: factiva-content-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-content-search-api-openapi.yml
- filename: factiva-default-api-openapi.yml
  format: yaml
  label: Factiva Default API
  slug: factiva-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-default-api-openapi.yml
- filename: factiva-editions-api-openapi.yml
  format: yaml
  label: Factiva Editions API
  slug: factiva-editions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-editions-api-openapi.yml
- filename: factiva-newsletters-api-openapi.yml
  format: yaml
  label: Factiva Newsletters API
  slug: factiva-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/openapi/factiva-newsletters-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: 'Factiva Integration implements two authentication methods side by side: a user key (API key) sent in a `user-key` header, and a bearer authorization token obtained through a two-step exchange against the Dow Jones identity service. The harvested OpenAPI/Swagger documents declare only the bearer half; the user-key half is documented but not modelled in any published spec, which is why this file is `searched` rather than `derived`.'
kind: authentication
layout: security
method: searched
name: Factiva Authentication
name_suffix: Authentication
oauth_flows:
- password
- refresh_token
overview: Factiva secures its APIs with apiKey, http, and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and refresh_token flow(s).
provider_name: Factiva
provider_slug: factiva
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/factiva-company-news-radar-api-openapi.json
  - openapi/factiva-newsletters-api-openapi.json
  type: http
- in: header
  name: Bearer
  note: Modelled as an apiKey header in the Swagger 2.0 Content API document; semantically the same bearer token as `bearerAuth` in the OpenAPI 3 documents.
  parameter: Authorization
  sources:
  - openapi/factiva-content-api-swagger.json
  type: apiKey
slug: factiva-authentication
source_filename: factiva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/factiva-company-news-radar-api-openapi.json, openapi/factiva-content-api-swagger.json,\n  openapi/factiva-newsletters-api-openapi.json\ndocs: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication\ndescription: >-\n  Factiva Integration implements two authentication methods side by side: a user key (API key)\n  sent in a `user-key` header, and a bearer authorization token obtained through a two-step\n  exchange against the Dow Jones identity service. The harvested OpenAPI/Swagger documents\n  declare only the bearer half; the user-key half is documented but not modelled in any\n  published spec, which is why this file is `searched` rather than `derived`.\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  api_key_names:\n    - user-key\n    - Authorization\n  oauth2_flows:\n    - password\n    - refresh_token\n  credential_issuance: sales-issued\n\
  \  self_service_signup: false\nmethods:\n  - id: user-key\n    name: User Key-Based Authentication\n    type: apiKey\n    in: header\n    parameter: user-key\n    description: >-\n      The most widely used method within Factiva. Dow Jones issues the user key to the customer;\n      it is sent on every request in the `user-key` header, typically alongside an\n      `X-API-VERSION` header naming the endpoint version.\n    example: >-\n      curl --location --request GET 'https://api.dowjones.com/taxonomies'\n      --header 'user-key: {your-user-key-here}' --header 'X-API-VERSION: 3.0'\n    applies_to:\n      - Factiva Snapshots\n      - Factiva Streams\n      - Factiva Extractions\n      - Factiva Analytics\n      - Factiva Taxonomy\n    source: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication\n  - id: bearer-token\n    name: Token-Based Authentication\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    parameter: Authorization\n\
  \    description: >-\n      An authorization (AuthZ) token sent in the `Authorization: Bearer` header. Obtained in a\n      two-step exchange: first POST service-account credentials to the identity service to get\n      the AuthN tokens (id_token + access_token, plus a refresh token when offline_access is\n      requested), then exchange those for the AuthZ token used against the Factiva endpoints.\n    applies_to:\n      - Factiva Content / Article Fetch\n      - Factiva Newsletters\n      - Factiva Retrieval (GenAI)\n      - Company News Radar\n    source: https://developer.dowjones.com/documents/factiva_integration-essentials-authentication\noauth2:\n  issuer: https://sso.accounts.dowjones.com/\n  discovery: https://accounts.dowjones.com/.well-known/openid-configuration\n  discovery_file: well-known/factiva-openid-configuration.json\n  token_endpoint: https://accounts.dowjones.com/oauth2/v1/token\n  issuer_token_endpoint: https://sso.accounts.dowjones.com/oauth/token\n  authorization_endpoint:\
  \ https://sso.accounts.dowjones.com/authorize\n  jwks_uri: https://sso.accounts.dowjones.com/.well-known/jwks.json\n  grant_types_supported:\n    - authorization_code\n    - implicit\n    - refresh_token\n    - password\n    - client_credentials\n    - urn:ietf:params:oauth:grant-type:jwt-bearer\n  grant_type_used_by_factiva: password\n  connection: service-account\n  pkce: [S256, plain]\n  id_token_signing_alg: [RS256, HS256]\n  documented_flows:\n    - name: Service Account Integration\n      grant: password\n      note: >-\n        The flow the Factiva Integration docs prescribe for server-to-server use; parameters are\n        username, client_id, password, connection=service-account, grant_type=password, scope.\n    - name: Authorization Code Grant Flow\n      grant: authorization_code\n      source: https://developer.dowjones.com/documents/site-docs-factiva_apis-factiva_analytics_apis-factiva_article_retrieval-authentication-authorization_code_grant_flow\n    - name: Implicit Grant\
  \ Flow\n      grant: implicit\n      source: https://developer.dowjones.com/documents/site-docs-factiva_apis-factiva_analytics_apis-factiva_article_retrieval-authentication-implicit_grant_flow\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    sources:\n      - openapi/factiva-company-news-radar-api-openapi.json\n      - openapi/factiva-newsletters-api-openapi.json\n  - name: Bearer\n    type: apiKey\n    in: header\n    parameter: Authorization\n    sources:\n      - openapi/factiva-content-api-swagger.json\n    note: >-\n      Modelled as an apiKey header in the Swagger 2.0 Content API document; semantically the same\n      bearer token as `bearerAuth` in the OpenAPI 3 documents.\ncredentials:\n  issuance: >-\n    Credentials are not self-service. A customer submits the Request Trial form, a Dow Jones\n    representative matches the use case to a product, and credentials arrive by email.\n  request_url: https://developer.dowjones.com/request-trial\n\
  \  docs: https://developer.dowjones.com/documents/site-docs-getting_started-quick_start-getting_credentials\nobserved:\n  - request: GET https://api.dowjones.com/content/swagger (unauthenticated)\n    http_status: 403\n    body: '{\"errors\":[{\"title\":\"Authentication parameters missing\",\"status\":403,\"code\":1011001}]}'\n    fetched: '2026-08-13'\n    note: >-\n      Live unauthenticated probe. Confirms the gateway rejects with 403 (not 401) and returns a\n      JSON:API-shaped `errors[]` envelope carrying a numeric Dow Jones error code.\nrelated:\n  - scopes/factiva-scopes.yml\n  - conventions/factiva-conventions.yml\n  - well-known/factiva-well-known.yml\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factiva/refs/heads/main/authentication/factiva-authentication.yml
summary_line: apiKey/http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Business Intelligence
- Content Aggregation
- Enterprise Data
- GenAI
- Market Data
- Media Monitoring
- News
- News API
- Research
- Taxonomy
---
