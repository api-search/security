---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apilayer-endpoints-api-openapi.yml
  format: yaml
  label: APILayer Endpoints API
  slug: apilayer-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apilayer/refs/heads/main/openapi/apilayer-endpoints-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Apilayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: APILayer declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: APILayer
provider_slug: apilayer
scheme_count: 3
schemes:
- applies_to: every REST product endpoint (exchangerate.host, exchangeratesapi.io, ipapi.com and every other APILayer product host)
  caveats:
  - The key travels in the URL, so it is written to proxy logs, browser history and Referer headers. APILayer documents no header alternative.
  - 'A missing or invalid key does NOT return 401 over the wire. The live surface answers HTTP 200 with a body of {"success": false, "error": {"code": 101, "type": "invalid_access_key"}}. Observed 2026-09-12 on https://api.ipapi.com/api/check?access_key=x and https://api.exchangerate.host/live. The OpenAPI documents 401 for this case; the deployed API does not send it.'
  - Only 9 of the 22 OpenAPI documents APILayer publishes declare a securityScheme at all. The three specs captured in this repo declare `access_key` as a required query parameter on every operation but carry no components.securitySchemes block and no top-level security requirement.
  description: Your API Access Key, issued per product subscription in the APILayer dashboard.
  evidence: openapi/_original/apilayer-ipapi-openapi-original.json parameters[access_key]
  id: access_key
  in: query
  name: access_key
  required: true
  type: apiKey
- applies_to: https://api.apilayer.com - the marketplace gateway behind marketplace.apilayer.com
  caveats:
  - 'This gateway DOES honour HTTP status: an invalid key returned a real 401 with {"message":"Invalid authentication credentials"} when probed 2026-09-12, unlike the product hosts, which answer 200 on an auth failure. The two halves of APILayer behave differently on the same failure and an agent must know which host it is talking to.'
  - The header form is the more defensible design of the two - the credential stays out of the URL - but it is used only on the legacy marketplace, not on the flagship products.
  description: Marketplace API key, sent as an `apikey` request header.
  evidence: 'https://marketplace.apilayer.com/bank_data-api publishes the call verbatim: curl --request GET ''https://api.apilayer.com/bank_data/iban_validate?iban_number=...'' --header ''apikey: YOUR API KEY'''
  id: apikey-header
  in: header
  name: apikey
  required: true
  type: apiKey
- applies_to: https://mcp.apilayer.com/mcp
  authorization_endpoint: https://auth.apilayer.com/oauth2/auth
  bearer_methods:
  - header
  device_authorization_endpoint: https://auth.apilayer.com/oauth2/device/auth
  dynamic_client_registration: true
  evidence: well-known/apilayer-openid-configuration.json, well-known/apilayer-oauth-protected-resource.json
  grant_types:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id: apilayer-oauth
  issuer: https://auth.apilayer.com
  jwks_uri: https://auth.apilayer.com/.well-known/jwks.json
  pkce: true
  registration_endpoint: https://auth.apilayer.com/oauth2/register
  token_endpoint: https://auth.apilayer.com/oauth2/token
  type: oauth2
  userinfo_endpoint: https://auth.apilayer.com/userinfo
