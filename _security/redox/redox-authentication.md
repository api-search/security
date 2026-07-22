---
api_key_in: []
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Redox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Redox secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Redox
provider_slug: redox
scheme_count: 2
schemes:
- applies_to:
  - Redox FHIR API
  - Redox Data Model API
  - Redox Platform API
  authorization_endpoint: https://api.redoxengine.com/platform/v1/oauth/authorize
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://api.redoxengine.com
  jwks_uri: https://api.redoxengine.com/platform/v1/oauth/jwks.json
  name: RedoxPlatformOAuth
  registration_endpoint: https://api.redoxengine.com/platform/v1/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://api.redoxengine.com/platform/v1/oauth/revoke
  scopes_supported:
  - openid
  - offline_access
  - platform_access
  sources:
  - well-known/redox-oauth-authorization-server.json
  token_endpoint: https://api.redoxengine.com/platform/v1/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- applies_to:
  - Redox Platform API
  description: User-level API keys used to manage organizations, sources, and destinations.
  in: header
  name: platform-api-key
  sources:
  - https://docs.redoxengine.com/api-reference/platform-api/
  type: apiKey
slug: redox-authentication
source_filename: redox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.redoxengine.com/.well-known/oauth-authorization-server\ndocs: https://docs.redoxengine.com/basics/security/\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  oauth2_flows:\n  - authorizationCode\n  notes: >-\n    Redox exposes an RFC 8414 OAuth 2.0 authorization server at\n    https://api.redoxengine.com/.well-known/oauth-authorization-server. The FHIR and Data\n    Model APIs authenticate with OAuth2 bearer access tokens; the Platform API additionally\n    supports user-level API keys.\nschemes:\n- name: RedoxPlatformOAuth\n  type: oauth2\n  applies_to:\n  - Redox FHIR API\n  - Redox Data Model API\n  - Redox Platform API\n  issuer: https://api.redoxengine.com\n  authorization_endpoint: https://api.redoxengine.com/platform/v1/oauth/authorize\n  token_endpoint: https://api.redoxengine.com/platform/v1/oauth/token\n  revocation_endpoint: https://api.redoxengine.com/platform/v1/oauth/revoke\n  jwks_uri: https://api.redoxengine.com/platform/v1/oauth/jwks.json\n\
  \  registration_endpoint: https://api.redoxengine.com/platform/v1/oauth/register\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  code_challenge_methods_supported:\n  - S256\n  scopes_supported:\n  - openid\n  - offline_access\n  - platform_access\n  sources:\n  - well-known/redox-oauth-authorization-server.json\n- name: platform-api-key\n  type: apiKey\n  in: header\n  applies_to:\n  - Redox Platform API\n  description: User-level API keys used to manage organizations, sources, and destinations.\n  sources:\n  - https://docs.redoxengine.com/api-reference/platform-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redox/refs/heads/main/authentication/redox-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Healthcare
- Interoperability
- FHIR
- EHR
- Health Data
- Integration
- HL7
- Digital Health
- Healthcare API
---
