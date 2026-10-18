---
anonymous_access: false
api_key_in: []
api_specs:
- filename: metal-openapi-generated.yml
  format: yaml
  label: Metal API
  slug: metal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metal/refs/heads/main/openapi/_ae-authored/metal-openapi-generated.yml
auth_types: []
description: Authentication schemes for Metal API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Metal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Metal
provider_slug: metal
scheme_count: 2
schemes:
- evidence: With basic authentication, you use your username and password to authenticate your HTTP requests.
  header: Authorization
  how_to_obtain: Use your username and password provided for the Protocol account.
  location: header
  name: Basic authentication
  type: http-basic
- evidence: The recommended way to authenticate with the Protocol API is by using OAuth2. When establishing a connection using OAuth2, you will need your access token — you will find it in the Protocol dashboard under API settings.
  header: x-api-key
  how_to_obtain: Retrieve the access token from the Protocol dashboard under API settings.
  location: header
  name: OAuth2 with bearer token
  type: http-bearer
slug: metal-authentication
source_filename: metal-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.metal.build/authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.metal.build/authentication\nsources:\n- https://docs.metal.build/authentication\n- https://docs.metal.build/token-locks\n- https://docs.metal.build/get-tokens\n- https://docs.metal.build/get-holders\ndescription: Authentication schemes for Metal API\nschemes:\n- type: http-basic\n  name: Basic authentication\n  evidence: With basic authentication, you use your username and password to authenticate your HTTP requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Use your username and password provided for the Protocol account.\n- type: http-bearer\n  name: OAuth2 with bearer token\n  evidence: The recommended way to authenticate with the Protocol API is by using OAuth2. When establishing a connection using OAuth2, you will\n    need your access token — you will find it in the Protocol dashboard under API settings.\n  location: header\n  header: x-api-key\n\
  \  how_to_obtain: Retrieve the access token from the Protocol dashboard under API settings.\ndocs: https://docs.metal.build/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metal/refs/heads/main/authentication/metal-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Platform
- Cloud
- DeveloperTools
- WebApplications
---
