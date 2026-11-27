---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as published on the page
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ichabod Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ichabod declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ichabod
provider_slug: ichabod-dev
scheme_count: 1
schemes:
- evidence: 'with the header `Authorization: Bearer ick_...`.'
  header: Authorization
  how_to_obtain: An API key (`ick_...`) is provided once at the end of signup and shown exactly once on the dashboard.
  location: header
  name: Bearer token
  type: http-bearer
slug: ichabod-dev-authentication
source_filename: ichabod-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ichabod.dev/quickstart.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ichabod.dev/quickstart.md\nsources:\n- https://docs.ichabod.dev/quickstart.md\ndescription: Authentication methods as published on the page\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'with the header `Authorization: Bearer ick_...`.'\n  location: header\n  header: Authorization\n  how_to_obtain: An API key (`ick_...`) is provided once at the end of signup and shown exactly once on the dashboard.\ndocs: https://docs.ichabod.dev/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/ichabod-dev/authentication/ichabod-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
