---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses an API key sent in the request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Matchwire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Matchwire declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Matchwire
provider_slug: matchwire-win
scheme_count: 1
schemes:
- evidence: You get a key when you start a plan. Send it on every call as the x-api-key header.
  header: x-api-key
  how_to_obtain: Get a key when you start a plan.
  location: header
  name: API Key
  type: apiKey
slug: matchwire-win-authentication
source_filename: matchwire-win-authentication.yml
source_heading: Authentication Profile
source_url: https://matchwire.win/docs/
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://matchwire.win/docs/\nsources:\n- https://matchwire.win/docs/\ndescription: Authentication uses an API key sent in the request header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: You get a key when you start a plan. Send it on every call as the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Get a key when you start a plan.\ndocs: https://matchwire.win/docs/\n"
source_yaml_url: https://artifacts.apis.io/matchwire-win/authentication/matchwire-win-authentication.yml
summary_line: 1 scheme
tags:
- Prediction Markets
- Market Data
- Sports Betting
- Real-Time Streaming
- Alias Mapping
- Commercial License
---
