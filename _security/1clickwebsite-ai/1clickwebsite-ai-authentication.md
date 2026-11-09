---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 1Clickwebsite Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1ClickWebsite.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 1ClickWebsite.ai
provider_slug: 1clickwebsite-ai
scheme_count: 2
schemes:
- bearerFormat: 1ClickWebsite API key
  description: Account keys begin with `lgen_`; white-label agency keys begin with `1cw_agency_`.
  scheme: bearer
  type: http
- description: WordPress username and application password. Remove display spaces from the application password.
  scheme: basic
  type: http
slug: 1clickwebsite-ai-authentication
source_filename: 1clickwebsite-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://www.1clickwebsite.ai/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: 1ClickWebsite API key\n    description: Account keys begin with `lgen_`; white-label agency keys begin with `1cw_agency_`.\n  - type: http\n    scheme: basic\n    description: WordPress username and application password. Remove display spaces from the application password.\n"
source_yaml_url: https://artifacts.apis.io/1clickwebsite-ai/authentication/1clickwebsite-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- SEO
- WordPress
- Agency
- Automation
---
