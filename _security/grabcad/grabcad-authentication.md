---
api_key_in: []
auth_types:
- account-login
description: ''
kind: authentication
layout: security
method: searched
name: Grabcad Authentication
name_suffix: Authentication
oauth_flows: []
overview: GrabCAD secures its APIs with account-login across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GrabCAD
provider_slug: grabcad
scheme_count: 1
schemes:
- description: Authentication uses GrabCAD account credentials. Interactive docs require login; programmatic access is provisioned through the GrabCAD Software Partner Program (grabcad.com/software-partner/become-a-partner).
  login_url: https://print-api.grabcad.com/obscure/login
  name: grabcad-account
  sources:
  - searched:print-api.grabcad.com/public/documentation
  type: account-login
slug: grabcad-authentication
source_filename: grabcad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://print-api.grabcad.com/public/documentation\ndocs: https://print-api.grabcad.com/public/documentation\nsummary:\n  types:\n  - account-login\n  notes: 'The GrabCAD Print API is gated behind GrabCAD account credentials and the\n    GrabCAD Software Partner Program. The public documentation endpoint presents a\n    login form (\"Please login using your GrabCAD credentials\") and an OAuth-style\n    authorization path at /obscure/login; the machine-facing token/authorization\n    scheme is not published on the open web and requires partner enrollment. No\n    OpenAPI/Swagger securitySchemes are publicly available to derive from.'\nschemes:\n- name: grabcad-account\n  type: account-login\n  description: 'Authentication uses GrabCAD account credentials. Interactive docs\n    require login; programmatic access is provisioned through the GrabCAD Software\n    Partner Program (grabcad.com/software-partner/become-a-partner).'\n\
  \  login_url: https://print-api.grabcad.com/obscure/login\n  sources:\n  - searched:print-api.grabcad.com/public/documentation\npartner_program: https://grabcad.com/software-partner/become-a-partner\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grabcad/refs/heads/main/authentication/grabcad-authentication.yml
summary_line: account-login · 1 scheme
tags:
- Company
- B2B
- 3D Printing
- Additive Manufacturing
- CAD
- Manufacturing
- Hardware
- Developer SDK
---
