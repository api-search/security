---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Deep Sentinel Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Deep Sentinel secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Deep Sentinel
provider_slug: deep-sentinel
scheme_count: 1
schemes:
- authorization_endpoint: https://account.deepsentinel.com/authentication/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://account.deepsentinel.com/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/26153082
  jwks_uri: https://account.deepsentinel.com/authentication/.well-known/jwks.json
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://shop.deepsentinel.com/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/deep-sentinel-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://account.deepsentinel.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: deep-sentinel-authentication
source_filename: deep-sentinel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://shop.deepsentinel.com/.well-known/openid-configuration\nnote: >-\n  Derived entirely from the OpenID Connect discovery and RFC 8414 / RFC 9728 metadata\n  Deep Sentinel serves from its own hosts. There is no OpenAPI in this repo to derive\n  securitySchemes from, and Deep Sentinel publishes no developer authentication\n  documentation of its own — this profile covers the customer-account identity layer on\n  the store host only. The two MCP endpoints under shop.deepsentinel.com answered\n  `tools/list` ANONYMOUSLY (no bearer token required); the OAuth layer below gates the\n  authenticated Customer Account API and Customer Account MCP API, not anonymous\n  catalog/checkout discovery.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_surfaces:\n  - https://shop.deepsentinel.com/api/mcp\n  - https://shop.deepsentinel.com/api/ucp/mcp\nschemes:\n- name: shopify-customer-account-oidc\n\
  \  type: openIdConnect\n  openIdConnectUrl: https://shop.deepsentinel.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/26153082\n  authorization_endpoint: https://account.deepsentinel.com/authentication/oauth/authorize\n  token_endpoint: https://account.deepsentinel.com/authentication/oauth/token\n  end_session_endpoint: https://account.deepsentinel.com/authentication/logout\n  jwks_uri: https://account.deepsentinel.com/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  sources: [well-known/deep-sentinel-openid-configuration.json]\nprotected_resources:\n- resource: https://shop.deepsentinel.com\n  authorization_servers:\n\
  \  - https://account.deepsentinel.com\n  - https://shopify.com/authentication/26153082\n  bearer_methods_supported: [header]\n  source: well-known/deep-sentinel-oauth-protected-resource.json\n- resource: https://account.deepsentinel.com\n  authorization_servers:\n  - https://account.deepsentinel.com\n  - https://shopify.com/authentication/26153082\n  bearer_methods_supported: [header]\n  source: https://account.deepsentinel.com/.well-known/oauth-protected-resource\nscopes_reference: scopes/deep-sentinel-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deep-sentinel/refs/heads/main/authentication/deep-sentinel-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Security
- Physical Security
- Video Surveillance
- Home Security
- Artificial Intelligence
- Computer Vision
- Monitoring
- Internet of Things
- Commerce
---
