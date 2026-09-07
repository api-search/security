---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: benchmark-minerals-prices-api.yml
  format: yaml
  label: Benchmark Minerals API
  slug: benchmark-minerals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benchmark-minerals/refs/heads/main/openapi/benchmark-minerals-prices-api.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Benchmark Minerals Authentication
name_suffix: Authentication
oauth_flows: []
overview: Benchmark Minerals secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Benchmark Minerals
provider_slug: benchmark-minerals
scheme_count: 2
schemes:
- applies_to: all 36 operations
  base: https://api.benchmarkminerals.com/v2
  in: header
  name: api_key
  observed:
    body: '{"message":"Forbidden"}'
    note: AWS API Gateway rejects an unkeyed request at the edge with no discovery surface behind it.
    unauthenticated_status: 403
    url: https://api.benchmarkminerals.com/v2
  parameter: x-api-key
  provisioning: 'Self-service for existing subscribers only: "Your API key is available in the subscription section of your account. Simply log in to securely retrieve your API key" — https://www.benchmarkminerals.com/api. There is no public sign-up for an API key; a Benchmark subscription is a prerequisite.'
  rotation:
    documented: false
  sources:
  - openapi/benchmark-minerals-prices-api.yml
  - https://www.benchmarkminerals.com/api
  statement: 'info.description: "Access to our API is secured using an API key. Users must include their unique API key in the request header x-api-key to authenticate their requests."'
  surface: Prices REST API
  type: apiKey
- authorization_endpoint: https://mcp-auth.benchmarkminerals.com/oauth2/authorize
  endpoint: https://mcp.benchmarkminerals.com/mcp
  flow: bearer token
  issuer: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_GuiZRnNNK
  jwks_uri: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_GuiZRnNNK/.well-known/jwks.json
  name: mcp_oauth
  provisioning:
    documented: false
    note: No public page explains how to obtain an MCP client_id/client_secret; the surface is undocumented.
  response_types:
  - code
  - token
  revocation_endpoint: https://mcp-auth.benchmarkminerals.com/oauth2/revoke
  scopes:
  - benchmark-tools/sandbox.read
  - benchmark-tools/production.read
  signing_alg:
  - RS256
  sources:
  - https://mcp.benchmarkminerals.com/.well-known/oauth-protected-resource
  - well-known/benchmark-minerals-cognito-openid-configuration.json
  surface: MCP gateway
  token_endpoint: https://mcp-auth.benchmarkminerals.com/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://mcp-auth.benchmarkminerals.com/oauth2/userInfo
slug: benchmark-minerals-authentication
source_filename: benchmark-minerals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://www.benchmarkminerals.com/prices-api.yml + https://www.benchmarkminerals.com/api + https://mcp.benchmarkminerals.com/.well-known/oauth-protected-resource\ndocs: https://www.benchmarkminerals.com/api\nprovider: Benchmark Minerals\nproviderId: benchmark-minerals\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  surfaces: 2\n  note: Two independent auth models on two independent surfaces; a credential for one does not work on\n    the other.\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  surface: Prices REST API\n  base: https://api.benchmarkminerals.com/v2\n  applies_to: all 36 operations\n  provisioning: 'Self-service for existing subscribers only: \"Your API key is available in the subscription\n    section of your account. Simply log in to securely retrieve your API key\" — https://www.benchmarkminerals.com/api.\n    There is no public sign-up for an API\
  \ key; a Benchmark subscription is a prerequisite.'\n  rotation:\n    documented: false\n  statement: 'info.description: \"Access to our API is secured using an API key. Users must include their\n    unique API key in the request header x-api-key to authenticate their requests.\"'\n  sources:\n  - openapi/benchmark-minerals-prices-api.yml\n  - https://www.benchmarkminerals.com/api\n  observed:\n    url: https://api.benchmarkminerals.com/v2\n    unauthenticated_status: 403\n    body: '{\"message\":\"Forbidden\"}'\n    note: AWS API Gateway rejects an unkeyed request at the edge with no discovery surface behind it.\n- name: mcp_oauth\n  type: oauth2\n  flow: bearer token\n  surface: MCP gateway\n  endpoint: https://mcp.benchmarkminerals.com/mcp\n  issuer: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_GuiZRnNNK\n  authorization_endpoint: https://mcp-auth.benchmarkminerals.com/oauth2/authorize\n  token_endpoint: https://mcp-auth.benchmarkminerals.com/oauth2/token\n  revocation_endpoint:\
  \ https://mcp-auth.benchmarkminerals.com/oauth2/revoke\n  userinfo_endpoint: https://mcp-auth.benchmarkminerals.com/oauth2/userInfo\n  jwks_uri: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_GuiZRnNNK/.well-known/jwks.json\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  response_types:\n  - code\n  - token\n  signing_alg:\n  - RS256\n  scopes:\n  - benchmark-tools/sandbox.read\n  - benchmark-tools/production.read\n  provisioning:\n    documented: false\n    note: No public page explains how to obtain an MCP client_id/client_secret; the surface is undocumented.\n  sources:\n  - https://mcp.benchmarkminerals.com/.well-known/oauth-protected-resource\n  - well-known/benchmark-minerals-cognito-openid-configuration.json\ngaps:\n- issue: no auth error schema\n  impact: 401 and 403 are declared with a description only; an agent cannot machine-read whether a failure\n    is a bad key or an unentitled market\n- issue: no documented key rotation or expiry\n\
  \  impact: long-lived agent credentials have no published lifecycle\n- issue: the OAuth surface is undocumented\n  impact: the only way to learn the MCP auth model is to probe the gateway\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchmark-minerals/refs/heads/main/authentication/benchmark-minerals-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Batteries
- Cobalt
- Critical Minerals
- Electric Vehicles
- Energy Transition
- Graphite
- Lithium
- Lithium-Ion
- Market Intelligence
- Mining
- Nickel
- Price Reporting
- Rare Earths
- Supply Chain
---
