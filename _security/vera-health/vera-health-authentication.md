---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vera-health-chat-api-openapi.yml
  format: yaml
  label: Vera Health Chat API
  slug: vera-health-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vera-health/openapi/vera-health-chat-api-openapi.yml
auth_types: []
description: Authentication methods for Vera Health API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vera Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vera Health declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vera Health
provider_slug: vera-health
scheme_count: 1
schemes:
- evidence: Send a POST request to `/api/chat/v2` with your API key in the `x-api-key` header
  header: x-api-key
  how_to_obtain: Contact support@verahealth.ai to request credentials.
  location: header
  name: API Key
  type: apiKey
slug: vera-health-authentication
source_filename: vera-health-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.verahealth.ai/docs/quickstart.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.verahealth.ai/docs/quickstart.md\nsources:\n- https://docs.verahealth.ai/docs/quickstart.md\n- https://docs.verahealth.ai/docs/quickstart\ndescription: Authentication methods for Vera Health API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Send a POST request to `/api/chat/v2` with your API key in the `x-api-key` header\n  location: header\n  header: x-api-key\n  how_to_obtain: Contact support@verahealth.ai to request credentials.\ndocs: https://docs.verahealth.ai/docs/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/vera-health/authentication/vera-health-authentication.yml
summary_line: 1 scheme
tags:
- Health
- AI
- Clinical Decision Support
- Medical Knowledge
- Healthcare
---
