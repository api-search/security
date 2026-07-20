---
api_key_in: []
api_specs:
- filename: curlec-razorpay-openapi.json
  format: json
  label: Razorpay Curlec REST API
  slug: razorpay-curlec-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curlec/refs/heads/main/openapi/curlec-razorpay-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Curlec Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Curlec secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Curlec
provider_slug: curlec
scheme_count: 2
schemes:
- description: HTTP Basic authentication using your Razorpay API key pair. Use key_id as the username and key_secret as the password. Encode as Base64(key_id:key_secret). Keys are environment-scoped (Test vs Live). Obtain keys at https://dashboard.razorpay.com/app/keys. Keys are case-sensitive.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/curlec-razorpay-openapi.json
  type: http
- description: OAuth 2.0 via the Razorpay MCP server (mcp.razorpay.com). Supports Authorization Code with PKCE (S256) for user-delegated access and Client Credentials for server-to-server access. Tokens expire in 3600 seconds. Dynamic Client Registration available at the registration endpoint. For integration setup see https://razorpay.com/docs/build/llm-docs/mcp-server/oauth.md.
  flows:
  - authorizationUrl: https://mcp.razorpay.com/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://mcp.razorpay.com/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://mcp.razorpay.com/token
  name: oauth2
  sources:
  - openapi/curlec-razorpay-openapi.json
  type: oauth2
slug: curlec-authentication
source_filename: curlec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/curlec-razorpay-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using your Razorpay API key pair. Use key_id as the\n    username and key_secret as the password. Encode as Base64(key_id:key_secret). Keys are environment-scoped\n    (Test vs Live). Obtain keys at https://dashboard.razorpay.com/app/keys. Keys are case-sensitive.\n  sources:\n  - openapi/curlec-razorpay-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.razorpay.com/authorize\n    tokenUrl: https://mcp.razorpay.com/token\n    scopes: 1\n  - flow: clientCredentials\n    tokenUrl: https://mcp.razorpay.com/token\n    scopes: 1\n  description: OAuth 2.0 via the Razorpay MCP server (mcp.razorpay.com). Supports Authorization\n\
  \    Code with PKCE (S256) for user-delegated access and Client Credentials for server-to-server\n    access. Tokens expire in 3600 seconds. Dynamic Client Registration available at the registration\n    endpoint. For integration setup see https://razorpay.com/docs/build/llm-docs/mcp-server/oauth.md.\n  sources:\n  - openapi/curlec-razorpay-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curlec/refs/heads/main/authentication/curlec-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Payments
- Payment Gateway
- Recurring Payments
- Subscriptions
- Direct Debit
- FinTech
- Malaysia
- DuitNow
- FPX
- Webhooks
- Razorpay
---
