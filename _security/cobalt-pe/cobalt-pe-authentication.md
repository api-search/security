---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cobalt Pe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cobalt declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cobalt
provider_slug: cobalt-pe
scheme_count: 2
schemes:
- description: Personal API token passed in Authorization header as "Bearer <token>"
  scheme: bearer
  type: http
- description: Organization token required for organization-scoped requests
  in: header
  name: X-Org-Token
  type: apiKey
slug: cobalt-pe-authentication
source_filename: cobalt-pe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://developer.cobalt.io/v2/\nschemes:\n  - type: http\n    scheme: bearer\n    description: Personal API token passed in Authorization header as \"Bearer <token>\"\n  - type: apiKey\n    in: header\n    name: X-Org-Token\n    description: Organization token required for organization-scoped requests"
source_yaml_url: https://artifacts.apis.io/cobalt-pe/authentication/cobalt-pe-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
