---
anonymous_access: false
api_key_in: []
api_specs:
- filename: life360-product-api-openapi.yml
  format: yaml
  label: Life360 Product API
  slug: life360-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/life360/refs/heads/main/openapi/life360-product-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: none
name: Life360 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Life360 declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Life360
provider_slug: life360
scheme_count: 0
schemes: []
slug: life360-authentication
source_filename: life360-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: none\nsource: openapi/life360-openapi.yml, https://www.life360.com/.well-known/ai-plugin.json\nschemes: []\nnote: >-\n  The only published contract (Life360 WEB API v0.1, 4 GET operations under\n  /api/catalog on www.life360.com) declares no securitySchemes and no security\n  requirement, and the ai-plugin manifest that advertises it declares auth type none:\n  the catalog API is unauthenticated. Life360 documents no OAuth, API keys or scopes;\n  the member app's own API is private and undocumented. Note that on 2026-10-20 the\n  host answered 403 to a non-browser client, so access is gated by bot protection,\n  not by credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/life360/refs/heads/main/authentication/life360-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Consumer
- Family Safety
- Location
- GPS Tracking
- Bluetooth Trackers
- Mobile App
- Driving Safety
- Wearables
- Subscription
---
