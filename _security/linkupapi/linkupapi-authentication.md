---
anonymous_access: false
api_key_in: []
api_specs:
- filename: linkupapi-openapi-generated.yml
  format: yaml
  label: LinkupAPI API
  slug: linkupapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkupapi/refs/heads/main/openapi/_ae-authored/linkupapi-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Linkupapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkupAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LinkupAPI
provider_slug: linkupapi
scheme_count: 1
schemes:
- evidence: Your API key
  header: x-api-key
  how_to_obtain: Call the Login endpoint with LinkedIn email, password, and optional country to receive a login_token (valid for 365 days).
  location: header
  name: x-api-key
  type: apiKey
slug: linkupapi-authentication
source_filename: linkupapi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.linkupapi.com/api-reference/linkedin-engagement-api/getting-linkedin-cookie.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.linkupapi.com/api-reference/linkedin-engagement-api/getting-linkedin-cookie.md\nsources:\n- https://docs.linkupapi.com/api-reference/linkedin-engagement-api/getting-linkedin-cookie.md\n- https://docs.linkupapi.com/api-reference/linkup/authentication/login.md\n- https://docs.linkupapi.com/api-reference/linkup/authentication/verify.md\n- https://docs.linkupapi.com/api-reference/webhook-realtime/whatsapp-authentication.md\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: Your API key\n  location: header\n  header: x-api-key\n  how_to_obtain: Call the Login endpoint with LinkedIn email, password, and optional country to receive a login_token (valid for 365 days).\ndocs: https://docs.linkupapi.com/api-reference/linkedin-engagement-api/getting-linkedin-cookie.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkupapi/refs/heads/main/authentication/linkupapi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- Outreach
- AI
- Automation
---
