---
anonymous_access: false
api_key_in: []
api_specs:
- filename: velocitycard-openapi-generated.yml
  format: yaml
  label: VelocityCard Card Issuing API
  slug: velocitycard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/velocitycard/openapi/_ae-authored/velocitycard-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: VelocityCard Authentication
name_suffix: Authentication
oauth_flows: []
overview: VelocityCard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: VelocityCard
provider_slug: velocitycard
scheme_count: 1
schemes:
- description: Authenticate with a Bearer token in the Authorization header. Keep your key secret and never put it in browser or mobile code.
  format: 'Authorization: Bearer your-api-key'
  header: Authorization
  name: bearerAuth
  obtain: Your base URL and API key are provided together during onboarding.
  scheme: bearer
  type: http
slug: velocitycard-authentication
source_filename: velocitycard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: VelocityCard authentication\ngenerated: '2026-11-19'\nmethod: searched\nsource: https://www.velocitycard.io/card-issuing-api\ndocs: https://www.velocitycard.io/card-issuing-api\nschemes:\n- type: http\n  scheme: bearer\n  name: bearerAuth\n  header: Authorization\n  format: 'Authorization: Bearer your-api-key'\n  description: Authenticate with a Bearer token in the Authorization header. Keep\n    your key secret and never put it in browser or mobile code.\n  obtain: Your base URL and API key are provided together during onboarding.\n"
source_yaml_url: https://artifacts.apis.io/velocitycard/authentication/velocitycard-authentication.yml
summary_line: 1 scheme
tags:
- Card Issuing
- Banking as a Service
- Embedded Finance
- Commercial Cards
- Payments
- Expense Management
---
