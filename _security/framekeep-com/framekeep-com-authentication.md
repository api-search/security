---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: framekeep-com-public-discovery-api-openapi.yml
  format: yaml
  label: Framekeep Public discovery API
  slug: framekeep-com-public-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framekeep-com/openapi/framekeep-com-public-discovery-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Framekeep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Framekeep secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Framekeep
provider_slug: framekeep-com
scheme_count: 1
schemes:
- description: Human-established secure browser session for studio administration. It is not accepted by the public v1 endpoints.
  in: cookie
  name: StudioSession
  parameter: framekeep_admin_session
  sources:
  - openapi/framekeep-com-openapi.json
  type: apiKey
slug: framekeep-com-authentication
source_filename: framekeep-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/framekeep-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: StudioSession\n  type: apiKey\n  in: cookie\n  parameter: framekeep_admin_session\n  description: Human-established secure browser session for studio administration. It is not\n    accepted by the public v1 endpoints.\n  sources:\n  - openapi/framekeep-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/framekeep-com/authentication/framekeep-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Photography
- Private Galleries
- Boudoir
- Branding
---
