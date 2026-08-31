---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Todyl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Todyl declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Todyl
provider_slug: todyl
scheme_count: 1
schemes:
- description: 'A paired credential: a client identifier and an access token, both sent as request headers on every call. Todyl calls this an "External API token".'
  evidence:
  - body: '{"error":{"code":"auth_missing_token","message":"Credentials missing or invalid.","request_id":"req_..."}}'
    probe: GET https://api.todyl.com/v1/devices with no credentials
    status: 401
  - body: '{"error":{"code":"auth_malformed_token","message":"Credentials missing or invalid.","request_id":"req_..."}}'
    note: The error code CHANGED from auth_missing_token to auth_malformed_token, which is what proves the service recognises these two header names. Without that differential the header names would be an unverified third-party claim.
    probe: GET https://api.todyl.com/v1/devices with X-Todyl-Client-Id and X-Todyl-Access-Token set to deliberately invalid values
    status: 401
  id: todyl_external_api_token
  in: header
  names:
  - X-Todyl-Client-Id
  - X-Todyl-Access-Token
  token_issuance:
    portal: https://portal.todyl.com/session/login
    self_service: true
    verified: Named verbatim in the community MCP client's required-env error message; the portal path itself is behind the customer login and was not opened.
    where: Todyl portal — Account -> Developer APIs -> External API Tokens
  type: apiKey
slug: todyl-authentication
source_filename: todyl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of https://api.todyl.com/v1/devices on 2026-08-30, corroborated by the\n  token-creation path named in the community MCP client at\n  https://github.com/shaank0/todyl-mcp/blob/main/src/config.ts\napi: Todyl External API\nbase_url: https://api.todyl.com\ndocs: null\ndocs_note: >-\n  Todyl publishes no public authentication reference page. The API reference lives in the\n  customer-authenticated knowledge base at support.todyl.com, which answers the root URL with a\n  sign-in page (Next.js SignInPage route, robots noindex/nofollow/noarchive).\nschemes:\n- id: todyl_external_api_token\n  type: apiKey\n  in: header\n  names:\n  - X-Todyl-Client-Id\n  - X-Todyl-Access-Token\n  description: >-\n    A paired credential: a client identifier and an access token, both sent as request headers on\n    every call. Todyl calls this an \"External API token\".\n  evidence:\n    - probe: GET https://api.todyl.com/v1/devices\
  \ with no credentials\n      status: 401\n      body: '{\"error\":{\"code\":\"auth_missing_token\",\"message\":\"Credentials missing or invalid.\",\"request_id\":\"req_...\"}}'\n    - probe: >-\n        GET https://api.todyl.com/v1/devices with X-Todyl-Client-Id and X-Todyl-Access-Token set to\n        deliberately invalid values\n      status: 401\n      body: '{\"error\":{\"code\":\"auth_malformed_token\",\"message\":\"Credentials missing or invalid.\",\"request_id\":\"req_...\"}}'\n      note: >-\n        The error code CHANGED from auth_missing_token to auth_malformed_token, which is what proves\n        the service recognises these two header names. Without that differential the header names\n        would be an unverified third-party claim.\n  token_issuance:\n    where: Todyl portal — Account -> Developer APIs -> External API Tokens\n    portal: https://portal.todyl.com/session/login\n    self_service: true\n    verified: >-\n      Named verbatim in the community MCP client's required-env\
  \ error message; the portal path\n      itself is behind the customer login and was not opened.\noauth2: false\nopenid_connect: false\nmutual_tls: unknown\nscopes:\n  documented: false\n  note: >-\n    No scope or permission reference is public. Whether External API tokens carry scopes, and what\n    they are, cannot be established without a customer account.\ngating:\n  contract_public: false\n  reference_public: false\n  note: >-\n    Every path on api.todyl.com — including /openapi.json, /v1/openapi.json and /.well-known/* —\n    returns 401 auth_missing_token. There is no anonymous surface on the API host at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/todyl/refs/heads/main/authentication/todyl-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Cybersecurity
- Security
- Managed Service Providers
- SASE
- SIEM
- Endpoint Security
- Managed Detection and Response
- Governance Risk and Compliance
- Zero Trust
- Networking
---
