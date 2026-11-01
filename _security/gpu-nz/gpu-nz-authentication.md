---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gpu Nz Authentication
name_suffix: Authentication
oauth_flows: []
overview: gpu.nz declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: gpu.nz
provider_slug: gpu-nz
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer $GPUNZ_API_KEY"'
  header: Authorization
  how_to_obtain: 'Create one in the console: Keys → API keys. Or run gpunz login and the key is issued for you.'
  location: header
  name: Bearer
  type: http-bearer
slug: gpu-nz-authentication
source_filename: gpu-nz-authentication.yml
source_heading: Authentication Profile
source_url: https://gpu.nz/en/docs
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gpu.nz/en/docs\nsources:\n- https://gpu.nz/en/docs\ndescription: Authentication uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '-H \"Authorization: Bearer $GPUNZ_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create one in the console: Keys → API keys. Or run gpunz login and the key is issued for you.'\ndocs: https://gpu.nz/en/docs\n"
source_yaml_url: https://artifacts.apis.io/gpu-nz/authentication/gpu-nz-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- GPU
- Rentals
- Artificial Intelligence
- Compute
---
