---
anonymous_access: false
api_key_in: []
api_specs:
- filename: snapgen-org-openapi-generated.yml
  format: yaml
  label: SnapGen API
  slug: snapgen-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapgen-org/openapi/_ae-authored/snapgen-org-openapi-generated.yml
auth_types: []
description: SnapGen authenticates API requests with a secret API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: SnapGen Authentication
name_suffix: Authentication
oauth_flows: []
overview: SnapGen declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SnapGen
provider_slug: snapgen-org
scheme_count: 1
schemes:
- evidence: SnapGen authenticates API requests with a secret API key.
  header: Authorization
  how_to_obtain: Create a new key in the SnapGen Console under API Keys and copy it when shown.
  location: header
  name: API Key
  type: http-bearer
slug: snapgen-org-authentication
source_filename: snapgen-org-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.snapgen.org/authentication.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.snapgen.org/authentication.md\nsources:\n- https://docs.snapgen.org/authentication.md\n- https://docs.snapgen.org/quickstart.md\ndescription: SnapGen authenticates API requests with a secret API key.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: SnapGen authenticates API requests with a secret API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a new key in the SnapGen Console under API Keys and copy it when shown.\ndocs: https://docs.snapgen.org/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/snapgen-org/authentication/snapgen-org-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Audio Generation
- Multi-Modal
---
