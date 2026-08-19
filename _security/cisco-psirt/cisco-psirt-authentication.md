---
api_key_in: []
api_specs:
- filename: cisco-psirt-current-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Current Endpoints API
  slug: cisco-psirt-current-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-current-endpoints-api-openapi.yml
- filename: cisco-psirt-obsolete-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Obsolete Endpoints API
  slug: cisco-psirt-obsolete-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml
- filename: cisco-psirt-sunset-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Sunset Endpoints API
  slug: cisco-psirt-sunset-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-sunset-endpoints-api-openapi.yml
auth_types:
- http
- oauth2
description: 'The OpenAPI declares only the WIRE format — HTTP bearer with a JWT. That is half the contract. Cisco''s authentication docs supply the other half: the token is an OAuth 2.0 client-credentials access token minted by Cisco''s Okta-backed identity service at id.cisco.com, from a client_id/client_secret pair issued when you register an application against this specific API in the Cisco API Console. The spec cannot express that, so an integrator reading the spec alone would not know where a token comes from.'
kind: authentication
layout: security
method: searched
name: Cisco Psirt Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cisco PSIRT openVuln API secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cisco PSIRT openVuln API
provider_slug: cisco-psirt
scheme_count: 2
schemes:
- applied: global
  bearerFormat: JWT
  name: psirt_openvuln_api_auth
  note: Declared in the spec and applied at the document level, so every one of the 30 operations requires it. The spec does not say the bearer is an OAuth2 access token; the docs do.
  scheme: bearer
  sources:
  - openapi/cisco-psirt-current-endpoints-api-openapi.yml
  - openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml
  - openapi/cisco-psirt-sunset-endpoints-api-openapi.yml
  type: http
- audience: api://default
  expires_in: 3600
  flow: clientCredentials
  issuer: https://id.cisco.com/oauth2/default
  name: cisco-oauth2-client-credentials
  note: Not in the OpenAPI. Captured from the docs, which publish the exact client-credentials exchange. SEARCHED, not derived.
  scopes:
    customscope: The only scope observed in Cisco's own published token response. Cisco does not document a scope reference or per-endpoint scopes for this API.
  source: https://developer.cisco.com/docs/psirt/authentication/
  tokenUrl: https://id.cisco.com/oauth2/default/v1/token
  token_type: Bearer
  type: oauth2
slug: cisco-psirt-authentication
source_filename: cisco-psirt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://developer.cisco.com/docs/psirt/authentication/\nderived_from: >-\n  openapi/cisco-psirt-current-endpoints-api-openapi.yml,\n  openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml,\n  openapi/cisco-psirt-sunset-endpoints-api-openapi.yml\ndocs: https://developer.cisco.com/docs/psirt/authentication/\ndescription: >-\n  The OpenAPI declares only the WIRE format — HTTP bearer with a JWT. That is half\n  the contract. Cisco's authentication docs supply the other half: the token is an\n  OAuth 2.0 client-credentials access token minted by Cisco's Okta-backed identity\n  service at id.cisco.com, from a client_id/client_secret pair issued when you\n  register an application against this specific API in the Cisco API Console. The\n  spec cannot express that, so an integrator reading the spec alone would not know\n  where a token comes from.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  bearer_format: JWT\n\
  \  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  transport: HTTPS only — \"All operations must communicate over a secure HTTPS connection.\"\nschemes:\n  - name: psirt_openvuln_api_auth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applied: global\n    sources:\n      - openapi/cisco-psirt-current-endpoints-api-openapi.yml\n      - openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml\n      - openapi/cisco-psirt-sunset-endpoints-api-openapi.yml\n    note: >-\n      Declared in the spec and applied at the document level, so every one of the\n      30 operations requires it. The spec does not say the bearer is an OAuth2\n      access token; the docs do.\n  - name: cisco-oauth2-client-credentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://id.cisco.com/oauth2/default/v1/token\n    issuer: https://id.cisco.com/oauth2/default\n    audience: api://default\n    token_type: Bearer\n    expires_in: 3600\n    scopes:\n      customscope: >-\n\
  \        The only scope observed in Cisco's own published token response. Cisco does\n        not document a scope reference or per-endpoint scopes for this API.\n    source: https://developer.cisco.com/docs/psirt/authentication/\n    note: >-\n      Not in the OpenAPI. Captured from the docs, which publish the exact\n      client-credentials exchange. SEARCHED, not derived.\nregistration:\n  console: https://apiconsole.cisco.com/\n  keys_page: https://apiconsole.cisco.com/apps/mykeys\n  identity: A Cisco.com ID is required; register one from the console if you have none.\n  steps:\n    - Log in to the Cisco API Console with a Cisco.com ID.\n    - Open \"My Apps & Keys\" and choose \"Register a New App\".\n    - Set Application Type to \"Service\".\n    - Set Grant Type to \"Client Credentials\".\n    - Select the \"Cisco PSIRT openVuln API\".\n    - Agree to the terms of service and register.\n    - Collect the resulting \"Key\" (client_id) and \"Client Secret\".\n  eligibility: >-\n\
  \    \"The openVuln API is open to registered Cisco customers and partners.\"\n    (https://github.com/CiscoPSIRT/openVulnAPI/blob/master/README.md)\n  migration_notice: >-\n    \"IMPORTANT: Current registered applications will be deprecated in coming\n    months. Please migrate your applications to continue using API's.\"\ntoken_exchange:\n  method: POST\n  url: https://id.cisco.com/oauth2/default/v1/token\n  content_type: application/x-www-form-urlencoded\n  parameters: [client_id, client_secret, grant_type=client_credentials]\n  client_authentication: >-\n    Credentials in the form body, or as an HTTP Basic header (Cisco's Postman\n    walkthrough sets \"Client Authentication: Send as Basic Auth Header\").\n  response_fields: [token_type, expires_in, access_token, scope]\n  lifetime_seconds: 3600\n  refresh: >-\n    No refresh token is issued. Client-credentials tokens are re-minted on expiry;\n    Cisco's own openVulnQuery client regenerates the token on every call.\nrequest_usage:\n\
  \  header: 'Authorization: Bearer <access_token>'\n  accept: 'application/json (or application/xml — the API serves .json and .xml)'\n  example_base: https://apix.cisco.com/security/advisories/v2\ngateway:\n  vendor: Mashery\n  evidence: >-\n    api.cisco.com and apix.cisco.com both return \"Server: Mashery Proxy\". An\n    unauthenticated GET on a real path\n    (https://apix.cisco.com/security/advisories/v2/all) returns 403; unrouted paths\n    return 504. HEAD is not supported (596).\nunauthenticated_access: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/authentication/cisco-psirt-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Security
- Vulnerability Management
- Threat Intelligence
- Disclosure
- Compliance
- Networking
---
