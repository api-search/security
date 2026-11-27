---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: OwlCAD Authentication
name_suffix: Authentication
oauth_flows: []
overview: OwlCAD secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OwlCAD
provider_slug: owlcad-com
scheme_count: 1
schemes:
- bearerFormat: PAT
  description: Personal Access Token generated in OwlCAD Account → Access tokens. Pro-only, and re-checked on every request.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/owlcad-com-openapi.json
  type: http
slug: owlcad-com-authentication
source_filename: owlcad-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/owlcad-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  description: Personal Access Token generated in OwlCAD Account → Access tokens. Pro-only,\n    and re-checked on every request.\n  sources:\n  - openapi/owlcad-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/owlcad-com/authentication/owlcad-com-authentication.yml
summary_line: http · 1 scheme
tags:
- CAD
- 3D Printing
- Browser
- Parametric
- Free
---
