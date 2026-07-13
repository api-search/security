---
api_key_in: []
api_specs:
- filename: spring-security-oauth2-openapi.yml
  format: yaml
  label: Spring Security OAuth2 API
  slug: spring-security-oauth2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-oauth2-openapi.yml
- filename: spring-authorization-server-openapi.yml
  format: yaml
  label: Spring Authorization Server API
  slug: spring-authorization-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-authorization-server-openapi.yml
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
- OAuth2
- OpenID Connect
- SAML
- Security
- Spring Framework
---
