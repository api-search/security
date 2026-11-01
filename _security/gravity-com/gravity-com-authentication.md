---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Gravity Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gravity declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Gravity
provider_slug: gravity-com
scheme_count: 2
schemes:
- description: WordPress cookie authentication for plugins/themes running on the site.
  details: Uses logged-in user cookies; requires WordPress nonce _gf_json_nonce for API calls.
  type: cookie
- description: Expiring signature authentication for external applications.
  example:
    request: GET /forms/1/entries?api_key=1234&expires=1369749344&signature=uJEnk0EoQ4d3...
  parameters:
  - description: Public API key defined in settings.
    name: api_key
  - description: UNIX timestamp expiration.
    name: expires
  - description: Base64 HMAC-SHA1 of "api_key:HTTP_METHOD:route:expires".
    name: signature
  type: signature
slug: gravity-com-authentication
source_filename: gravity-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.gravityforms.com/web-api/\nschemes:\n  - type: cookie\n    description: WordPress cookie authentication for plugins/themes running on the site.\n    details: \"Uses logged-in user cookies; requires WordPress nonce _gf_json_nonce for API calls.\"\n  - type: signature\n    description: Expiring signature authentication for external applications.\n    parameters:\n      - name: api_key\n        description: Public API key defined in settings.\n      - name: expires\n        description: UNIX timestamp expiration.\n      - name: signature\n        description: Base64 HMAC-SHA1 of \"api_key:HTTP_METHOD:route:expires\".\n    example:\n      request: \"GET /forms/1/entries?api_key=1234&expires=1369749344&signature=uJEnk0EoQ4d3...\"\n"
source_yaml_url: https://artifacts.apis.io/gravity-com/authentication/gravity-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- WordPress
- Forms
- Automation
- Marketplace
---
