---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bits-technology-openapi-generated.yml
  format: yaml
  label: Bits Technology API
  slug: bits-technology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bits-technology/refs/heads/main/openapi/_ae-authored/bits-technology-openapi-generated.yml
auth_types: []
description: Authentication schemes as published on Bits Technology documentation
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bits Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bits Technology declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bits Technology
provider_slug: bits-technology
scheme_count: 1
schemes:
- evidence: The access token is a bearer token and the holder of the token is authorized to create applications and read application data.
  header: Authorization
  how_to_obtain: Obtain the token via the OAuth client_credentials flow described above and include it in the Authorization header as "Bearer <accessToken>".
  location: header
  name: Bearer token
  type: http-bearer
slug: bits-technology-authentication
source_filename: bits-technology-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bits.bi/api-reference/authentication-and-authorization
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bits.bi/api-reference/authentication-and-authorization\nsources:\n- https://docs.bits.bi/api-reference/authentication-and-authorization\n- https://www.bits.bi/use-cases/onboarding\n- https://docs.bits.bi/getting-started\n- https://docs.bits.bi/sandbox\ndescription: Authentication schemes as published on Bits Technology documentation\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: The access token is a bearer token and the holder of the token is authorized to create applications and read application data.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the token via the OAuth client_credentials flow described above and include it in the Authorization header as \"Bearer\n    <accessToken>\".\ndocs: https://docs.bits.bi/api-reference/authentication-and-authorization\nnote: 1 extracted row(s) were dropped because their quote was not\
  \ on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bits-technology/refs/heads/main/authentication/bits-technology-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AML
- Compliance
- Fintech
- Europe
---
