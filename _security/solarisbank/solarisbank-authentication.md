---
anonymous_access: false
api_key_in: []
api_specs:
- filename: solarisbank-openapi-generated.yml
  format: yaml
  label: solarisBank AG API
  slug: solarisbank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/solarisbank/openapi/_ae-authored/solarisbank-openapi-generated.yml
auth_types: []
description: Solaris uses the OAuth2 framework for authentication. To access the API, you must exchange your credentials for a short-lived **Bearer Access Token**.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Solarisbank Authentication
name_suffix: Authentication
oauth_flows: []
overview: solarisBank AG declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: solarisBank AG
provider_slug: solarisbank
scheme_count: 1
schemes:
- evidence: Solaris uses the OAuth2 framework for authentication.
  flows:
  - client_credentials
  how_to_obtain: Provide your client_id and client_secret encoded in Base64 in the Authorization header (Basic {base64_string}) and POST to the token URL with grant_type=client_credentials and scope=partners.
  name: OAuth2 Client Credentials
  scopes:
  - partners
  token_url: https://auth.solaris-sandbox.de/oauth2/token
  type: oauth2
slug: solarisbank-authentication
source_filename: solarisbank-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.solarisgroup.com/guides/authentication.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.solarisgroup.com/guides/authentication.md\nsources:\n- https://docs.solarisgroup.com/guides/authentication.md\n- https://docs.solarisgroup.com/guides/authentication/device-binding.md\n- https://docs.solarisgroup.com/guides/authentication/strong-customer-authentication.md\n- https://docs.solarisgroup.com/api-reference/authentication.md\ndescription: Solaris uses the OAuth2 framework for authentication. To access the API, you must exchange your credentials for a short-lived **Bearer\n  Access Token**.\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: Solaris uses the OAuth2 framework for authentication.\n  flows:\n  - client_credentials\n  token_url: https://auth.solaris-sandbox.de/oauth2/token\n  scopes:\n  - partners\n  how_to_obtain: Provide your client_id and client_secret encoded in Base64 in the Authorization header (Basic {base64_string})\
  \ and POST to the\n    token URL with grant_type=client_credentials and scope=partners.\ndocs: https://docs.solarisgroup.com/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/solarisbank/authentication/solarisbank-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Banking-as-a-Service
- Embedded Finance
- Europe
---
