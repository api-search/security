---
anonymous_access: false
api_key_in: []
api_specs:
- filename: geckovision-tech-case-studies-api-openapi.yml
  format: yaml
  label: Gecko Case Studies API
  slug: geckovision-tech-case-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geckovision-tech/openapi/geckovision-tech-case-studies-api-openapi.yml
- filename: geckovision-tech-waitlist-api-openapi.yml
  format: yaml
  label: Gecko Waitlist API
  slug: geckovision-tech-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geckovision-tech/openapi/geckovision-tech-waitlist-api-openapi.yml
auth_types: []
description: Authentication schemes as described on the Gecko documentation pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Gecko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gecko declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Gecko
provider_slug: geckovision-tech
scheme_count: 3
schemes:
- evidence: 'Authorization: Bearer <session JWT> (httpAuth)'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'X-Api-Token: <long-lived apiToken> (apiKeyAuth)'
  header: X-Api-Token
  location: header
  name: X-Api-Token
  type: apiKey
- evidence: 'session.auth_headers() # a valid Bearer token — refreshed transparently as it nears expiry'
  header: Authorization
  location: header
  name: OAuth2
  type: oauth2
slug: geckovision-tech-authentication
source_filename: geckovision-tech-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.geckovision.tech/access-and-auth
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.geckovision.tech/access-and-auth\nsources:\n- https://docs.geckovision.tech/access-and-auth\n- https://docs.geckovision.tech/quickstart\ndescription: Authentication schemes as described on the Gecko documentation pages.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer <session JWT> (httpAuth)'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: X-Api-Token\n  evidence: 'X-Api-Token: <long-lived apiToken> (apiKeyAuth)'\n  location: header\n  header: X-Api-Token\n- type: oauth2\n  name: OAuth2\n  evidence: 'session.auth_headers() # a valid Bearer token — refreshed transparently as it nears expiry'\n  location: header\n  header: Authorization\ndocs: https://docs.geckovision.tech/access-and-auth\n"
source_yaml_url: https://artifacts.apis.io/geckovision-tech/authentication/geckovision-tech-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Data
- Agents
- Platform
- MCP
---
