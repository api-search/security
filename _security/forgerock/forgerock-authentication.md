---
api_key_in:
- header
api_specs:
- filename: forgerock-identity-cloud-openapi.yml
  format: yaml
  label: ForgeRock Identity Cloud REST API
  slug: forgerock-identity-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-identity-cloud-openapi.yml
- filename: forgerock-access-management-openapi.yml
  format: yaml
  label: ForgeRock Access Management API
  slug: forgerock-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-access-management-openapi.yml
- filename: forgerock-identity-management-openapi.yml
  format: yaml
  label: ForgeRock Identity Management API
  slug: forgerock-identity-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-identity-management-openapi.yml
- filename: forgerock-identity-gateway-openapi.yml
  format: yaml
  label: ForgeRock Identity Gateway API
  slug: forgerock-identity-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-identity-gateway-openapi.yml
- filename: forgerock-directory-services-openapi.yml
  format: yaml
  label: ForgeRock Directory Services API
  slug: forgerock-directory-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-directory-services-openapi.yml
- filename: forgerock-identity-governance-openapi.yml
  format: yaml
  label: ForgeRock Identity Governance API
  slug: forgerock-identity-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-identity-governance-openapi.yml
- filename: forgerock-autonomous-identity-openapi.yml
  format: yaml
  label: ForgeRock Autonomous Identity API
  slug: forgerock-autonomous-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-autonomous-identity-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Forgerock Authentication
name_suffix: Authentication
oauth_flows: []
overview: ForgeRock secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ForgeRock
provider_slug: forgerock
scheme_count: 4
schemes:
- description: AM SSO token obtained from authentication
  in: header
  name: ssoToken
  parameter: iPlanetDirectoryPro
  sources:
  - openapi/forgerock-access-management-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/forgerock-access-management-openapi.yml
  - openapi/forgerock-autonomous-identity-openapi.yml
  - openapi/forgerock-directory-services-openapi.yml
  - openapi/forgerock-identity-cloud-openapi.yml
  - openapi/forgerock-identity-gateway-openapi.yml
  - openapi/forgerock-identity-governance-openapi.yml
  - openapi/forgerock-identity-management-openapi.yml
  type: http
- description: HTTP Basic authentication (for directory bind)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/forgerock-directory-services-openapi.yml
  - openapi/forgerock-identity-management-openapi.yml
  type: http
- description: API key for tenant read-only operations. Used together with x-api-secret header.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/forgerock-identity-cloud-openapi.yml
  type: apiKey
slug: forgerock-authentication
source_filename: forgerock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/forgerock-access-management-openapi.yml, openapi/forgerock-autonomous-identity-openapi.yml,\n  openapi/forgerock-directory-services-openapi.yml, openapi/forgerock-identity-cloud-openapi.yml,\n  openapi/forgerock-identity-gateway-openapi.yml, openapi/forgerock-identity-governance-openapi.yml,\n  openapi/forgerock-identity-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ssoToken\n  type: apiKey\n  in: header\n  parameter: iPlanetDirectoryPro\n  description: AM SSO token obtained from authentication\n  sources:\n  - openapi/forgerock-access-management-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token\n  sources:\n  - openapi/forgerock-access-management-openapi.yml\n  - openapi/forgerock-autonomous-identity-openapi.yml\n  - openapi/forgerock-directory-services-openapi.yml\n  - openapi/forgerock-identity-cloud-openapi.yml\n\
  \  - openapi/forgerock-identity-gateway-openapi.yml\n  - openapi/forgerock-identity-governance-openapi.yml\n  - openapi/forgerock-identity-management-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication (for directory bind)\n  sources:\n  - openapi/forgerock-directory-services-openapi.yml\n  - openapi/forgerock-identity-management-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for tenant read-only operations. Used together with x-api-secret header.\n  sources:\n  - openapi/forgerock-identity-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/authentication/forgerock-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
---
