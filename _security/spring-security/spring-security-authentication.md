---
api_key_in: []
api_specs:
- filename: spring-security-authorization-api-openapi.yml
  format: yaml
  label: Spring Security Authorization API
  slug: spring-security-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-authorization-api-openapi.yml
- filename: spring-security-client-management-api-openapi.yml
  format: yaml
  label: Spring Security Client Management API
  slug: spring-security-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-client-management-api-openapi.yml
- filename: spring-security-device-api-openapi.yml
  format: yaml
  label: Spring Security Device API
  slug: spring-security-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-device-api-openapi.yml
- filename: spring-security-discovery-api-openapi.yml
  format: yaml
  label: Spring Security Discovery API
  slug: spring-security-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-discovery-api-openapi.yml
- filename: spring-security-keys-api-openapi.yml
  format: yaml
  label: Spring Security Keys API
  slug: spring-security-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-keys-api-openapi.yml
- filename: spring-security-openid-connect-api-openapi.yml
  format: yaml
  label: Spring Security OpenID Connect API
  slug: spring-security-openid-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-openid-connect-api-openapi.yml
- filename: spring-security-session-api-openapi.yml
  format: yaml
  label: Spring Security Session API
  slug: spring-security-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-session-api-openapi.yml
- filename: spring-security-token-api-openapi.yml
  format: yaml
  label: Spring Security Token API
  slug: spring-security-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-token-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spring Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spring Security secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spring Security
provider_slug: spring-security
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/spring-authorization-server-openapi.yml
  - openapi/spring-security-oauth2-openapi.yml
  type: http
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/spring-authorization-server-openapi.yml
  - openapi/spring-security-oauth2-openapi.yml
  type: http
slug: spring-security-authentication
source_filename: spring-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spring-authorization-server-openapi.yml, openapi/spring-security-oauth2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/spring-authorization-server-openapi.yml\n  - openapi/spring-security-oauth2-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/spring-authorization-server-openapi.yml\n  - openapi/spring-security-oauth2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/authentication/spring-security-authentication.yml
summary_line: http · 2 schemes
tags:
- Authentication
- Authorization
- Java
- JWT
- OpenID Connect
- SAML
- Security
- Spring Framework
---
