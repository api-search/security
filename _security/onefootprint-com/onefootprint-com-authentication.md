---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Footprint API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Onefootprint Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Footprint declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Footprint
provider_slug: onefootprint-com
scheme_count: 1
schemes:
- evidence: Your backend authenticates each request to the Footprint API with the `X-Footprint-Secret-Key` header, whose value is an API key from the developer dashboard.
  header: X-Footprint-Secret-Key
  how_to_obtain: View and manage your API keys in the developer dashboard (https://dashboard.onefootprint.com/developers).
  location: header
  name: apiKey
  type: apiKey
slug: onefootprint-com-authentication
source_filename: onefootprint-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.onefootprint.com/llms/api-reference/authentication.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.onefootprint.com/llms/api-reference/authentication.md\nsources:\n- https://docs.onefootprint.com/llms/api-reference/authentication.md\n- https://docs.onefootprint.com/llms/articles/getting-started/introduction.md\n- https://docs.onefootprint.com/llms/articles/onboarding/introduction.md\n- https://docs.onefootprint.com/llms/articles/integrate/onboarding-sessions.md\ndescription: Authentication schemes for Footprint API\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Your backend authenticates each request to the Footprint API with the `X-Footprint-Secret-Key` header, whose value is an API key from\n    the developer dashboard.\n  location: header\n  header: X-Footprint-Secret-Key\n  how_to_obtain: View and manage your API keys in the developer dashboard (https://dashboard.onefootprint.com/developers).\ndocs: https://docs.onefootprint.com/llms/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/onefootprint-com/authentication/onefootprint-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Risk Management
- ESG
- Sustainability
---
