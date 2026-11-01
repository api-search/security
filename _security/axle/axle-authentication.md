---
anonymous_access: false
api_key_in: []
api_specs:
- filename: axle-api-openapi.yml
  format: yaml
  label: Axle API API
  slug: axle-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axle/openapi/_original/axle-api-openapi.yml
auth_types: []
description: Axle uses an API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Axle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Axle declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Axle
provider_slug: axle
scheme_count: 1
schemes:
- evidence: Your secret API key. This will be shared with you during onboarding and should be considered sensitive - it’s a password after all! Your secret will be matched with your client ID to authenticate your requests.
  header: x-client-secret
  location: header
  name: ApiKeyAuth
  type: apiKey
slug: axle-authentication
source_filename: axle-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.axle.insure/api-reference/tokens/exchange-token.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.axle.insure/api-reference/tokens/exchange-token.md\nsources:\n- https://docs.axle.insure/api-reference/tokens/exchange-token.md\n- https://docs.axle.insure/api-reference/tokens/descope-token.md\n- https://docs.axle.insure/guides/quickstart.md\ndescription: Axle uses an API key authentication scheme.\nschemes:\n- type: apiKey\n  name: ApiKeyAuth\n  evidence: Your secret API key. This will be shared with you during onboarding and should be considered sensitive - it’s a password after all!\n    Your secret will be matched with your client ID to authenticate your requests.\n  location: header\n  header: x-client-secret\ndocs: https://docs.axle.insure/api-reference/tokens/exchange-token.md\n"
source_yaml_url: https://artifacts.apis.io/axle/authentication/axle-authentication.yml
summary_line: 1 scheme
tags:
- Insurance
- AI
- Automation
- FinTech
- Platform
---
