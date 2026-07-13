---
api_key_in: []
api_specs:
- filename: keycloak-admin-rest-api-openapi.yml
  format: yaml
  label: Keycloak Admin REST API
  slug: admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/openapi/keycloak-admin-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Keycloak Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keycloak secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Keycloak
provider_slug: keycloak
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Access token obtained from the Keycloak token endpoint. Use the master realm admin credentials or a service account with appropriate realm-management roles.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/keycloak-admin-rest-api-openapi.yml
  type: http
slug: keycloak-authentication
source_filename: keycloak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keycloak-admin-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Access token obtained from the Keycloak token endpoint. Use the master realm\n    admin credentials or a service account with appropriate realm-management roles.\n  sources:\n  - openapi/keycloak-admin-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/authentication/keycloak-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Authorization
- Identity Management
- OAuth
- OpenID Connect
- Security
- SSO
---
