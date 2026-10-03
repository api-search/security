---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bold-penguin-api-openapi-generated.yml
  format: yaml
  label: Bold Penguin api API
  slug: api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-penguin/refs/heads/main/openapi/_ae-authored/bold-penguin-api-openapi-generated.yml
- filename: bold-penguin-core-openapi-generated.yml
  format: yaml
  label: Bold Penguin core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-penguin/refs/heads/main/openapi/_ae-authored/bold-penguin-core-openapi-generated.yml
- filename: bold-penguin-insurance_intelligence-openapi-generated.yml
  format: yaml
  label: Bold Penguin insurance_intelligence API
  slug: insurance_intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-penguin/refs/heads/main/openapi/_ae-authored/bold-penguin-insurance_intelligence-openapi-generated.yml
auth_types: []
description: Authentication methods for Bold Penguin APIs as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bold Penguin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bold Penguin declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bold Penguin
provider_slug: bold-penguin
scheme_count: 2
schemes:
- evidence: 'We can inject credentials into that request either via basic authentication or a static header ( X-API-KEY , Authorization: Bearer , etc.)'
  header: 'Authorization: Basic <base64_credentials>'
  how_to_obtain: Your Account Manager will provide you with a username and password for basic authentication.
  location: header
  name: Basic Authentication
  type: http-basic
- evidence: 'We can inject credentials into that request either via basic authentication or a static header ( X-API-KEY , Authorization: Bearer , etc.)'
  header: 'X-API-KEY: <api_key>'
  how_to_obtain: Your Account Manager will provide you with a unique bearer token (or API key) for each environment.
  location: header
  name: Static Header
  type: apiKey
slug: bold-penguin-authentication
source_filename: bold-penguin-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.boldpenguin.com/docs/terminal/quote_start/authentication
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.boldpenguin.com/docs/terminal/quote_start/authentication\nsources:\n- https://developers.boldpenguin.com/docs/terminal/quote_start/authentication\n- https://developers.boldpenguin.com/docs/exchange/send_side/ss_authentication\n- https://developers.boldpenguin.com/docs/exchange/receive_side/rs_authentication\n- https://developers.boldpenguin.com/docs/sdk/custom_storefront_tutorials/sdk_guest_auth\ndescription: Authentication methods for Bold Penguin APIs as documented.\nschemes:\n- type: http-basic\n  name: Basic Authentication\n  evidence: 'We can inject credentials into that request either via basic authentication or a static header ( X-API-KEY , Authorization: Bearer\n    , etc.)'\n  location: header\n  header: 'Authorization: Basic <base64_credentials>'\n  how_to_obtain: Your Account Manager will provide you with a username and password for basic authentication.\n\
  - type: apiKey\n  name: Static Header\n  evidence: 'We can inject credentials into that request either via basic authentication or a static header ( X-API-KEY , Authorization: Bearer\n    , etc.)'\n  location: header\n  header: 'X-API-KEY: <api_key>'\n  how_to_obtain: Your Account Manager will provide you with a unique bearer token (or API key) for each environment.\ndocs: https://developers.boldpenguin.com/docs/terminal/quote_start/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bold-penguin/refs/heads/main/authentication/bold-penguin-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Insurance
- API
- Platform
- Commercial
- AI
---
