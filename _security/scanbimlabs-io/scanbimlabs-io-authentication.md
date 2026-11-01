---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Scanbimlabs Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: scanbimlabs-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: scanbimlabs-io
provider_slug: scanbimlabs-io
scheme_count: 2
schemes:
- description: API key for programmatic access
  in: header
  name: X-ScanBIM-Key
  official: true
  type: apiKey
- description: Session cookie after login
  name: sb_session
  official: true
  type: cookie
slug: scanbimlabs-io-authentication
source_filename: scanbimlabs-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: \"derive-authentication script\"\nschemes:\n  - type: apiKey\n    name: X-ScanBIM-Key\n    in: header\n    description: API key for programmatic access\n    official: true\n  - type: cookie\n    name: sb_session\n    description: Session cookie after login\n    official: true\n"
source_yaml_url: https://artifacts.apis.io/scanbimlabs-io/authentication/scanbimlabs-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
