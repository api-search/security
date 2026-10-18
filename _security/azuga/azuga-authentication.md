---
anonymous_access: false
api_key_in: []
api_specs:
- filename: azuga-azuga-ws-oauth-api-openapi.yml
  format: yaml
  label: Azuga Azuga Ws Oauth API
  slug: azuga-azuga-ws-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuga/refs/heads/main/openapi/azuga-azuga-ws-oauth-api-openapi.yml
auth_types: []
description: Azuga APIs use JWT access tokens obtained from the authentication API and sent in the Authorization header as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Azuga Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azuga declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Azuga
provider_slug: azuga
scheme_count: 1
schemes:
- evidence: Once the token is obtained, it needs to be added to the header of every request by prefixing the word "Bearer" before the token.
  header: Authorization
  how_to_obtain: Make a request to the Azuga authentication API using the user's credentials to receive a JWT access token.
  location: header
  name: Bearer
  type: http-bearer
slug: azuga-authentication
source_filename: azuga-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.azuga.com/reference/authentication-workflow.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.azuga.com/reference/authentication-workflow.md\nsources:\n- https://developer.azuga.com/reference/authentication-workflow.md\n- https://developer.azuga.com/changelog/api-authentication-upgrade-to-oauth-20.md\n- https://developer.azuga.com/changelog/authentication-on-v4.md\n- https://developer.azuga.com/reference/authentication-workflow\ndescription: Azuga APIs use JWT access tokens obtained from the authentication API and sent in the Authorization header as a Bearer token.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Once the token is obtained, it needs to be added to the header of every request by prefixing the word \"Bearer\" before the token.\n  location: header\n  header: Authorization\n  how_to_obtain: Make a request to the Azuga authentication API using the user's credentials to receive a JWT access token.\ndocs: https://developer.azuga.com/reference/authentication-workflow.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azuga/refs/heads/main/authentication/azuga-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fleet Management
- GPS Tracking
- Telematics
- Software-as-a-Service
---
