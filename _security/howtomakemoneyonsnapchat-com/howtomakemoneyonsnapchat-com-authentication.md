---
anonymous_access: false
api_key_in: []
api_specs:
- filename: howtomakemoneyonsnapchat-com-calculations-api-openapi.yml
  format: yaml
  label: howtomakemoneyonsnapchat-com Calculations API
  slug: howtomakemoneyonsnapchat-com-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/howtomakemoneyonsnapchat-com/openapi/howtomakemoneyonsnapchat-com-calculations-api-openapi.yml
- filename: howtomakemoneyonsnapchat-com-facts-api-openapi.yml
  format: yaml
  label: howtomakemoneyonsnapchat-com Facts API
  slug: howtomakemoneyonsnapchat-com-facts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/howtomakemoneyonsnapchat-com/openapi/howtomakemoneyonsnapchat-com-facts-api-openapi.yml
- filename: howtomakemoneyonsnapchat-com-meta-api-openapi.yml
  format: yaml
  label: howtomakemoneyonsnapchat-com Meta API
  slug: howtomakemoneyonsnapchat-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/howtomakemoneyonsnapchat-com/openapi/howtomakemoneyonsnapchat-com-meta-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Howtomakemoneyonsnapchat Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: howtomakemoneyonsnapchat-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: howtomakemoneyonsnapchat-com
provider_slug: howtomakemoneyonsnapchat-com
scheme_count: 2
schemes:
- description: Optional for get_monetization_requirements and get_rule_changes. Required for calculation, payout, and Watch tools.
  scheme: bearer
  type: http
- description: Optional for the two fact tools. Required for calculation, payout, and Watch tools.
  in: header
  name: X-API-Key
  type: apiKey
slug: howtomakemoneyonsnapchat-com-authentication
source_filename: howtomakemoneyonsnapchat-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://howtomakemoneyonsnapchat.com/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    description: Optional for get_monetization_requirements and get_rule_changes. Required for calculation, payout, and Watch tools.\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: Optional for the two fact tools. Required for calculation, payout, and Watch tools.\n"
source_yaml_url: https://artifacts.apis.io/howtomakemoneyonsnapchat-com/authentication/howtomakemoneyonsnapchat-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Snapchat
- Monetization
- Calculator
- Rules
---
