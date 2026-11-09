---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Argus Ing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argus declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Argus
provider_slug: argus-ing
scheme_count: 1
schemes:
- authorizationUrl: https://argus.ing/auth/login
  flow: authorization_code
  scopes:
    recon: Access to recon data
  tokenUrl: https://argus.ing/auth/token
  type: oauth2
slug: argus-ing-authentication
source_filename: argus-ing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://argus.ing/.well-known/oauth-protected-resource\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    authorizationUrl: https://argus.ing/auth/login\n    tokenUrl: https://argus.ing/auth/token\n    scopes:\n      recon: \"Access to recon data\"\n"
source_yaml_url: https://artifacts.apis.io/argus-ing/authentication/argus-ing-authentication.yml
summary_line: 1 scheme
tags:
- Tender
- Procurement
- Analytics
- Artificial Intelligence
- Belgium
---