slug: apilayer-authentication
source_filename: apilayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://docs.apilayer.com/exchangerate/docs/api-documentation (docs), plus openapi/_original/*.json\n  and the probed discovery documents in well-known/\nprovider: APILayer\nproviderId: apilayer\nsummary: APILayer runs THREE independent authentication systems. (1) Every REST product API (ipapi.com,\n  exchangerate.host, exchangeratesapi.io and the rest of the *stack/*layer family) is authenticated with\n  a per-product API access key passed as the `access_key` QUERY STRING parameter - no header form, no\n  bearer token, no scope. (2) The legacy marketplace gateway at api.apilayer.com uses an `apikey` REQUEST\n  HEADER instead. (3) The hosted MCP server at mcp.apilayer.com uses OAuth 2.1 bearer tokens from auth.apilayer.com,\n  advertised through RFC 9728 protected-resource metadata and RFC 8414 / OpenID Connect discovery. A developer\n  holding an APILayer account can meet all three.\nschemes:\n- id: access_key\n  type: apiKey\n\
  \  in: query\n  name: access_key\n  required: true\n  applies_to: every REST product endpoint (exchangerate.host, exchangeratesapi.io, ipapi.com and every\n    other APILayer product host)\n  description: Your API Access Key, issued per product subscription in the APILayer dashboard.\n  evidence: openapi/_original/apilayer-ipapi-openapi-original.json parameters[access_key]\n  caveats:\n  - The key travels in the URL, so it is written to proxy logs, browser history and Referer headers. APILayer\n    documents no header alternative.\n  - 'A missing or invalid key does NOT return 401 over the wire. The live surface answers HTTP 200 with\n    a body of {\"success\": false, \"error\": {\"code\": 101, \"type\": \"invalid_access_key\"}}. Observed 2026-09-12\n    on https://api.ipapi.com/api/check?access_key=x and https://api.exchangerate.host/live. The OpenAPI\n    documents 401 for this case; the deployed API does not send it.'\n  - Only 9 of the 22 OpenAPI documents APILayer publishes declare\
  \ a securityScheme at all. The three specs\n    captured in this repo declare `access_key` as a required query parameter on every operation but carry\n    no components.securitySchemes block and no top-level security requirement.\n- id: apikey-header\n  type: apiKey\n  in: header\n  name: apikey\n  required: true\n  applies_to: https://api.apilayer.com - the marketplace gateway behind marketplace.apilayer.com\n  description: Marketplace API key, sent as an `apikey` request header.\n  evidence: 'https://marketplace.apilayer.com/bank_data-api publishes the call verbatim: curl --request\n    GET ''https://api.apilayer.com/bank_data/iban_validate?iban_number=...'' --header ''apikey: YOUR API\n    KEY'''\n  caveats:\n  - 'This gateway DOES honour HTTP status: an invalid key returned a real 401 with {\"message\":\"Invalid\n    authentication credentials\"} when probed 2026-09-12, unlike the product hosts, which answer 200 on\n    an auth failure. The two halves of APILayer behave differently\
  \ on the same failure and an agent must\n    know which host it is talking to.'\n  - The header form is the more defensible design of the two - the credential stays out of the URL - but\n    it is used only on the legacy marketplace, not on the flagship products.\n- id: apilayer-oauth\n  type: oauth2\n  applies_to: https://mcp.apilayer.com/mcp\n  issuer: https://auth.apilayer.com\n  authorization_endpoint: https://auth.apilayer.com/oauth2/auth\n  token_endpoint: https://auth.apilayer.com/oauth2/token\n  device_authorization_endpoint: https://auth.apilayer.com/oauth2/device/auth\n  registration_endpoint: https://auth.apilayer.com/oauth2/register\n  userinfo_endpoint: https://auth.apilayer.com/userinfo\n  jwks_uri: https://auth.apilayer.com/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - implicit\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  pkce: true\n  dynamic_client_registration: true\n  bearer_methods:\n  - header\n\
  \  evidence: well-known/apilayer-openid-configuration.json, well-known/apilayer-oauth-protected-resource.json\ntransport:\n  https_required: true\n  note: HTTPS on the REST products is a PAID feature. The published error catalog carries code 105 https_access_restricted\n    - \"Access Restricted - Your current Subscription Plan does not support HTTPS Encryption\" - so free-tier\n    keys are expected to be sent over plaintext HTTP.\nmfa_or_mtls: none published\nkey_rotation: not documented\nchecked: '2026-09-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apilayer/refs/heads/main/authentication/apilayer-authentication.yml
summary_line: 3 schemes
tags:
- API Marketplace
- API Catalog
- API Discovery
- Developer Tools
- SaaS APIs
- Geolocation
- Currency
- Data API
---
