---
anonymous_access: false
api_key_in: []
api_specs:
- filename: monkedo-openapi-generated.yml
  format: yaml
  label: Z Yazilim API
  slug: monkedo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monkedo/openapi/_ae-authored/monkedo-openapi-generated.yml
auth_types: []
description: Authentication schemes for Monkedo API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Monkedo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Z Yazilim declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Z Yazilim
provider_slug: monkedo
scheme_count: 1
schemes:
- evidence: 'Every request requires a valid API key in the Authorization header: Authorization : Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Create API key in the Monkedo dashboard (Keys page) and copy the secret token.
  location: header
  name: API Key
  type: http-bearer
slug: monkedo-authentication
source_filename: monkedo-authentication.yml
source_heading: Authentication Profile
source_url: https://monkedo.com/docs/api-keys/introduction
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://monkedo.com/docs/api-keys/introduction\nsources:\n- https://monkedo.com/docs/api-keys/introduction\n- https://monkedo.com/docs/api-keys/structure\n- https://monkedo.com/docs/api-keys/api\ndescription: Authentication schemes for Monkedo API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Every request requires a valid API key in the Authorization header: Authorization : Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create API key in the Monkedo dashboard (Keys page) and copy the secret token.\nnote: No OAuth2, apiKey, or other authentication methods are documented.\ndocs: https://monkedo.com/docs/api-keys/introduction\n"
source_yaml_url: https://artifacts.apis.io/monkedo/authentication/monkedo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Automation
- No-Code
- Integration
- Workflow
---
