---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Claimhit Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: claimhit-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: claimhit-com
provider_slug: claimhit-com
scheme_count: 2
schemes:
- description: 'A ClaimHit API key, `ch_live_…`, as `Authorization: Bearer <key>`.'
  name: ApiKey
  scheme: bearer
  type: http
- description: OAuth 2.1 authentication via the ClaimHit connector, recommended for Claude integration.
  flow: authorizationCode
  type: oauth2
slug: claimhit-com-authentication
source_filename: claimhit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://app.claimhit.com/connectors\nschemes:\n  - type: http\n    scheme: bearer\n    name: ApiKey\n    description: \"A ClaimHit API key, `ch_live_…`, as `Authorization: Bearer <key>`.\"\n  - type: oauth2\n    flow: authorizationCode\n    description: \"OAuth 2.1 authentication via the ClaimHit connector, recommended for Claude integration.\"\n"
source_yaml_url: https://artifacts.apis.io/claimhit-com/authentication/claimhit-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Patent
- Intelligence
- LegalTech
- IP
---
