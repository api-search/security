---
anonymous_access: false
api_key_in: []
api_specs:
- filename: banksapi-openapi-generated.yml
  format: yaml
  label: fineconomy API
  slug: banksapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/banksapi/openapi/_ae-authored/banksapi-openapi-generated.yml
auth_types: []
description: Authentication is based on the (2‑legged) OAuth2 protocol.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Banksapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: fineconomy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: fineconomy
provider_slug: banksapi
scheme_count: 1
schemes:
- evidence: we're basing our authentication on the (2-legged) OAuth2 protocol
  flows:
  - client_credentials
  - password
  how_to_obtain: Use the POST /auth/oauth2/token endpoint with grant_type=client_credentials for management‑level tokens or grant_type=password with username and password for user‑level tokens.
  name: OAuth2
  scopes:
  - http://banksapi.io/customer/read
  - http://banksapi.io/provider/read
  - http://banksapi.io/customer/modify
  - http://banksapi.io/customer/ueberweisung
  - auth/tenants/users/create
  token_url: /auth/oauth2/token
  type: oauth2
slug: banksapi-authentication
source_filename: banksapi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.banksapi.de/guide/quickstart.html
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.banksapi.de/guide/quickstart.html\nsources:\n- https://docs.banksapi.de/guide/quickstart.html\ndescription: Authentication is based on the (2‑legged) OAuth2 protocol.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: we're basing our authentication on the (2-legged) OAuth2 protocol\n  flows:\n  - client_credentials\n  - password\n  token_url: /auth/oauth2/token\n  scopes:\n  - http://banksapi.io/customer/read\n  - http://banksapi.io/provider/read\n  - http://banksapi.io/customer/modify\n  - http://banksapi.io/customer/ueberweisung\n  - auth/tenants/users/create\n  how_to_obtain: Use the POST /auth/oauth2/token endpoint with grant_type=client_credentials for management‑level tokens or grant_type=password\n    with username and password for user‑level tokens.\ndocs: https://docs.banksapi.de/guide/quickstart.html\n"
source_yaml_url: https://artifacts.apis.io/banksapi/authentication/banksapi-authentication.yml
summary_line: 1 scheme
tags:
- Banking
- API
- FinTech
- Payments
- DataAnalytics
---
