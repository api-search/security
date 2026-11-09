---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bike4mind-com-openapi.json
  format: json
  label: Bike4Mind API
  slug: bike4mind-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bike4mind-com/openapi/bike4mind-com-openapi.json
auth_types: []
description: Authentication methods for the B4M Completions API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bike4Mind Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bike4Mind declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bike4Mind
provider_slug: bike4mind-com
scheme_count: 2
schemes:
- evidence: Use an API key for production integrations and server-to-server communication.
  header: Authorization
  how_to_obtain: Open the Profile menu → More → API Keys → Click Create API Key → Configure name, scopes, rate limits → Click Create and copy the key (shown only once).
  location: header
  name: API Key
  scopes:
  - ai:generate
  - ai:chat
  type: apiKey
- evidence: Use JWT tokens for user-context requests where you need to authenticate on behalf of a specific user.
  header: Authorization
  how_to_obtain: Obtain a JWT from your authentication system after user login; the token is then sent as a Bearer token.
  location: header
  name: JWT Token
  type: http-bearer
slug: bike4mind-com-authentication
source_filename: bike4mind-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bike4mind.com/tags/authentication
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bike4mind.com/tags/authentication\nsources:\n- https://docs.bike4mind.com/tags/authentication\n- https://docs.bike4mind.com/tags/oauth\n- https://docs.bike4mind.com/api/completions/authentication\n- https://docs.bike4mind.com/features/slack-multi-workspace-oauth\ndescription: Authentication methods for the B4M Completions API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Use an API key for production integrations and server-to-server communication.\n  location: header\n  header: Authorization\n  scopes:\n  - ai:generate\n  - ai:chat\n  how_to_obtain: Open the Profile menu → More → API Keys → Click Create API Key → Configure name, scopes, rate limits → Click Create and copy\n    the key (shown only once).\n- type: http-bearer\n  name: JWT Token\n  evidence: Use JWT tokens for user-context requests where you need to authenticate on behalf of a specific user.\n\
  \  location: header\n  header: Authorization\n  how_to_obtain: Obtain a JWT from your authentication system after user login; the token is then sent as a Bearer token.\ndocs: https://docs.bike4mind.com/tags/authentication\n"
source_yaml_url: https://artifacts.apis.io/bike4mind-com/authentication/bike4mind-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Open Source
- Platform
- Workbench
---
