---
anonymous_access: false
api_key_in: []
api_specs:
- filename: opn-ooo-openapi-generated.yml
  format: yaml
  label: Omise API
  slug: opn-ooo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opn-ooo/openapi/_ae-authored/opn-ooo-openapi-generated.yml
auth_types: []
description: Omise uses HTTP Basic Authentication with API keys.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Opn Ooo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Omise declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Omise
provider_slug: opn-ooo
scheme_count: 1
schemes:
- evidence: We use HTTP Basic Authentication .
  header: Authorization
  how_to_obtain: Find the public, secret, or chain key on your Omise dashboard.
  location: header
  name: API Key
  type: http-basic
slug: opn-ooo-authentication
source_filename: opn-ooo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.omise.co/api-authentication
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.omise.co/api-authentication\nsources:\n- https://docs.omise.co/api-authentication\n- https://docs.omise.co/api-authentication\n- https://docs.omise.co/tokens-api\n- https://docs.omise.co/\ndescription: Omise uses HTTP Basic Authentication with API keys.\nschemes:\n- type: http-basic\n  name: API Key\n  evidence: We use HTTP Basic Authentication .\n  location: header\n  header: Authorization\n  how_to_obtain: Find the public, secret, or chain key on your Omise dashboard.\nnote: The same HTTP Basic scheme is used for public keys, secret keys, and chain keys; the key is supplied as the username and the password is\n  left blank.\ndocs: https://docs.omise.co/api-authentication\n"
source_yaml_url: https://artifacts.apis.io/opn-ooo/authentication/opn-ooo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- API
- FinTech
- Southeast-Asia
---
