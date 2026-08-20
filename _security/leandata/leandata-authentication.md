---
api_key_in:
- header
api_specs:
- filename: leandata-availability-api-openapi.yml
  format: yaml
  label: LeanData 🗓️ Availability API
  slug: leandata-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-availability-api-openapi.yml
- filename: leandata-legacy-still-supported-api-openapi.yml
  format: yaml
  label: LeanData Legacy (still supported) API
  slug: leandata-legacy-still-supported-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-legacy-still-supported-api-openapi.yml
- filename: leandata-matching-api-openapi.yml
  format: yaml
  label: LeanData Matching API
  slug: leandata-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-matching-api-openapi.yml
- filename: leandata-meetings-create-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Create API
  slug: leandata-meetings-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-create-api-openapi.yml
- filename: leandata-meetings-manage-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Manage API
  slug: leandata-meetings-manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-manage-api-openapi.yml
- filename: leandata-meetings-retrieve-api-openapi.yml
  format: yaml
  label: LeanData 📆 Meetings > Retrieve API
  slug: leandata-meetings-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-meetings-retrieve-api-openapi.yml
- filename: leandata-one-time-routing-api-openapi.yml
  format: yaml
  label: LeanData One Time Routing API
  slug: leandata-one-time-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-one-time-routing-api-openapi.yml
- filename: leandata-retrieve-routing-graphs-information-api-openapi.yml
  format: yaml
  label: LeanData Retrieve Routing Graphs Information API
  slug: leandata-retrieve-routing-graphs-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-retrieve-routing-graphs-information-api-openapi.yml
- filename: leandata-scheduling-inputs-api-openapi.yml
  format: yaml
  label: LeanData 🧠 Scheduling Inputs API
  slug: leandata-scheduling-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/openapi/leandata-scheduling-inputs-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: 'LeanData runs three distinct authentication models across three distinct hosts, and a consumer has to know which product they are calling before they can pick one. The BookIt and Graph REST APIs on api.leandata.com use a server-side API key in an X-Api-Key header. The Matching and Round Robin APIs are not LeanData-hosted at all — they are dispatched through the customer''s own Salesforce org via the managed package''s Apex REST endpoint and authenticate with a Salesforce OAuth 2.0 Connected App session. The BookIt MCP server on mcp.leandata.com is the newest and the only one with machine-readable discovery: OAuth 2.1 authorization-code + PKCE with dynamic client registration and a real scope model. None of the harvested OpenAPI files declare a securityScheme, so this profile was built by reading LeanData''s published documentation rather than derived from the specs — running derive-authentication.py against openapi/ yields zero schemes.'
kind: authentication
layout: security
method: searched
name: Leandata Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: LeanData secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: LeanData
provider_slug: leandata
scheme_count: 4
schemes:
- applies_to:
  - openapi/leandata-scheduling-inputs-api-openapi.yml
  - openapi/leandata-availability-api-openapi.yml
  - openapi/leandata-meetings-retrieve-api-openapi.yml
  - openapi/leandata-meetings-create-api-openapi.yml
  - openapi/leandata-meetings-manage-api-openapi.yml
  - openapi/leandata-legacy-still-supported-api-openapi.yml
  failure: HTTP 401 Unauthorized
  host: https://api.leandata.com
  in: header
  name: BookItApiKey
  observed_unauthenticated_response: '{"message":"Unauthorized"}'
  parameter_name: X-Api-Key
  provisioning: Obtain a valid API key by contacting your LeanData Solutions Engineering Team. There is no self-service key issuance.
  rules:
  - All requests must be made over HTTPS; requests made over HTTP are rejected.
  - Server-side only. LeanData explicitly warns that API keys must not be exposed in client-side code or browser-based applications.
  - The API does not support bulk updates; only one object can be modified per request.
  sources:
  - https://docs.leandata.com
  type: apiKey
- applies_to:
  - openapi/leandata-one-time-routing-api-openapi.yml
  - openapi/leandata-retrieve-routing-graphs-information-api-openapi.yml
  failure: HTTP 401 Unauthorized
  host: https://api.leandata.com
  in: header
  name: GraphApiKey
  observed_unauthenticated_response: '{"message":"Unauthorized"}'
  parameter_name: X-Api-Key
  provisioning: Obtain a valid API key via the LeanData admin settings page — Settings > Admin > Authorization. Unlike BookIt, Graph API keys are self-service for an org admin.
  sources:
  - https://docs.leandata.com
  type: apiKey
