---
anonymous_access: false
api_key_in: []
api_specs:
- filename: farpy-com-api-openapi.json
  format: json
  label: FARPY Public API API
  slug: farpy-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/_original/farpy-com-api-openapi.json
auth_types: []
description: Authentication schemes for Farpy API as described on the Quickstart page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Farpy Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Farpy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Farpy
provider_slug: farpy-com
scheme_count: 1
schemes:
- evidence: 'Inspect/start: Job API farpy_agent_… Bearer key.'
  header: Authorization
  how_to_obtain: Export a farpy_agent_ key with jobs:inspect jobs:quote jobs:start jobs:status
  location: header
  name: farpy_agent_key
  type: http-bearer
slug: farpy-com-authentication
source_filename: farpy-com-authentication.yml
source_heading: Authentication Profile
source_url: https://farpy.com/api/quickstart/
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://farpy.com/api/quickstart/\nsources:\n- https://farpy.com/api/quickstart/\ndescription: Authentication schemes for Farpy API as described on the Quickstart page.\nschemes:\n- type: http-bearer\n  name: farpy_agent_key\n  evidence: 'Inspect/start: Job API farpy_agent_… Bearer key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Export a farpy_agent_ key with jobs:inspect jobs:quote jobs:start jobs:status\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are mentioned on the page.\ndocs: https://farpy.com/api/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/farpy-com/authentication/farpy-com-authentication.yml
summary_line: 1 scheme
tags:
- GPU
- Rendering
- Blender
- Cloud
- Distributed
---
