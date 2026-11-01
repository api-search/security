---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aqara-automation-api-openapi.yml
  format: yaml
  label: Aqara Automation API
  slug: aqara-automation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-automation-api-openapi.yml
- filename: aqara-device-api-openapi.yml
  format: yaml
  label: Aqara Device API
  slug: aqara-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-device-api-openapi.yml
- filename: aqara-gateway-api-openapi.yml
  format: yaml
  label: Aqara Gateway API
  slug: aqara-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-gateway-api-openapi.yml
- filename: aqara-space-api-openapi.yml
  format: yaml
  label: Aqara Space API
  slug: aqara-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-space-api-openapi.yml
- filename: aqara-studio-api-openapi.yml
  format: yaml
  label: Aqara Studio API
  slug: aqara-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-studio-api-openapi.yml
auth_types: []
description: Authentication for Aqara Studio API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aqara Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aqara declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aqara
provider_slug: aqara
scheme_count: 1
schemes:
- evidence: When calling the Aqara Studio API, you must include the Authorization header in the request headers. Set the Authorization header to Bearer <token> , where <token> is the access token you obtained from Aqara Studio.
  header: Authorization
  how_to_obtain: Obtain an access token from Aqara Studio as described in the Developer Guide – Obtain Token.
  location: header
  name: Bearer token
  type: http-bearer
slug: aqara-authentication
source_filename: aqara-authentication.yml
source_heading: Authentication Profile
source_url: http://docs.aqara.com/docs/aqara-studio/overview/introduction/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: http://docs.aqara.com/docs/aqara-studio/overview/introduction/\nsources:\n- http://docs.aqara.com/docs/aqara-studio/overview/introduction/\n- http://docs.aqara.com/docs/aqara-developer/data-export-api/getting-started-with-the-data-export-api/\ndescription: Authentication for Aqara Studio API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: When calling the Aqara Studio API, you must include the Authorization header in the request headers. Set the Authorization header\n    to Bearer <token> , where <token> is the access token you obtained from Aqara Studio.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an access token from Aqara Studio as described in the Developer Guide – Obtain Token.\ndocs: http://docs.aqara.com/docs/aqara-studio/overview/introduction/\n"
source_yaml_url: https://artifacts.apis.io/aqara/authentication/aqara-authentication.yml
summary_line: 1 scheme
tags:
- Smart Home
- IoT
- Consumer Electronics
- Home Automation
- Security
---