- applies_to:
  - openapi/leandata-matching-api-openapi.yml
  endpoint: /services/apexrest/LeanData/LeanDataAPI
  failure: Salesforce error envelope, e.g. {"message":"Session expired or invalid","errorCode":"INVALID_SESSION_ID"}
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    refresh: supported
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  host: https://<your-instance>.my.salesforce.com
  name: SalesforceConnectedApp
  note: This is Salesforce's auth, not LeanData's. The access token, instance URL and refresh token all come from Salesforce, and the request is executed inside the customer's own org under the managed package's Apex REST service.
  provisioning: Customer builds their own Salesforce OAuth Connected App (client id, client secret, redirect URL), authorizes the LeanData token from the LeanData tab in Salesforce, and asks their LeanData CSM to provision the Matching API for that Salesforce org id. Partners request access at partners@leandatainc.com.
  sources:
  - https://docs.leandata.com
  type: oauth2
- bearer_methods_supported:
  - header
  dynamic_client_registration: true
  failure: 'HTTP 401 {"error":"Missing or invalid Authorization header"} with WWW-Authenticate: Bearer resource_metadata=".../.well-known/oauth-protected-resource"'
  flows:
  - authorizationUrl: https://mcp.leandata.com/authorize
    flow: authorizationCode
    pkce: S256
    refresh: supported
    tokenUrl: https://mcp.leandata.com/token
  host: https://mcp.leandata.com
  identity:
  - Salesforce OAuth for LeanData admins and reps; the caller's BookIt permission set is detected after login
  - One-time code for external partners or AI agents that have no Salesforce credentials in the org; an email address and a permission set are assigned in advance
  name: BookItMcpOAuth
  registration_endpoint: https://mcp.leandata.com/register
  resource: https://mcp.leandata.com
  scopes:
  - admin
  - user
  - partner
  - offline_access
  sources:
  - https://mcp.leandata.com/.well-known/oauth-authorization-server
  - https://mcp.leandata.com/.well-known/oauth-protected-resource
  - https://www.leandata.com/resources/leandatas-bookit-mcp/
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: leandata-authentication
source_filename: leandata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.leandata.com\ndocs:\n  - https://docs.leandata.com\n  - https://mcp.leandata.com/.well-known/oauth-authorization-server\ndescription: >-\n  LeanData runs three distinct authentication models across three distinct hosts, and a\n  consumer has to know which product they are calling before they can pick one. The BookIt\n  and Graph REST APIs on api.leandata.com use a server-side API key in an X-Api-Key header.\n  The Matching and Round Robin APIs are not LeanData-hosted at all — they are dispatched\n  through the customer's own Salesforce org via the managed package's Apex REST endpoint and\n  authenticate with a Salesforce OAuth 2.0 Connected App session. The BookIt MCP server on\n  mcp.leandata.com is the newest and the only one with machine-readable discovery: OAuth 2.1\n  authorization-code + PKCE with dynamic client registration and a real scope model.\n  None of the harvested OpenAPI files declare a securityScheme,\
  \ so this profile was built by\n  reading LeanData's published documentation rather than derived from the specs — running\n  derive-authentication.py against openapi/ yields zero schemes.\n\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_names: [X-Api-Key]\n  oauth2_flows: [authorizationCode, refreshToken]\n  transport: https-only\n  spec_declared: false\n  spec_note: >-\n    Zero securitySchemes across all nine refined OpenAPI files and all three _original files.\n    This is the single largest contract-quality gap in the LeanData surface: an agent reading\n    the spec alone cannot tell how to authenticate.\n\nschemes:\n  - name: BookItApiKey\n    type: apiKey\n    in: header\n    parameter_name: X-Api-Key\n    applies_to:\n      - openapi/leandata-scheduling-inputs-api-openapi.yml\n      - openapi/leandata-availability-api-openapi.yml\n      - openapi/leandata-meetings-retrieve-api-openapi.yml\n      - openapi/leandata-meetings-create-api-openapi.yml\n      -\
  \ openapi/leandata-meetings-manage-api-openapi.yml\n      - openapi/leandata-legacy-still-supported-api-openapi.yml\n    host: https://api.leandata.com\n    provisioning: >-\n      Obtain a valid API key by contacting your LeanData Solutions Engineering Team. There is\n      no self-service key issuance.\n    failure: HTTP 401 Unauthorized\n    observed_unauthenticated_response: '{\"message\":\"Unauthorized\"}'\n    rules:\n      - All requests must be made over HTTPS; requests made over HTTP are rejected.\n      - >-\n        Server-side only. LeanData explicitly warns that API keys must not be exposed in\n        client-side code or browser-based applications.\n      - The API does not support bulk updates; only one object can be modified per request.\n    sources:\n      - https://docs.leandata.com\n\n  - name: GraphApiKey\n    type: apiKey\n    in: header\n    parameter_name: X-Api-Key\n    applies_to:\n      - openapi/leandata-one-time-routing-api-openapi.yml\n      - openapi/leandata-retrieve-routing-graphs-information-api-openapi.yml\n\
  \    host: https://api.leandata.com\n    provisioning: >-\n      Obtain a valid API key via the LeanData admin settings page — Settings > Admin >\n      Authorization. Unlike BookIt, Graph API keys are self-service for an org admin.\n    failure: HTTP 401 Unauthorized\n    observed_unauthenticated_response: '{\"message\":\"Unauthorized\"}'\n    sources:\n      - https://docs.leandata.com\n\n  - name: SalesforceConnectedApp\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n        tokenUrl: https://login.salesforce.com/services/oauth2/token\n        refresh: supported\n    applies_to:\n      - openapi/leandata-matching-api-openapi.yml\n    host: https://<your-instance>.my.salesforce.com\n    endpoint: /services/apexrest/LeanData/LeanDataAPI\n    provisioning: >-\n      Customer builds their own Salesforce OAuth Connected App (client id, client secret,\n      redirect URL), authorizes the LeanData\
  \ token from the LeanData tab in Salesforce, and\n      asks their LeanData CSM to provision the Matching API for that Salesforce org id.\n      Partners request access at partners@leandatainc.com.\n    failure: >-\n      Salesforce error envelope, e.g.\n      {\"message\":\"Session expired or invalid\",\"errorCode\":\"INVALID_SESSION_ID\"}\n    note: >-\n      This is Salesforce's auth, not LeanData's. The access token, instance URL and refresh\n      token all come from Salesforce, and the request is executed inside the customer's own org\n      under the managed package's Apex REST service.\n    sources:\n      - https://docs.leandata.com\n\n  - name: BookItMcpOAuth\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.leandata.com/authorize\n        tokenUrl: https://mcp.leandata.com/token\n        refresh: supported\n        pkce: S256\n    registration_endpoint: https://mcp.leandata.com/register\n    dynamic_client_registration: true\n\
  \    token_endpoint_auth_methods: [none]\n    bearer_methods_supported: [header]\n    scopes: [admin, user, partner, offline_access]\n    host: https://mcp.leandata.com\n    resource: https://mcp.leandata.com\n    identity:\n      - Salesforce OAuth for LeanData admins and reps; the caller's BookIt permission set is detected after login\n      - >-\n        One-time code for external partners or AI agents that have no Salesforce credentials\n        in the org; an email address and a permission set are assigned in advance\n    failure: >-\n      HTTP 401 {\"error\":\"Missing or invalid Authorization header\"} with\n      WWW-Authenticate: Bearer resource_metadata=\".../.well-known/oauth-protected-resource\"\n    sources:\n      - https://mcp.leandata.com/.well-known/oauth-authorization-server\n      - https://mcp.leandata.com/.well-known/oauth-protected-resource\n      - https://www.leandata.com/resources/leandatas-bookit-mcp/\n\nrecommendations:\n  - >-\n    Declare the X-Api-Key apiKey\
  \ securityScheme in the published BookIt and Graph OpenAPI and\n    apply it at the document level. Today the specs are silent and every consumer has to read\n    prose to authenticate.\n  - >-\n    Publish the MCP scope semantics (what admin / user / partner each grant) alongside the\n    protected-resource metadata; the scope names are discoverable but their meaning is not.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leandata/refs/heads/main/authentication/leandata-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Revenue Operations
- Lead Routing
- Lead to Account Matching
- Salesforce
- Sales Engagement
- Sales Productivity
- Marketing Operations
- Scheduling
- Meeting Booking
- Account Based Marketing
- Buying Groups
- Signal Orchestration
- Go-To-Market
- CRM
- AppExchange
---
