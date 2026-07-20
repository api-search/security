---
api_key_in: []
api_specs:
- filename: finix-openapi-original.yml
  format: yaml
  label: Finix API
  slug: finix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Finix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Finix
provider_slug: finix
scheme_count: 1
schemes:
- header: 'Authorization: Basic <Base64(username:password)>'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/finix-openapi-original.yml
  type: http
slug: finix-authentication
source_filename: finix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/finix-openapi-original.yml\ndocs: https://docs.finix.com/additional-resources/developers/authentication-and-api-basics/api-keys\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  standard: RFC 7617 HTTP Basic Authentication\n  key_model: API key ID (username) + API key secret (password), Base64-encoded in the Authorization header\n  environment_separation: Sandbox keys and Live keys are not interchangeable; each is issued from its own dashboard\nroles:\n- name: ROLE_PLATFORM\n  description: Highest access. Access all Applications and Merchant data, create Applications and Merchants, and assign roles.\n- name: ROLE_PARTNER\n  description: Access to one Application and its Merchant data.\n- name: ROLE_MERCHANT\n  description: Access to a single Merchant and its data.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  header: 'Authorization: Basic <Base64(username:password)>'\n  sources:\n  - openapi/finix-openapi-original.yml\n\
  notes:\n- Combine the API key username and password with a colon and Base64-encode, per RFC 7617.\n- The optional finix-apiuser-role header can scope a request to a specific role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/authentication/finix-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Payment Processing
- Payment Facilitation
- Merchant Onboarding
- Payouts
- Marketplaces
---
