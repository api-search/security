---
api_key_in: []
auth_types:
- http-basic
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Imperson Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imperson secures its APIs with http-basic and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Imperson
provider_slug: imperson
scheme_count: 2
schemes:
- documented_by_provider: false
  evidence: 'HTTP 401 with ''WWW-Authenticate: Basic realm="messaging.api"'' returned for every path probed on api.imperson.com (/, /api, /docs, /swagger, /openapi.json, /.well-known/*). Server header ''Microsoft-IIS/10.0'', ''x-powered-by: ASP.NET''. Host resolves to messagingapi-env.ntktwhrm2k.us-east-1.elasticbeanstalk.com (AWS Elastic Beanstalk).'
  host: https://api.imperson.com
  name: messaging-api-basic
  probed: '2026-08-14'
  realm: messaging.api
  scheme: basic
  type: http
- documented_by_provider: false
  evidence: Imperson's free self-service chatbot builder (linked from https://www.imperson.com/toolbox) is a React SPA that ships auth0-js and exchanges tokens through https://auth0-proxy-dot-toolbox-235607.appspot.com/userinfo, with custom claims namespaced under https://imperson.com/ (app_metadata, email, name, user_id). This is end-user login for the app, not a documented developer authorization flow — no client registration, scope reference, or token endpoint is published.
  host: https://toolbox.imperson.com
  name: toolbox-auth0
  probed: '2026-08-14'
  type: oauth2
  vendor: Auth0
slug: imperson-authentication
source_filename: imperson-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  live HTTP probes of api.imperson.com plus the publicly-served JavaScript bundle of Imperson's own\n  self-service app at https://toolbox.imperson.com/static/js/main.9d3efa87.chunk.js\ndocs: null\nnotes: >-\n  Imperson publishes NO authentication documentation, no developer portal, and no OpenAPI. Everything\n  below was established by probing hosts the company controls; nothing here is derived from a\n  specification because none exists. This file exists to record that a real, reachable product API host\n  was confirmed and to describe the authentication challenge it actually returns — it is NOT evidence\n  that the provider documents its authentication, and no `type: Authentication` pointer is emitted in\n  apis.yml for that reason.\nschemes:\n- name: messaging-api-basic\n  type: http\n  scheme: basic\n  realm: messaging.api\n  host: https://api.imperson.com\n  evidence: >-\n    HTTP 401 with 'WWW-Authenticate: Basic realm=\"\
  messaging.api\"' returned for every path probed on\n    api.imperson.com (/, /api, /docs, /swagger, /openapi.json, /.well-known/*). Server header\n    'Microsoft-IIS/10.0', 'x-powered-by: ASP.NET'. Host resolves to\n    messagingapi-env.ntktwhrm2k.us-east-1.elasticbeanstalk.com (AWS Elastic Beanstalk).\n  documented_by_provider: false\n  probed: '2026-08-14'\n- name: toolbox-auth0\n  type: oauth2\n  vendor: Auth0\n  host: https://toolbox.imperson.com\n  evidence: >-\n    Imperson's free self-service chatbot builder (linked from https://www.imperson.com/toolbox) is a\n    React SPA that ships auth0-js and exchanges tokens through\n    https://auth0-proxy-dot-toolbox-235607.appspot.com/userinfo, with custom claims namespaced under\n    https://imperson.com/ (app_metadata, email, name, user_id). This is end-user login for the app,\n    not a documented developer authorization flow — no client registration, scope reference, or token\n    endpoint is published.\n  documented_by_provider: false\n\
  \  probed: '2026-08-14'\nsummary:\n  types: [http-basic, oauth2]\n  api_key_in: []\n  oauth2_flows: []\n  public_reference_published: false\n  spec_backed: false\nanonymous_surfaces:\n- url: https://api.imperson.com/health\n  status: 200\n  body: '\"OK\"'\n  note: the only unauthenticated response observed on the product API host\n- url: https://www.imperson.com/_api/mcp\n  status: 200\n  auth: none\n  note: >-\n    Wix Site MCP endpoint — anonymous, but it is the Wix platform's site surface, not Imperson's\n    product API. See mcp/imperson-mcp.yml.\nx-evidence:\n- url: https://api.imperson.com/\n  status: 401\n  header: 'WWW-Authenticate: Basic realm=\"messaging.api\"'\n- url: https://api.imperson.com/health\n  status: 200\n- url: https://docs.imperson.com/\n  status: 302\n  note: redirects to http://drive.google.com/a/imperson.com — a Google Workspace Drive, not public docs\n- url: https://www.imperson.com/developers\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imperson/refs/heads/main/authentication/imperson-authentication.yml
summary_line: http-basic/oauth2 · 2 schemes
tags:
- Company
- Conversational AI
- Chatbots
- Customer Support
- Lead Generation
- Sales Automation
- Enterprise
- Model Context Protocol
---
