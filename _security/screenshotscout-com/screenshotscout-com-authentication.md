---
anonymous_access: false
api_key_in: []
api_specs:
- filename: screenshotscout-com-openapi-generated.yml
  format: yaml
  label: screenshotscout-com API
  slug: screenshotscout-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/screenshotscout-com/openapi/_ae-authored/screenshotscout-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Screenshotscout Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: screenshotscout-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: screenshotscout-com
provider_slug: screenshotscout-com
scheme_count: 2
schemes:
- description: Your public access key provided on the API Keys page. Required for all requests.
  in: query
  name: access_key
  type: apiKey
- description: HMAC signature computed from request parameters and your secret key. Optional unless you enable signed requests for the API key.
  in: query
  name: signature
  type: apiKey
slug: screenshotscout-com-authentication
source_filename: screenshotscout-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://screenshotscout.com/docs/signed-requests\nschemes:\n  - type: apiKey\n    name: access_key\n    in: query\n    description: \"Your public access key provided on the API Keys page. Required for all requests.\"\n  - type: apiKey\n    name: signature\n    in: query\n    description: \"HMAC signature computed from request parameters and your secret key. Optional unless you enable signed requests for the API key.\"\n"
source_yaml_url: https://artifacts.apis.io/screenshotscout-com/authentication/screenshotscout-com-authentication.yml
summary_line: 2 schemes
tags:
- Screenshots
- API
- WebAutomation
- DeveloperTools
- SaaS
---
