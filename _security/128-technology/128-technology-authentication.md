---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: 128 Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: 128 Technology secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 128 Technology
provider_slug: 128-technology
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Every REST and GraphQL call carries an Authorization header of the form "Bearer <token>". The token is an RS256-signed JWT issued by the SSR itself and carries the caller's name, roles, scopes and capabilities as claims.
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - https://docs.128technology.com/docs/intro_rest_graphql_apis
  type: http
slug: 128-technology-authentication
source_filename: 128-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.128technology.com/docs/intro_rest_graphql_apis\ndocs: https://docs.128technology.com/docs/intro_rest_graphql_apis\nnote: >-\n  Derived from the provider's own published API documentation, not from an OpenAPI document.\n  128 Technology publishes no OpenAPI: the SSR serves an interactive Swagger reference from the\n  deployed instance itself (https://<SSR address>/documentation/swagger), reachable only from a\n  customer's own router or conductor, so no securityScheme block could be harvested.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  model: bearer-jwt-from-password-login\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  description: >-\n    Every REST and GraphQL call carries an Authorization header of the form\n    \"Bearer <token>\". The token is an RS256-signed JWT issued by the SSR itself and carries the\n\
  \    caller's name, roles, scopes and capabilities as claims.\n  sources:\n  - https://docs.128technology.com/docs/intro_rest_graphql_apis\ntoken_issuance:\n  operation: POST /api/v1/login\n  content_type: application/json\n  request_fields:\n  - username\n  - password\n  response_field: token\n  token_type: JWT (RS256)\n  docs: https://docs.128technology.com/docs/intro_rest_graphql_apis\n  note: >-\n    Credentials are the SSR local user account. There is no OAuth authorization server, no\n    client_id/client_secret exchange, and no refresh-token flow documented.\nauthorization:\n  model: RBAC\n  docs: https://docs.128technology.com/docs/config_RBAC\n  description: >-\n    Access Management Roles carry capabilities and are bound to Resource Groups, which are in\n    turn assigned to Authority-level resources (routers, tenants, services, service-policies).\n    The RBAC privileges of the authenticated user determine which resources an API call can\n    reach; a role may additionally exclude\
  \ named resources, which are then hidden from that\n    user's view entirely.\n  capabilities:\n  - name: config-read\n    description: Read the configuration tree.\n  - name: config-write\n    description: Modify and commit configuration.\n  - name: provisioning\n    description: >-\n      Software lifecycle management — download software, upgrade existing installations.\n  built_in_roles:\n  - name: admin\n    description: Default administrator role; has access to all configuration options and cannot be removed.\n  jwt_claims_observed:\n  - name\n  - roles\n  - scopes\n  - capabilities\n  - application\n  - userAgent\n  - iss\n  - iat\n  jwt_claim_note: >-\n    Claim names read from the example decoded token published in the REST/GraphQL API\n    documentation; scopes observed there were \"configure\" and \"show-commands\", capabilities\n    \"config-read\", \"config-write\" and \"provisioning\". No published scope reference page exists,\n    so scopes/ was not written.\nother_interfaces:\n\
  - interface: NETCONF\n  auth: SSH transport (password or public-key), per RFC 6242\n  note: The SSR also exposes its YANG data model over NETCONF alongside REST and GraphQL.\n- interface: SSH / PCLI\n  auth: Local username+password or public-key authentication using keys in the local filesystem\n  source: https://docs.128technology.com/docs/cc_fips_intro\ntransport_note: >-\n  The documented curl examples pass -k (skip TLS verification) because a factory SSR presents a\n  self-signed webserver certificate; the SSR supports replacing it with a CA-signed certificate\n  (see https://docs.128technology.com/docs/config_webserver_certs).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/128-technology/refs/heads/main/authentication/128-technology-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Networking
- SD-WAN
- Routing
- Network Management
- Session Smart Networking
- NETCONF
- YANG
- Telecommunications
- Infrastructure
---
