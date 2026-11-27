---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: nimo Authentication
name_suffix: Authentication
oauth_flows: []
overview: nimo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: nimo
provider_slug: heynimo-com
scheme_count: 1
schemes:
- evidence: Use bearer auth Reference the secret through the client's documented credential or environment mechanism, then send the resolved value in the Authorization bearer header.
  header: Authorization
  how_to_obtain: Create the key in Settings and provide it through the client's local secret or documented environment-reference mechanism.
  location: header
  name: API Key
  type: http-bearer
slug: heynimo-com-authentication
source_filename: heynimo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://heynimo.com/docs/billing-and-api-keys
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://heynimo.com/docs/billing-and-api-keys\nsources:\n- https://heynimo.com/docs/billing-and-api-keys\n- https://heynimo.com/docs/billing-and-api-keys.md\n- https://heynimo.com/docs\n- https://heynimo.com/docs/setup\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Use bearer auth Reference the secret through the client's documented credential or environment mechanism, then send the resolved value\n    in the Authorization bearer header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create the key in Settings and provide it through the client's local secret or documented environment-reference mechanism.\ndocs: https://heynimo.com/docs/billing-and-api-keys\n"
source_yaml_url: https://artifacts.apis.io/heynimo-com/authentication/heynimo-com-authentication.yml
summary_line: 1 scheme
tags:
- website-performance
- speed monitoring
- performance alerts
- site audits
---
