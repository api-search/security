---
api_key_in: []
api_specs:
- filename: boxc-openapi-original.yml
  format: yaml
  label: BoxC API
  slug: boxc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boxc/refs/heads/main/openapi/boxc-openapi-original.yml
auth_types:
- oauth2
- openIdConnect
- http
description: ''
kind: authentication
layout: security
method: searched
name: Boxc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
overview: Boxc secures its APIs with oauth2, openIdConnect, and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and clientCredentials flow(s).
provider_name: Boxc
provider_slug: boxc
scheme_count: 2
schemes:
- bearer_format: JWT
  description: 'All operations require a JSON Web Token obtained after completing an OAuth 2.0 flow. Presented as `Authorization: Bearer <jwt>`.'
  name: JWT
  scheme: bearer
  sources:
  - openapi/boxc-openapi-original.yml
  type: http
- bearer_format: JWT
  description: Some operations require a client with special privileges granted by BoxC. No additional scope is needed beyond the privileged-client grant.
  name: PrivilegedClient
  scheme: bearer
  sources:
  - openapi/boxc-openapi-original.yml
  type: http
slug: boxc-authentication
source_filename: boxc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/boxc-openapi-original.yml\ndocs: https://docs.boxc.com/#tag/Authentication\noidc_discovery: https://accounts.boxc.com/.well-known/openid-configuration\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - clientCredentials\nmodel: >-\n  BoxC uses OAuth 2.0 / OpenID Connect. Clients are created in the BoxC account (up to\n  two per account) and users authorize a client to obtain an access token. Access tokens\n  are RS256-signed JSON Web Tokens (JWT) presented as a Bearer token in the Authorization\n  header on every API request against https://api.boxc.com/v1. The entire authorization\n  workflow runs at accounts.boxc.com.\nauthorization_server:\n  issuer: https://accounts.boxc.com\n  authorization_endpoint: https://accounts.boxc.com/auth/v1/authorize\n  token_endpoint: https://accounts.boxc.com/auth/v1/token\n  revocation_endpoint:\
  \ https://accounts.boxc.com/auth/v1/revoke\n  registration_endpoint: https://accounts.boxc.com/auth/v1/register\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  response_types_supported:\n  - code\n  - token\n  - id_token\n  - id_token token\n  - none\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - implicit\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    All operations require a JSON Web Token obtained after completing an OAuth 2.0 flow.\n    Presented as `Authorization: Bearer <jwt>`.\n  sources:\n  - openapi/boxc-openapi-original.yml\n- name: PrivilegedClient\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Some operations require a client with special privileges granted by BoxC. No\n    additional scope is needed beyond the privileged-client grant.\n  sources:\n  - openapi/boxc-openapi-original.yml\n\
  notes: >-\n  The OpenAPI securityDefinitions model the runtime credential as an http bearer JWT;\n  the OAuth 2.0 / OIDC authorization-code, implicit and client_credentials grants that\n  mint those JWTs are documented in the Authentication tag and confirmed by the live\n  OIDC discovery document. Client management and permission (scope) selection are done\n  in the BoxC Support Center.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boxc/refs/heads/main/authentication/boxc-authentication.yml
summary_line: oauth2/openIdConnect/http · 2 schemes
tags:
- Company
- Logistics
- Shipping
- Ecommerce
- Cross-Border
- Fulfillment
- Customs
- Tracking
- Webhooks
---
