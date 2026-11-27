---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hanchu-ess-openapi-generated.yml
  format: yaml
  label: Hanchu ESS API
  slug: hanchu-ess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hanchu-ess/openapi/_ae-authored/hanchu-ess-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hanchu ESS Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hanchu ESS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hanchu ESS
provider_slug: hanchu-ess
scheme_count: 1
schemes:
- authorize_url: https://idaas-sandbox.hanchuess.com/portal/oauth/authorize
  evidence: IDaaS authentication support under `client_credentials` and `authorization_code`
  flows:
  - client_credentials
  - authorization_code
  how_to_obtain: Your organisation should have received client id and secret by email or slack during initial setup; contact Hanchu if not.
  name: OAuth2Auth
  scopes:
  - all
  token_url: https://idaas-sandbox.hanchuess.com/portal/oauth/token
  type: oauth2
slug: hanchu-ess-authentication
source_filename: hanchu-ess-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hanchuess.com/home/easy-connect/authentication.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hanchuess.com/home/easy-connect/authentication.md\nsources:\n- https://docs.hanchuess.com/home/easy-connect/authentication.md\n- https://docs.hanchuess.com/home/customer-lifecycle/onboarding.md\ndescription: Authentication\nschemes:\n- type: oauth2\n  name: OAuth2Auth\n  evidence: IDaaS authentication support under `client_credentials` and `authorization_code`\n  flows:\n  - client_credentials\n  - authorization_code\n  token_url: https://idaas-sandbox.hanchuess.com/portal/oauth/token\n  authorize_url: https://idaas-sandbox.hanchuess.com/portal/oauth/authorize\n  scopes:\n  - all\n  how_to_obtain: Your organisation should have received client id and secret by email or slack during initial setup; contact Hanchu if not.\ndocs: https://docs.hanchuess.com/home/easy-connect/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/hanchu-ess/authentication/hanchu-ess-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Energy
- Storage
- Battery
- Renewables
- Smart Grid
---
