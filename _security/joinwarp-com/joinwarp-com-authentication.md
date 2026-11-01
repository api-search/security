---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Warp API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Joinwarp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Warp declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Warp
provider_slug: joinwarp-com
scheme_count: 1
schemes:
- evidence: The Warp API uses API keys to authenticate requests. Include your API key in the `x-api-key` header on every request.
  header: x-api-key
  how_to_obtain: Create a company API key in the Warp dashboard (https://app.joinwarp.com).
  location: header
  name: API Key
  type: apiKey
slug: joinwarp-com-authentication
source_filename: joinwarp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.warp.co/authentication.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.warp.co/authentication.md\nsources:\n- https://docs.warp.co/authentication.md\n- https://help.joinwarp.com/articles/9593326177-multi-factor-authentication-mfa-on-warp\n- https://docs.warp.co/quickstart.md\n- https://docs.warp.co/webhooks/worker-onboarding-completed.md\ndescription: Authentication schemes for Warp API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The Warp API uses API keys to authenticate requests. Include your API key in the `x-api-key` header on every request.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a company API key in the Warp dashboard (https://app.joinwarp.com).\nnote: No OAuth2 or other authentication methods are documented.\ndocs: https://docs.warp.co/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/joinwarp-com/authentication/joinwarp-com-authentication.yml
summary_line: 1 scheme
tags:
- Payroll
- Benefits
- Tax Compliance
- IT Management
- Global Payroll
- HRIS
- AI Agents
---
