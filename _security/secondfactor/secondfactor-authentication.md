---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for SecondFactor API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Secondfactor Authentication
name_suffix: Authentication
oauth_flows: []
overview: SecondFactor declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SecondFactor
provider_slug: secondfactor
scheme_count: 1
schemes:
- evidence: Send your API key in the X-API-Key header on every request.
  header: X-API-Key
  how_to_obtain: Create and revoke keys on the dashboard's API keys page.
  location: header
  name: X-API-Key
  type: apiKey
slug: secondfactor-authentication
source_filename: secondfactor-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.secondfactor.ai/authentication
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.secondfactor.ai/authentication\nsources:\n- https://docs.secondfactor.ai/authentication\n- https://docs.secondfactor.ai/\ndescription: Authentication schemes for SecondFactor API\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Send your API key in the X-API-Key header on every request.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create and revoke keys on the dashboard's API keys page.\ndocs: https://docs.secondfactor.ai/authentication\n"
source_yaml_url: https://artifacts.apis.io/secondfactor/authentication/secondfactor-authentication.yml
summary_line: 1 scheme
tags:
- Company
- OTP
- Authentication
- Multi-Channel
- Messaging
---
