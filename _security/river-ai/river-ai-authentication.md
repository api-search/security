---
anonymous_access: false
api_key_in: []
api_specs:
- filename: river-ai-openapi-generated.yml
  format: yaml
  label: River AI, Inc. API
  slug: river-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/river-ai/openapi/_ae-authored/river-ai-openapi-generated.yml
auth_types: []
description: River API uses an API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: River Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: River AI, Inc. declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: River AI, Inc.
provider_slug: river-ai
scheme_count: 1
schemes:
- evidence: 'curl --fail-with-body https://api.river.ai/v1/chat/completions \  -H "Authorization: Bearer $RIVER_API_KEY"'
  header: Authorization
  how_to_obtain: Create an API key on the API Keys page of the River Console.
  location: header
  name: Bearer
  type: http-bearer
slug: river-ai-authentication
source_filename: river-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.river.ai/quickstart.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.river.ai/quickstart.md\nsources:\n- https://docs.river.ai/quickstart.md\n- https://docs.river.ai/guides/inference.md\ndescription: River API uses an API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl --fail-with-body https://api.river.ai/v1/chat/completions \\  -H \"Authorization: Bearer $RIVER_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key on the API Keys page of the River Console.\ndocs: https://docs.river.ai/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/river-ai/authentication/river-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Automation
- Data Analytics
- Enterprise
---
