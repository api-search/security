---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flowboard-studio-openapi-generated.yml
  format: yaml
  label: Flowboard API
  slug: flowboard-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowboard-studio/openapi/_ae-authored/flowboard-studio-openapi-generated.yml
auth_types: []
description: Authentication schemes extracted from Flowboard documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Flowboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flowboard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Flowboard
provider_slug: flowboard-studio
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer $FLOWBOARD_PERSONAL_KEY"'
  header: Authorization
  location: header
  type: http-bearer
slug: flowboard-studio-authentication
source_filename: flowboard-studio-authentication.yml
source_heading: Authentication Profile
source_url: https://flowboard.studio/developers/quickstart.sh
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://flowboard.studio/developers/quickstart.sh\nsources:\n- https://flowboard.studio/developers/quickstart.sh\n- https://flowboard.studio/docs/quickstart\ndescription: Authentication schemes extracted from Flowboard documentation.\nschemes:\n- type: http-bearer\n  evidence: '-H \"Authorization: Bearer $FLOWBOARD_PERSONAL_KEY\"'\n  location: header\n  header: Authorization\ndocs: https://flowboard.studio/developers/quickstart.sh\n"
source_yaml_url: https://artifacts.apis.io/flowboard-studio/authentication/flowboard-studio-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Architecture
- Whiteboard
- Visualization
- Automation
---
