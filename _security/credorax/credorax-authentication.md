---
anonymous_access: false
api_key_in: []
api_specs:
- filename: credorax-charges-api-openapi.yml
  format: yaml
  label: Credorax Charges API
  slug: credorax-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credorax/refs/heads/main/openapi/credorax-charges-api-openapi.yml
- filename: credorax-customers-api-openapi.yml
  format: yaml
  label: Credorax Customers API
  slug: credorax-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credorax/refs/heads/main/openapi/credorax-customers-api-openapi.yml
- filename: credorax-events-api-openapi.yml
  format: yaml
  label: Credorax Events API
  slug: credorax-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credorax/refs/heads/main/openapi/credorax-events-api-openapi.yml
- filename: credorax-plans-api-openapi.yml
  format: yaml
  label: Credorax Plans API
  slug: credorax-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credorax/refs/heads/main/openapi/credorax-plans-api-openapi.yml
- filename: credorax-tokens-api-openapi.yml
  format: yaml
  label: Credorax Tokens API
  slug: credorax-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credorax/refs/heads/main/openapi/credorax-tokens-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Credorax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credorax declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Credorax
provider_slug: credorax
scheme_count: 1
schemes:
- evidence: The Shift4 API uses HTTP Basic Authentication. Provide your API secret key as the username and leave the password empty.
  header: Authorization
  location: header
  name: basic
  type: http-basic
slug: credorax-authentication
source_filename: credorax-authentication.yml
source_heading: Authentication Profile
source_url: https://dev.shift4.com/docs/api/shift4-gateway/section/authentication
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dev.shift4.com/docs/api/shift4-gateway/section/authentication\nsources:\n- https://dev.shift4.com/docs/api/shift4-gateway/section/authentication\n- https://help.shift4.com/Transaction_Manager/Use_and_Operation/Enable_Multi_Factor_Authentication_for_Standard_Users\n- https://dev.shift4.com/docs/api/shift4-gateway/tokens\ndescription: Authentication\nschemes:\n- type: http-basic\n  name: basic\n  evidence: The Shift4 API uses HTTP Basic Authentication. Provide your API secret key as the username and leave the password empty.\n  location: header\n  header: Authorization\ndocs: https://dev.shift4.com/docs/api/shift4-gateway/section/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credorax/refs/heads/main/authentication/credorax-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
