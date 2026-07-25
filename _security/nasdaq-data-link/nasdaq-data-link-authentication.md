---
api_key_in:
- query
api_specs:
- filename: postman
  format: yaml
  label: Nasdaq Data Link REST API for Real-Time or Delayed Data
  slug: nasdaq-data-link-rest-api-for-real-time-or-delayed-data
  spec_type: Postman
  url: https://github.com/Nasdaq/NasdaqCloudDataService-REST-API/tree/main/restapi/postman
auth_types:
- apiKey
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Nasdaq Data Link Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nasdaq Data Link secures its APIs with apiKey, oauth2, and http-bearer across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nasdaq Data Link
provider_slug: nasdaq-data-link
scheme_count: 3
schemes:
- description: 'Tables / core REST API (data.nasdaq.com/api/v3): append your API key as the api_key query parameter (e.g. ?api_key=YOURAPIKEY). Keys are issued free on registration and found under account settings (https://data.nasdaq.com/account/api). Anonymous (keyless) access is allowed at heavily reduced rate limits. The Python CLI reads the key from the NDL_APIKEY environment variable.'
  in: query
  name: api_key
  parameter: api_key
  type: apiKey
- description: 'REST API for real-time or delayed data (Nasdaq Cloud Data Service): POST client_id + client_secret to https://<base_url>/v1/auth/token to obtain an access_token bearer token (with expires_in). Credentials and the customer-specific base URL are provisioned by Nasdaq sales.'
  name: ncds_rest_bearer
  scheme: bearer
  type: http
- description: 'Streaming API (NCDS Java/Python SDKs): OAuth 2.0 client credentials — Nasdaq sales provisions client ID, client secret, token endpoint, and Kafka bootstrap servers. The live authorization server metadata (RFC 8414, Okta) is captured in well-known/nasdaq-data-link-oauth-authorization-server.json and advertises the datalink scope. data.nasdaq.com also publishes RFC 9728 protected-resource metadata pointing at this authorization server.'
  flows:
  - authorizationUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/authorize
    flow: clientCredentials
    tokenUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/token
  name: ncds_streaming_oauth2
  type: oauth2
slug: nasdaq-data-link-authentication
source_filename: nasdaq-data-link-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://docs.data.nasdaq.com/docs/data-organization\ndocs:\n  - https://docs.data.nasdaq.com/docs/data-organization\n  - https://docs.data.nasdaq.com/docs/streaming-api\n  - https://github.com/Nasdaq/NasdaqCloudDataService-REST-API/blob/main/restapi/authenticate.md\nsummary:\n  types: [apiKey, oauth2, http-bearer]\n  api_key_in: [query]\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: api_key\n    type: apiKey\n    in: query\n    parameter: api_key\n    description: >-\n      Tables / core REST API (data.nasdaq.com/api/v3): append your API key as\n      the api_key query parameter (e.g. ?api_key=YOURAPIKEY). Keys are issued\n      free on registration and found under account settings\n      (https://data.nasdaq.com/account/api). Anonymous (keyless) access is\n      allowed at heavily reduced rate limits. The Python CLI reads the key\n      from the NDL_APIKEY environment variable.\n  - name: ncds_rest_bearer\n    type:\
  \ http\n    scheme: bearer\n    description: >-\n      REST API for real-time or delayed data (Nasdaq Cloud Data Service):\n      POST client_id + client_secret to https://<base_url>/v1/auth/token to\n      obtain an access_token bearer token (with expires_in). Credentials and\n      the customer-specific base URL are provisioned by Nasdaq sales.\n  - name: ncds_streaming_oauth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        authorizationUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/authorize\n        tokenUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/token\n    description: >-\n      Streaming API (NCDS Java/Python SDKs): OAuth 2.0 client credentials —\n      Nasdaq sales provisions client ID, client secret, token endpoint, and\n      Kafka bootstrap servers. The live authorization server metadata\n      (RFC 8414, Okta) is captured in\n      well-known/nasdaq-data-link-oauth-authorization-server.json and\n      advertises the datalink\
  \ scope. data.nasdaq.com also publishes RFC 9728\n      protected-resource metadata pointing at this authorization server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-data-link/refs/heads/main/authentication/nasdaq-data-link-authentication.yml
summary_line: apiKey/oauth2/http-bearer · 3 schemes
tags:
- Financial Data
- Stock Market
- Market Data
- Economic Data
- Alternative Data
- Time Series
- Open Data
- Public APIs
---
