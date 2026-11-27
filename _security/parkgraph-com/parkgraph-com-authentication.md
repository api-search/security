---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Park Graph Authentication
name_suffix: Authentication
oauth_flows: []
overview: Park Graph declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Park Graph
provider_slug: parkgraph-com
scheme_count: 1
schemes:
- evidence: All requests require a Bearer token.
  header: Authorization
  how_to_obtain: Get your API key from the dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: parkgraph-com-authentication
source_filename: parkgraph-com-authentication.yml
source_heading: Authentication Profile
source_url: https://parkgraph.com/developers/api
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://parkgraph.com/developers/api\nsources:\n- https://parkgraph.com/developers/api\n- https://parkgraph.com/developers/aws-marketplace\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All requests require a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Get your API key from the dashboard.\ndocs: https://parkgraph.com/developers/api\n"
source_yaml_url: https://artifacts.apis.io/parkgraph-com/authentication/parkgraph-com-authentication.yml
summary_line: 1 scheme
tags:
- Parking
- QR Payments
- Parking Management
- Contactless Payments
- Lot Owners
- Revenue Share
---
