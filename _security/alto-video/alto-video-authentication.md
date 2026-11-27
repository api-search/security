---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alto-video-openapi-generated.yml
  format: yaml
  label: Alto API
  slug: alto-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alto-video/openapi/_ae-authored/alto-video-openapi-generated.yml
auth_types: []
description: Authentication methods described on the page
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Alto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alto declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Alto
provider_slug: alto-video
scheme_count: 2
schemes:
- evidence: It speaks MCP’s Streamable HTTP transport and signs the agent in with the key as a bearer token.
  header: Authorization
  how_to_obtain: Create a key in Settings › API & agents; the key is shown once and starts with alto_
  location: header
  name: API Key
  type: http-bearer
- evidence: 'The CLI The alto command does the same from a terminal: alto login prints a link, you approve it in the browser, and every later command on that machine is signed in.'
  flows:
  - authorization_code
  how_to_obtain: Run `alto login`, open the printed link in a browser and approve the request
  name: Alto OAuth
  type: oauth2
slug: alto-video-authentication
source_filename: alto-video-authentication.yml
source_heading: Authentication Profile
source_url: https://alto.video/docs/cli-and-mcp
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://alto.video/docs/cli-and-mcp\nsources:\n- https://alto.video/docs/cli-and-mcp\ndescription: Authentication methods described on the page\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: It speaks MCP’s Streamable HTTP transport and signs the agent in with the key as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings › API & agents; the key is shown once and starts with alto_\n- type: oauth2\n  name: Alto OAuth\n  evidence: 'The CLI The alto command does the same from a terminal: alto login prints a link, you approve it in the browser, and every later\n    command on that machine is signed in.'\n  flows:\n  - authorization_code\n  how_to_obtain: Run `alto login`, open the printed link in a browser and approve the request\ndocs: https://alto.video/docs/cli-and-mcp\n"
source_yaml_url: https://artifacts.apis.io/alto-video/authentication/alto-video-authentication.yml
summary_line: 2 schemes
tags:
- Video Hosting
- Sales Enablement
- Demo Analytics
- Privacy
- Software-as-a-Service
---
