---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Marsello Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marsello declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Marsello
provider_slug: marsello
scheme_count: 1
schemes:
- flow: password
  scopes:
    https://dev.marsello.com/scope/read.all: Read access
    https://dev.marsello.com/scope/write.all: Write access
  tokenUrl: https://marselloexternal.b2clogin.com/marselloexternal.onmicrosoft.com/B2C_1_ROPC/oauth2/v2.0/token
  type: oauth2
slug: marsello-authentication
source_filename: marsello-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource: https://marsello.readme.io/reference/getting-started-with-marsello-api\nschemes:\n  - type: oauth2\n    flow: password\n    tokenUrl: https://marselloexternal.b2clogin.com/marselloexternal.onmicrosoft.com/B2C_1_ROPC/oauth2/v2.0/token\n    scopes:\n      https://dev.marsello.com/scope/write.all: Write access\n      https://dev.marsello.com/scope/read.all: Read access\n"
source_yaml_url: https://artifacts.apis.io/marsello/authentication/marsello-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Loyalty
- Marketing
- Retail
- Hospitality
---
