---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AffiliateSpy Authentication
name_suffix: Authentication
oauth_flows: []
overview: AffiliateSpy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AffiliateSpy
provider_slug: affiliatespy-io
scheme_count: 1
schemes:
- bearerFormat: asp_live_…
  description: Per-user API key from https://www.affiliatespy.io/dashboard/settings?tab=api. Included on every paid plan.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/affiliatespy-io-openapi.json
  type: http
slug: affiliatespy-io-authentication
source_filename: affiliatespy-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/affiliatespy-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: asp_live_…\n  description: Per-user API key from https://www.affiliatespy.io/dashboard/settings?tab=api.\n    Included on every paid plan.\n  sources:\n  - openapi/affiliatespy-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/affiliatespy-io/authentication/affiliatespy-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Affiliate Marketing
- Intelligence
- Artificial Intelligence
- Software-as-a-Service
---
