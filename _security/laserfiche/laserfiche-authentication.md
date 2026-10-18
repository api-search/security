---
anonymous_access: false
api_key_in: []
api_specs:
- filename: laserfiche-oauth-api-openapi.yml
  format: yaml
  label: Laserfiche OAuth API
  slug: laserfiche-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/laserfiche-oauth-api-openapi.yml
- filename: laserfiche-odata4-api-openapi.yml
  format: yaml
  label: Laserfiche Odata4 API
  slug: laserfiche-odata4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/laserfiche-odata4-api-openapi.yml
- filename: laserfiche-repositories-api-openapi.yml
  format: yaml
  label: Laserfiche Repositories API
  slug: laserfiche-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/laserfiche-repositories-api-openapi.yml
- filename: laserfiche-repository-api-openapi.yml
  format: yaml
  label: Laserfiche Repository API
  slug: laserfiche-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/laserfiche-repository-api-openapi.yml
auth_types: []
description: Laserfiche APIs use OAuth 2.0 bearer tokens or Basic authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Laserfiche Authentication
name_suffix: Authentication
oauth_flows: []
overview: Laserfiche declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Laserfiche
provider_slug: laserfiche
scheme_count: 1
schemes:
- evidence: If you have a username and password, find the Basic Authentication (http) option. Enter the username and password values you received in step 1. Click Authorize. This will automatically add the Authorization header to your requests.
  header: Authorization
  location: header
  name: Basic Authentication
  type: http-basic
slug: laserfiche-authentication
source_filename: laserfiche-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.laserfiche.com/docs/api/authentication/
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.laserfiche.com/docs/api/authentication/\nsources:\n- https://developer.laserfiche.com/docs/api/authentication/\n- https://developer.laserfiche.com/docs/api/authentication/guide_authenticating-to-the-swagger-playground/\n- https://developer.laserfiche.com/docs/api/authentication/guide_service-principals/\n- https://developer.laserfiche.com/docs/api/authentication/guide_oauth-service/\ndescription: Laserfiche APIs use OAuth 2.0 bearer tokens or Basic authentication.\nschemes:\n- type: http-basic\n  name: Basic Authentication\n  evidence: If you have a username and password, find the Basic Authentication (http) option. Enter the username and password values you received\n    in step 1. Click Authorize. This will automatically add the Authorization header to your requests.\n  location: header\n  header: Authorization\ndocs: https://developer.laserfiche.com/docs/api/authentication/\n\
  note: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/authentication/laserfiche-authentication.yml
summary_line: 1 scheme
tags:
- Company
- EnterpriseContentManagement
- Document Management
- ProcessAutomation
- Artificial Intelligence
---
