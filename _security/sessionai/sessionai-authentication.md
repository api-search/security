---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sessionai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Session AI secures its APIs with apiKey and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Session AI
provider_slug: sessionai
scheme_count: 5
schemes:
- description: The API key used to authenticate REST API calls. Master API keys are created in the C3 console; additional keys can be issued per site, app, or partner channel. The same key authenticates the HTML5/Android/iOS SDKs.
  in: header
  name: apikey
  parameter_name: apikey
  required: true
  sources:
  - https://devguide.zineone.com/docs/send-events
  - https://docs.zineone.com/docs/create-manage-master-api-keys
  type: apiKey
- description: Optional alternative to the apikey header. Access tokens are generated server-side. Documented as interchangeable with apikey on every public REST operation.
  in: header
  name: accesstoken
  parameter_name: accesstoken
  required: false
  sources:
  - https://devguide.zineone.com/docs/send-events
  type: apiKey
- description: Microservices are individually configured as public (no API key; the tenant namespace is passed as a query parameter instead) or restricted (a per-microservice API key is generated in the console).
  in: header
  name: microservice-api-key
  parameter_name: apikey
  required: false
  sources:
  - https://docs.zineone.com/docs/microservices
  type: apiKey
- description: The /c3/data/profile/detail and /c3/data/activity/all endpoints are documented as requiring a valid Session AI portal login rather than an API key.
  name: portal-session
  scheme: session
  sources:
  - https://devguide.zineone.com/docs/retrieve-profile-details
  - https://devguide.zineone.com/docs/retrieve-customer-activity
  type: http
- description: 'The remote MCP server at https://sessionai.com/mcp answers anonymous requests with HTTP 401 and WWW-Authenticate: Bearer realm="mcp", advertising RFC 9728 protected-resource metadata. The authorization server supports dynamic client registration (RFC 7591).'
  flows:
  - authorizationUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    registrationUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/clients/register
    scopes:
    - openid
    - profile
    - email
    - phone
    - offline_access
    tokenUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/token
  name: mcp-oauth
  sources:
  - well-known/sessionai-oauth-protected-resource.json
  - well-known/sessionai-oauth-authorization-server.json
  type: oauth2
slug: sessionai-authentication
source_filename: sessionai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://devguide.zineone.com/docs/rest-api-reference\ndocs: https://devguide.zineone.com/docs/send-events\nnote: >-\n  Session AI publishes no OpenAPI, so this profile is read from the published developer\n  guide (the parameter tables repeated on every REST operation page) plus the live\n  RFC 9728 protected-resource metadata for the MCP server. derive-authentication.py was\n  run and produced nothing, as there is no spec in openapi/ to derive from.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  surfaces:\n  - REST platform API — apikey header\n  - Remote MCP server — OAuth 2.0 bearer\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter_name: apikey\n  required: true\n  description: >-\n    The API key used to authenticate REST API calls. Master API keys are created in the\n    C3 console; additional keys can be issued per site, app, or partner\
  \ channel. The same\n    key authenticates the HTML5/Android/iOS SDKs.\n  sources:\n  - https://devguide.zineone.com/docs/send-events\n  - https://docs.zineone.com/docs/create-manage-master-api-keys\n- name: accesstoken\n  type: apiKey\n  in: header\n  parameter_name: accesstoken\n  required: false\n  description: >-\n    Optional alternative to the apikey header. Access tokens are generated server-side.\n    Documented as interchangeable with apikey on every public REST operation.\n  sources:\n  - https://devguide.zineone.com/docs/send-events\n- name: microservice-api-key\n  type: apiKey\n  in: header\n  parameter_name: apikey\n  required: false\n  description: >-\n    Microservices are individually configured as public (no API key; the tenant namespace\n    is passed as a query parameter instead) or restricted (a per-microservice API key is\n    generated in the console).\n  sources:\n  - https://docs.zineone.com/docs/microservices\n- name: portal-session\n  type: http\n  scheme: session\n\
  \  description: >-\n    The /c3/data/profile/detail and /c3/data/activity/all endpoints are documented as\n    requiring a valid Session AI portal login rather than an API key.\n  sources:\n  - https://devguide.zineone.com/docs/retrieve-profile-details\n  - https://devguide.zineone.com/docs/retrieve-customer-activity\n- name: mcp-oauth\n  type: oauth2\n  description: >-\n    The remote MCP server at https://sessionai.com/mcp answers anonymous requests with\n    HTTP 401 and WWW-Authenticate: Bearer realm=\"mcp\", advertising RFC 9728\n    protected-resource metadata. The authorization server supports dynamic client\n    registration (RFC 7591).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/token\n    registrationUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/clients/register\n    scopes:\n    - openid\n    - profile\n    - email\n\
  \    - phone\n    - offline_access\n  sources:\n  - well-known/sessionai-oauth-protected-resource.json\n  - well-known/sessionai-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sessionai/refs/heads/main/authentication/sessionai-authentication.yml
summary_line: apiKey/oauth2 · 5 schemes
tags:
- Company
- Artificial Intelligence
- E-Commerce
- Retail
- Personalization
- Marketing
- Agentic AI
- Decisioning
- Customer Data
- Event
- Real-Time
- MCP
---
