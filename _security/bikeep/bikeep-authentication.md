---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bikeep-openapi-generated.yml
  format: yaml
  label: Bikeep API
  slug: bikeep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bikeep/openapi/_ae-authored/bikeep-openapi-generated.yml
auth_types: []
description: Bikeep supports three authentication methods. The only method that uses a standard authentication scheme is S2S OAuth2 (client credentials flow).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bikeep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bikeep declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bikeep
provider_slug: bikeep
scheme_count: 1
schemes:
- evidence: The simplest method. Your backend authenticates directly with Bikeep using client credentials.
  flows:
  - client_credentials
  how_to_obtain: Obtain a client_id and client_secret from Bikeep, then POST to the token endpoint with grant_type=client_credentials (or use Basic Auth). The response contains an access_token to be used in API calls.
  name: S2S OAuth2
  token_url: https://auth.bikeep.com/oauth2/token
  type: oauth2
slug: bikeep-authentication
source_filename: bikeep-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bikeep.com/authentication.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bikeep.com/authentication.md\nsources:\n- https://docs.bikeep.com/authentication.md\n- https://docs.bikeep.com/quickstart.md\ndescription: Bikeep supports three authentication methods. The only method that uses a standard authentication scheme is S2S OAuth2 (client credentials\n  flow).\nschemes:\n- type: oauth2\n  name: S2S OAuth2\n  evidence: The simplest method. Your backend authenticates directly with Bikeep using client credentials.\n  flows:\n  - client_credentials\n  token_url: https://auth.bikeep.com/oauth2/token\n  how_to_obtain: Obtain a client_id and client_secret from Bikeep, then POST to the token endpoint with grant_type=client_credentials (or use\n    Basic Auth). The response contains an access_token to be used in API calls.\ndocs: https://docs.bikeep.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/bikeep/authentication/bikeep-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Smart Parking
- Mobility
- IoT
- Sustainability
- Urban Infrastructure
---
