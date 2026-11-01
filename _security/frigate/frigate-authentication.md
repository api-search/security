---
anonymous_access: false
api_key_in: []
api_specs:
- filename: frigate-openapi-generated.yml
  format: yaml
  label: Frigate NVR API
  slug: frigate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frigate/openapi/_ae-authored/frigate-openapi-generated.yml
auth_types: []
description: Authentication methods for Frigate NVR
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Frigate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frigate NVR declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Frigate NVR
provider_slug: frigate
scheme_count: 1
schemes:
- evidence: Upon successful login, a JWT token is issued with an expiration date and set as a cookie. The cookie is refreshed as needed automatically. This JWT token can also be passed in the Authorization header as a bearer token.
  header: Authorization
  how_to_obtain: Login endpoint returns a JWT token which is set as a cookie and can be used as a bearer token in the Authorization header.
  location: header
  name: Bearer
  type: http-bearer
slug: frigate-authentication
source_filename: frigate-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.frigate.video/configuration/authentication/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.frigate.video/configuration/authentication/\nsources:\n- https://docs.frigate.video/configuration/authentication/\ndescription: Authentication methods for Frigate NVR\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Upon successful login, a JWT token is issued with an expiration date and set as a cookie. The cookie is refreshed as needed automatically.\n    This JWT token can also be passed in the Authorization header as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Login endpoint returns a JWT token which is set as a cookie and can be used as a bearer token in the Authorization header.\nnote: Frigate does not implement OAuth2, API keys, or other authentication schemes directly; it relies on JWT tokens issued after login or via\n  upstream proxies.\ndocs: https://docs.frigate.video/configuration/authentication/\n"
source_yaml_url: https://artifacts.apis.io/frigate/authentication/frigate-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Video
- Surveillance
- OpenSource
- AI
---
