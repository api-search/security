---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lunacal-ai-openapi-generated.yml
  format: yaml
  label: Lunacal API
  slug: lunacal-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lunacal-ai/openapi/_ae-authored/lunacal-ai-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lunacal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lunacal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lunacal
provider_slug: lunacal-ai
scheme_count: 1
schemes:
- evidence: Just send a valid API key in the `Authorization` header;
  header: Authorization
  how_to_obtain: 'Create an API key in Settings → Developer, then copy the key and use it as `Authorization: Bearer <YOUR_API_KEY>`.'
  location: header
  name: API key
  type: apiKey
slug: lunacal-ai-authentication
source_filename: lunacal-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://help.lunacal.ai/api/authentication.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.lunacal.ai/api/authentication.md\nsources:\n- https://help.lunacal.ai/api/authentication.md\n- https://help.lunacal.ai/event-types/event-setup.md\n- https://help.lunacal.ai/event-types/setup-zoom-video.md\n- https://help.lunacal.ai/availability-configuration.md\nschemes:\n- type: apiKey\n  name: API key\n  evidence: Just send a valid API key in the `Authorization` header;\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create an API key in Settings → Developer, then copy the key and use it as `Authorization: Bearer <YOUR_API_KEY>`.'\ndocs: https://help.lunacal.ai/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/lunacal-ai/authentication/lunacal-ai-authentication.yml
summary_line: 1 scheme
tags:
- Scheduling
- Appointment
- Artificial Intelligence
- Software-as-a-Service
- Business
---
