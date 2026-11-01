---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication via Bearer token
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Daxko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daxko declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Daxko
provider_slug: daxko
scheme_count: 1
schemes:
- evidence: 'The authorization header must be in the format Authorization: Bearer <token> where token is the response from the POST /auth/token API resource.'
  header: Authorization
  how_to_obtain: Obtain the token by calling the POST /auth/token endpoint.
  location: header
  name: Bearer
  type: http-bearer
slug: daxko-authentication
source_filename: daxko-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.partners.daxko.com/tutorials/club_automation_getting_started/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.partners.daxko.com/tutorials/club_automation_getting_started/\nsources:\n- https://docs.partners.daxko.com/tutorials/club_automation_getting_started/\n- https://docs.partners.daxko.com/tutorials/spectrum_vanguard_getting_started/\ndescription: Authentication via Bearer token\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'The authorization header must be in the format Authorization: Bearer <token> where token is the response from the POST /auth/token\n    API resource.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the token by calling the POST /auth/token endpoint.\ndocs: https://docs.partners.daxko.com/tutorials/club_automation_getting_started/\n"
source_yaml_url: https://artifacts.apis.io/daxko/authentication/daxko-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Software
- Fitness
- Nonprofit
- SaaS
---
