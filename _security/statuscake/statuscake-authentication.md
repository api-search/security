---
anonymous_access: false
api_key_in: []
api_specs:
- filename: statuscake-openapi-generated.yml
  format: yaml
  label: StatusCake API
  slug: statuscake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/statuscake/openapi/_ae-authored/statuscake-openapi-generated.yml
auth_types: []
description: Authentication schemes for StatusCake API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: StatusCake Authentication
name_suffix: Authentication
oauth_flows: []
overview: StatusCake declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: StatusCake
provider_slug: statuscake
scheme_count: 1
schemes:
- evidence: The StatusCake API uses a bearer authentication (also called token authentication) HTTP authentication scheme that involves security tokens called bearer tokens.
  header: Authorization
  how_to_obtain: View and manage your API tokens from the StatusCake account panel.
  location: header
  name: Bearer
  type: http-bearer
slug: statuscake-authentication
source_filename: statuscake-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.statuscake.com/guides/api/authentication/
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.statuscake.com/guides/api/authentication/\nsources:\n- https://developers.statuscake.com/guides/api/authentication/\n- https://developers.statuscake.com/guides/sdks/quickstart/\ndescription: Authentication schemes for StatusCake API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: The StatusCake API uses a bearer authentication (also called token authentication) HTTP authentication scheme that involves security\n    tokens called bearer tokens.\n  location: header\n  header: Authorization\n  how_to_obtain: View and manage your API tokens from the StatusCake account panel.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://developers.statuscake.com/guides/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/statuscake/authentication/statuscake-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Monitoring
- Uptime
- Performance
---
