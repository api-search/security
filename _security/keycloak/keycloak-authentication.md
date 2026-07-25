---
api_key_in: []
api_specs:
- filename: keycloak-clients-api-openapi.yml
  format: yaml
  label: Keycloak Clients API
  slug: keycloak-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/openapi/keycloak-clients-api-openapi.yml
- filename: keycloak-groups-api-openapi.yml
  format: yaml
  label: Keycloak Groups API
  slug: keycloak-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/openapi/keycloak-groups-api-openapi.yml
- filename: keycloak-identity-providers-api-openapi.yml
  format: yaml
  label: Keycloak Identity Providers API
  slug: keycloak-identity-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/openapi/keycloak-identity-providers-api-openapi.yml
- filename: keycloak-realms-api-openapi.yml
  format: yaml
  label: Keycloak Realms API
  slug: keycloak-realms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/openapi/keycloak-realms-api-openapi.yml
- filename: keycloak-roles-api-openapi.yml
  format: yaml
  label: Keycloak Roles API
  slug: keycloak-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/openapi/keycloak-roles-api-openapi.yml
- filename: keycloak-users-api-openapi.yml
  format: yaml
  label: Keycloak Users API
  slug: keycloak-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycloak/refs/heads/main/openapi/keycloak-users-api-openapi.yml
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
source_yaml: "generated: '2026-07-16'\nmethod: derived\nsource: openapi/keycloak-admin-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Access token obtained from the Keycloak token endpoint. Use the master realm\n    admin credentials or a service account with appropriate realm-management roles.\n  sources:\n  - openapi/keycloak-admin-rest-api-openapi.yml\n"
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
