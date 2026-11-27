---
anonymous_access: false
api_key_in: []
api_specs:
- filename: duck-hub-com-integrationspublic-api-openapi.yml
  format: yaml
  label: Duckhub Integrations Public API
  slug: duck-hub-com-integrationspublic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duck-hub-com/openapi/duck-hub-com-integrationspublic-api-openapi.yml
- filename: duck-hub-com-open-api-api-openapi.yml
  format: yaml
  label: Duckhub Open API
  slug: duck-hub-com-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duck-hub-com/openapi/duck-hub-com-open-api-api-openapi.yml
auth_types: []
description: Authentication schemes for DuckHub API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Duckhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duckhub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Duckhub
provider_slug: duck-hub-com
scheme_count: 1
schemes:
- evidence: 'Every API request is authenticated with an API key sent as a Bearer token: http Authorization : Bearer dk_live_your_api_key'
  header: Authorization
  how_to_obtain: Generated in the DuckHub app under Integrations → Generate API key (or Regenerate/Revoke). The full key is shown only once after generation.
  location: header
  name: Authorization
  type: http-bearer
slug: duck-hub-com-authentication
source_filename: duck-hub-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.duck-hub.com/authentication
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.duck-hub.com/authentication\nsources:\n- https://docs.duck-hub.com/authentication\n- https://docs.duck-hub.com/authentication\n- https://docs.duck-hub.com/connect\ndescription: Authentication schemes for DuckHub API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Every API request is authenticated with an API key sent as a Bearer token: http Authorization : Bearer dk_live_your_api_key'\n  location: header\n  header: Authorization\n  how_to_obtain: Generated in the DuckHub app under Integrations → Generate API key (or Regenerate/Revoke). The full key is shown only once after\n    generation.\ndocs: https://docs.duck-hub.com/authentication\n"
source_yaml_url: https://artifacts.apis.io/duck-hub-com/authentication/duck-hub-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- QR
- Restaurant
- Software-as-a-Service
- Menus
- Company
---
