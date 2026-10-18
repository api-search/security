---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fort-robotics-openapi-generated.yml
  format: yaml
  label: Fort Robotics API
  slug: fort-robotics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fort-robotics/refs/heads/main/openapi/_ae-authored/fort-robotics-openapi-generated.yml
auth_types: []
description: Authentication for the Fort Robotics API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fort Robotics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fort Robotics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fort Robotics
provider_slug: fort-robotics
scheme_count: 1
schemes:
- evidence: To authenticate your requests, include the API key in the Authorization header of your HTTP request, prefixed with Bearer.
  header: Authorization
  how_to_obtain: Generate an API key from the FORT Manager web application (API Key Management page).
  location: header
  name: Authorization
  type: apiKey
slug: fort-robotics-authentication
source_filename: fort-robotics-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.fortrobotics.com/getting_started
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.fortrobotics.com/getting_started\nsources:\n- https://developer.fortrobotics.com/getting_started\ndescription: Authentication for the Fort Robotics API\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: To authenticate your requests, include the API key in the Authorization header of your HTTP request, prefixed with Bearer.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key from the FORT Manager web application (API Key Management page).\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented on the page.\ndocs: https://developer.fortrobotics.com/getting_started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fort-robotics/refs/heads/main/authentication/fort-robotics-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Robotics
- Artificial Intelligence
- Safety
- Platform
---
