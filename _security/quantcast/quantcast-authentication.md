---
api_key_in:
- query
api_specs:
- filename: QuantcastDeveloperAPI.postman_collection.json
  format: json
  label: Quantcast Platform GraphQL API
  slug: quantcast-platform-graphql-api
  spec_type: Postman
  url: https://developers.quantcast.com/docs/QuantcastDeveloperAPI.postman_collection.json
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Quantcast Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Quantcast secures its APIs with oauth2, http, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Quantcast
provider_slug: quantcast
scheme_count: 3
schemes:
- api: Quantcast Platform GraphQL API
  client_authentication: client_secret_basic
  credential_issuance: API Key and Secret are self-issued from the Quantcast Platform UI (Profile icon -> My Profile -> API Key -> Create API Key). Credentials cannot be recovered; a lost key requires creating a new pair.
  expired_token_status: 403
  flow: clientCredentials
  identity_provider: Okta
  name: QuantcastPlatformOAuth2
  presentation:
    format: Bearer <access_token>
    header: Authorization
  request_content_type: application/x-www-form-urlencoded
  scopes:
  - api_access
  - read_reports
  source: https://developers.quantcast.com/docs/get-started/authentication/
  token_lifetime_note: The documentation states each token is valid for one hour, while the sample token response it prints shows expires_in 86400. The prose is the normative statement; both values are recorded because the docs disagree with their own example.
  token_lifetime_seconds: 3600
  token_type: Bearer
  token_url: https://auth.quantcast.com/oauth2/default/v1/token
  type: oauth2
- api: Quantcast Platform GraphQL API
  description: The GraphQL endpoint itself accepts only the bearer token minted by the client-credentials flow above. An unauthenticated POST to https://developers.quantcast.com/api/v2/graphql returns HTTP 401 with {"error":"No authentication token in request"} — probed 2026-08-13.
  name: QuantcastPlatformBearer
  scheme: bearer
  source: https://developers.quantcast.com/docs/graphql-api/usage/requests-to-graphql/
  type: http
- api: Quantcast Conversion API
  description: The Conversion API and the browser token endpoint on pixel.quantserve.com are keyed by the Quantcast account id (pCode) passed as the `a` query parameter. This is an account identifier, not a secret credential; the documented trust model relies on the browser token (issued by the /token endpoint) or on client_user_agent + client_ip to identify the user. Quantcast documents no bearer token or signed request for this surface.
  in: query
  name: QuantcastConversionAccountId
  parameter: a
  source: https://help.quantcast.com/docs/tagging-with-the-quantcast-live-tag-using-the-conversion-api
  type: apiKey
slug: quantcast-authentication
source_filename: quantcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.quantcast.com/docs/get-started/authentication/\ndocs: https://developers.quantcast.com/docs/get-started/authentication/\nnote: >-\n  Derived by hand from the published developer documentation rather than from\n  an OpenAPI securityScheme block — Quantcast publishes no OpenAPI. The\n  OAuth 2.0 endpoints below were additionally confirmed against the live\n  discovery documents saved in well-known/.\nsummary:\n  types: [oauth2, http, apiKey]\n  api_key_in: [query]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: QuantcastPlatformOAuth2\n  type: oauth2\n  api: Quantcast Platform GraphQL API\n  flow: clientCredentials\n  token_url: https://auth.quantcast.com/oauth2/default/v1/token\n  client_authentication: client_secret_basic\n  request_content_type: application/x-www-form-urlencoded\n  scopes: [api_access, read_reports]\n  token_type: Bearer\n  token_lifetime_seconds: 3600\n  token_lifetime_note: >-\n\
  \    The documentation states each token is valid for one hour, while the\n    sample token response it prints shows expires_in 86400. The prose is the\n    normative statement; both values are recorded because the docs disagree\n    with their own example.\n  expired_token_status: 403\n  presentation:\n    header: Authorization\n    format: 'Bearer <access_token>'\n  identity_provider: Okta\n  credential_issuance: >-\n    API Key and Secret are self-issued from the Quantcast Platform UI\n    (Profile icon -> My Profile -> API Key -> Create API Key). Credentials\n    cannot be recovered; a lost key requires creating a new pair.\n  source: https://developers.quantcast.com/docs/get-started/authentication/\n- name: QuantcastPlatformBearer\n  type: http\n  scheme: bearer\n  api: Quantcast Platform GraphQL API\n  description: >-\n    The GraphQL endpoint itself accepts only the bearer token minted by the\n    client-credentials flow above. An unauthenticated POST to\n    https://developers.quantcast.com/api/v2/graphql\
  \ returns HTTP 401 with\n    {\"error\":\"No authentication token in request\"} — probed 2026-08-13.\n  source: https://developers.quantcast.com/docs/graphql-api/usage/requests-to-graphql/\n- name: QuantcastConversionAccountId\n  type: apiKey\n  in: query\n  parameter: a\n  api: Quantcast Conversion API\n  description: >-\n    The Conversion API and the browser token endpoint on\n    pixel.quantserve.com are keyed by the Quantcast account id (pCode) passed\n    as the `a` query parameter. This is an account identifier, not a secret\n    credential; the documented trust model relies on the browser token\n    (issued by the /token endpoint) or on client_user_agent + client_ip to\n    identify the user. Quantcast documents no bearer token or signed request\n    for this surface.\n  source: https://help.quantcast.com/docs/tagging-with-the-quantcast-live-tag-using-the-conversion-api\nauthorization_server:\n  issuer: https://auth.quantcast.com\n  discovery:\n  - well-known/quantcast-openid-configuration.json\n\
  \  - well-known/quantcast-oauth-authorization-server.json\n  documented_token_endpoint: https://auth.quantcast.com/oauth2/default/v1/token\n  discovery_token_endpoint: https://auth.quantcast.com/oauth2/v1/token\n  discovery_note: >-\n    The developer docs call the `default` custom authorization server\n    (/oauth2/default/v1/token); the org-level discovery document advertises\n    the org authorization server (/oauth2/v1/token). Use the documented\n    `default` endpoint — the api_access and read_reports scopes are defined\n    on it, not on the org server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantcast/refs/heads/main/authentication/quantcast-authentication.yml
summary_line: oauth2/http/apiKey · 3 schemes
tags:
- Advertising
- AdTech
- Programmatic Advertising
- Demand-Side Platform
- DSP
- Audience Measurement
- Audience Intelligence
- Consent Management
- CMP
- Privacy
- GraphQL
- Conversion Tracking
- CTV
- Video Advertising
- Display Advertising
- Artificial Intelligence
- Audience Graph
---
